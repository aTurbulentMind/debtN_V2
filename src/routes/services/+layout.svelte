<script>
	import { goto } from '$app/navigation';
	let menuItems = ['Services', 'Support', 'Training'];
	let selected = '';

	const select = (name) => {
		selected = name;
		if (name === 'Services') {
			goto('/services');
		} else {
			goto('/services/' + name.toLowerCase());
		}
	};
</script>

<meni>
	<!-- Side menu -->
	<div>
		<ul>
			{#each menuItems as item (item)}
				<li class={selected === item ? 'selected' : ''} on:click={() => select(item)}>
					{item}
				</li>
			{/each}
		</ul>
	</div>

	<!-- Page content -->
	<div style="flex-grow: 1; padding: 20px;">
		<slot />
	</div>
</meni>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	meni {
		display: flex;

		ul {
			position: fixed;
			margin: 50vh 2vw;
			width: 8vw;
			border-right: 1px solid var(--back_Hallow);

			li {
				list-style: none;
				cursor: pointer;
			}
		}
	}

	.selected {
		background-color: var(--back_Alt);
		color: var(--back_Main);
	}
</style>
