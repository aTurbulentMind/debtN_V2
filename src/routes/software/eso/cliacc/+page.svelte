<script>
	let items = [
		{
			name: 'Client View Module',
			text: "The Client View Module allows clients to access an agency's Debt$Net® system from their location. Clients may review accounts they have turned over to the agency for collection. Access is password protected using remote access software and allows clients to review (but not modify) debtor accounts, payment history, notice history, promises made and collector notes."
		},
		{
			name: 'WebAccess Interface',
			text: 'Client Access Web LogoThe WebAccess Interface allows agencies to interface with a web vendor, giving your client the ability to view and submit new accounts, report payments and review reports. Debt$Net® creates a file that updates the information available to clients, which is then submitted to a web vendor. When WebAccess is coupled with the Client Upload ESO, agencies can import accounts and payment information submitted by the clients from the web.'
		}
	];
	let selected = 'Full Trust Accounting';
	let select = (name) => (selected = name);
</script>

<h1>ESO's</h1>

<ul class="add-ons">
	{#each items as item (item.name)}
		<li
			class={selected === item.name ? 'selected' : 'unselected'}
			on:click={() => select(item.name)}
		>
			{item.name}
			<p class={selected === item.name ? '' : 'hidden'}>
				{item.text}
			</p>
		</li>
	{/each}
</ul>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	h1,
	h3 {
		width: fit-content;
		position: flex;
		padding: 10vh 0 10vh 15vw;
	}

	.add-ons {
		display: grid;
		grid-template-columns: 1fr;
		list-style-type: none;
		width: 80vw;
		margin: 2vw 10vw;

		.selected {
			border: var(--bord);
			border-radius: var(--rad);
			background-color: var(--back_Alt);
			color: var(--back_Main);
		}

		.unselected {
			height: fit-content;
		}

		li {
			background-color: var(--highlight);
			border: var(--bord);
			border-radius: var(--rad);
			font-size: var(--f_lg);
			cursor: pointer;
			width: fit-content;
			padding: 1%;
			margin: 2vh auto;

			p {
				font-size: var(--font);
				padding: 0;
				margin: 5% 0;
				cursor: default;
			}
		}

		.hidden {
			display: none;
		}
	}
</style>
