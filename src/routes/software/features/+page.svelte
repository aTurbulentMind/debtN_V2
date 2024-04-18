<script>
	let items = [
		{
			name: 'Full Trust Accounting',
			text: 'Debt$Net maintains an up-to-date trust account. It handles debtor payments, adjustments, NSF reversals, client payments, set up fees, trust account adjustment, direct payments, forward commissions and direct payment invoices. You can even place a hold on debtor payments you suspect will not clear the bank so you do not pay your client prematurely.'
		},
		{
			name: 'Client Statement',
			text: ' Debt$Net® is flexible in the production of statements and the handling of your clients accounts. You can close the billing period and produce statements as often as you require. You can bill your clients as Net Remit or Gross Remit and control whether client balances carry forward or deduct balances from current collections. You can immediately invoice your clients for direct payments. You can easily adjust client accounts for payments received, corrections to invoices or trust account transactions.'
		},
		{
			name: 'Definable Client Commission Structures',
			text: ' Debt$Net® lets you create variable rate commission formulas to match how you do business with each of your clients. You can base your formulas on the account age, amount assigned, average monthly client volume, flat fee or payments received.'
		},
		{
			name: 'Unlimited Contact Notes',
			text: '  Debt$Net® provides unlimited contact notes. Collectors are allowed to add new notes, but not modify old entries. The administrative staff has unrestricted access to all contact notes. Stamping date, time and initials of the collector into the notes provides an audit trail when updating critical data such as status of the account and entering contact notes.'
		},
		{
			name: 'Automated Dunning Notices ',
			text: '  Debt$Net® lets you create more then twelve hundred notices of your own design. The content of a notice is totally free form, letting you set up any kind of notice you need and easily pull information from the Debt$Net® files into your notice. Besides the standard notice variable, you can calculate data and create your own variables, you can chain notices into a series and have multiple dunning notice series as well. Design one dunning series to accommodate medical collections and another for commercial or retail collections. As accounts are processed through the dunning series, you can automatically turn them over to a collector for a call. The dunning series can update the status, priority or collector assigned to the account. They can interrupt the notification sequence, restart, or redirect it at their discretion. Collectors can even print quick notices without interrupting the processing of the dunning series. Debt$Net® can also export notices to outsource companies.'
		},
		{
			name: 'Debtor/Account Handling Debtor/Account handling',
			text: '   Debt$Net® allows comprehensive tracking of debtors, multiple accounts per debtor, interest, check return fees, agency fees, legal fees, contact dates and much, much more. We proved debtor and account handling through the base working screen – a central work area that provides point and click access to all the information required to process and account from assignment to "paid in full."'
		},
		{
			name: 'Collector Contact Screens',
			text: '  We have optimized the collector contact screens for quick and efficient debtor contact. Collectors can contact debtors, set up payment plans, take incoming calls, help other collectors and schedule follow on actions. We have provided options to work a list of scheduled calls for today or a list of all the accounts assigned to them. The collector can work campaigns by ordering the list by balance, status, date last worked, client or priority. The contact screens provide instant access to information on the debtor, multiple accounts, payments, payment plans, contact notes, post dated checks, notice history, etc. The contact notes are unlimited in size. The contact deferral feature automatically reminds the collectors when it is time for a same day call back at a specific time. '
		},
		{
			name: 'Credit Bureau Reporting',
			text: '  Debt$Net® helps you in reporting to the credit bureaus electronically and allows you to receive and capture skip tracing information. You have complete control over reporting accounts on and off the bureau. You can also report business accounts, spouses and co-makers to the credit bureau.'
		},
		{
			name: 'Payment Plan Processing',
			text: "   Payment plans are easily set up with Debt$Net®'s promise system. Debt$Net® manages the plan and can automatically issue a delinquency letter or schedule a collector call if a payment is late. Collectors no longer have to keep tabs on their payment plans. They only have to handle the delinquencies."
		},
		{
			name: 'Payment Receipt Processing',
			text: "   Receive and account for debtor payments quickly and efficiently. Debt$Net®'s payment transaction processing is designed to minimize data entry requirements and record accurately against affected accounts. Use default setting to apply payments received against balances owed or manually apply payments as you wish. Track payment methods including cash, check, credit card or electronic funds transfer. Record direct payments to clients and Debt$Net® will update client statements appropriately."
		},
		{
			name: 'New Business Contact Management',
			text: '   Debt$Net® provides the contact management support your sales staff requires to maintain contact with potential clients. Schedule contact meetings and send contact letters from the notice system. When potential business contacts become active clients, Debt$Net® allows all the information on the client to be exported from the marketing file to the client file.'
		},
		{
			name: 'User-Definable Screens',
			text: '   Debt$Net® lets you create your own user-definable screens. These screens let you easily handle the special tracking requirements of your agency. You can also add new fields to the standard debtor and account screens.'
		},
		{
			name: 'Extended Debtor',
			text: "  Search Debt$Net®'s extended search tool will save you time trying to locate debtors and accounts in your system when only partial information is provided. The extended search solves the problem of how to apply a payment to a debtor when the name on the check doesn't match a debtor in your system. Search by name, phone number, client information, account information or other fields. Debt$Net® will display all records which match the information you have provided, letting you make the final selection."
		},
		{
			name: ' State and Agency Contact Restrictions',
			text: '  State and agency restrictions let system users know about legal issues or when special account handling is required. Restrictions can stop mailing to the debtor and provide on-screen warning and instructions to collectors. Use state restrictions for issues such as licensing in a state. Create agency restrictions to manage special handling cases.'
		},
		{
			name: 'Password and Menu Level Security',
			text: '  Debt$Net® lets you control user access to sensitive business information. Debt$Net® is not only password protected, but allows you to specify who can access each menu of the program. Collectors can be kept from financial and client screens and even limited from updating some fields of debtor information such as name and social security number.'
		},
		{
			name: 'Post Dated Check Management',
			text: '  Post Dated Check Management Capture Post Dated Check information and let Debt$Net® keep track of payment processing. Debt$Net® allows you to design and send pre-deposit notices, review post dated checks on file and automatically deposit them at the scheduled time.'
		},
		{
			name: 'Check Printing ',
			text: '  Debt$Net® lets you layout and print client remittance checks to accommodate your style of checks.'
		},
		{
			name: 'Client Reporting',
			text: '  Client Reporting Debt$Net® provides numerous reports to support the management of your clients. These include: Client Activity and Status Reports, Client Acknowledgments, Multiple Month Recovery Report, Client Cancel and Return Report and Trust Summary.'
		},
		{
			name: 'Debtor Statements and Payment Coupons',
			text: '   Prepare and send debtor statements and payment coupon books to remind debtors of payment obligations. Debtor statements are a unique notice type showing debtor balances owed on their account(s). Debtor statements can be produced monthly or as required, independent of notice processing or other scheduled actions. Payment coupon books can be created by collectors when payment plans are set up.'
		},
		{
			name: 'Collector Productivity Tracking ',
			text: '  Debt$Net® helps you monitor collector productivity and performance. It tracks commissions, collector activity, contact frequency, contact type as well as the number of accounts collected, amount collected month-to-date and year-to-date activity.'
		}
	];
	let selected = 'Full Trust Accounting';
	let select = (name) => (selected = name);
</script>

<h1>Features</h1>

<div class="text_Block">
	<p class="text_Box">
		Debt$Net® offers all the features, flexibility and sophistication of mainframe packages at an
		affordable price. Click a selection below to expand and see just some of the many features
		Debt$Net® offers
	</p>
</div>

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

	.add-ons {
		li,
		button,
		p {
			cursor: pointer;
		}
	}

	@media (min-width: 426px) {
	}

	@media (min-width: 769px) {
		.add-ons {
			grid-template-columns: 1fr 1fr;

			button,
			p {
				width: 35vw;
			}

			p {
				padding: 1%;
			}
		}

		.text_Box {
			margin-left: 5vw;
		}
	}
</style>
