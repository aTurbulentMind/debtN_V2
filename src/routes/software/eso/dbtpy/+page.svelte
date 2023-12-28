<script>
	let items = [
		{
			name: 'Credit Card Interface',
			text: 'The Credit Card Interface module allows you to instantly verify credit card information and take payments using a VISA or MasterCard. The module provides real-time authorization and credit line hold via your vendor. Credit cards can be used when posting transactions, or when setting up post-dated payments. Credit card information can also be securely stored for future payments.'
		},
		{
			name: 'Electronic Funds Transfer Interface',
			text: 'The Electronic Funds Transfer module allows collection agencies to receive electronic debtors payments, including pre-authorized electronic payments in place of postdated checks. I also allows an agency to redeposit returned checks assigned by a client. The module creates an interface file to export either to interface software to to an ACH vendor. The time and costs associated with collecting are reduced due to the reduction in bank processing time and minimized direct debtor contact reduces the time and cost associated with collecting.'
		},
		{
			name: 'PhoneCheck Module ',
			text: 'The PhoneCheck module allows users to create and print checks for debtors making payments over the phone, including postdated payments. By entering debtor banking information, account number, routing number and check number, users may print checks for that debtor payable to the agency. This speeds the collection process by allowing users to quickly process debtor payments without the hassle of mail lag times and delay.'
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
