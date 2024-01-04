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

<h2>Client Access</h2>

<ul class="add-ons">
	{#each items as item (item.name)}
		<li>
			<button
				class={selected === item.name ? 'selected' : 'unselected'}
				on:click={() => select(item.name)}
			>
				{item.name}
				<p class={selected === item.name ? '' : 'hidden'}>
					{item.text}
				</p>
			</button>
		</li>
	{/each}
</ul>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	.add-ons {
		grid-template-columns: 1fr;
	}
</style>
