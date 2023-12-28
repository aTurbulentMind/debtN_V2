<script>
	let items = [
		{
			name: 'Accurint® Interface',
			text: 'Accurint is a collection industry skip tracing service which maintains a comprehensive consumer database containing over 20 billion records compiled from more than 400 sources. At a minimum, these sources confirm existing records and offer multiple telephone, name and address records.'
		},
		{
			name: 'Acollaid Interface',
			text: 'LexisNexis LogoAcollaid is a collection industry skip tracing service which maintains a comprehensive consumer database containing over 120 million households, most with telephone and social security numbers. The Acollaid Module provides an interface between the Acollaid database and Debt$Net® . (To use this interface you must first be a subscriber with Acollaid.)'
		},
		{
			name: 'BANKO® Interface Module',
			text: 'LexisNexis LogoThe BANKO® Interface allows an agency access to bankruptcy cases and deceased debtor information.  This service consolidates and updates bankruptcy cases from all fifty states, the District of Columbia, and Puerto Rico daily, supplying timely, accurate, and complete bankruptcy information.'
		},
		{
			name: 'CBC Innovis Interface',
			text: 'The Debt$Net® CBC Innovis Interface allows agencies to forward debtor information to CBC Innovis, who then processes it using the RPC Solutions product tools. The return file includes updated phone and/or address information.'
		},
		{
			name: 'Consumer Credit Reports ',
			text: '  The Consumer Credit Reports option allows your agency to request, pull and print credit reports on debtors as well as view them from the debtor screens in Debt$Net®. This is done on-line with a modem by calling into a credit bureau such as Equifax, Experian, or TransUnion®. The credit report can then be downloaded, saved, reviewed, printed, and/or transferred into the Debt$Net® debtor screens. This module also provides an activity log to track and monitor administrative costs.'
		},
		{
			name: 'Debtor/Account Handling Debtor/Account handling',
			text: "eBureauDebt$Net®'s eBureau interface allows agencies to access two eBureau's tools, eScore and eLink. eLink and eScore is a service that helps accounts receivable management firms and departments locate, update and append information to a debtor record. eLink and eScore provides highly accurate phone number, addresses, bankruptcy information, deceased identification, assets, relatives, associates, neighbors and other vital information for work flow management. eLink and eScore is a service that enables rapid development and deployment of customized statistical scores."
		},
		{
			name: 'Experian® Collection Advantage',
			text: 'The Experian Collection Advantage Extended Service Option (ESO) provides you access to an Experian service.  Data from collection activity files is forwarded to Experian, and they calculate a score to indicate how “collectable” the debtor’s account(s) are. In addition, Experian will provide service members with additional information (e.g., updated address) via a return file. '
		},
		{
			name: 'Insight America Interface',
			text: "The Insight America Interface works with Acxiom Insight's Investigate product, a skip tracing tool that uses sophisticated data sets and customized analytics to find persons of interest."
		},
		{
			name: 'Lexis Nexis Batch Interface',
			text: 'LexisNexis LogoThe Lexis Nexis Batch Interface module receives daily updates from various sources such as telephone numbers, addresses, and emergence from bankruptcy directly from the source rather then from "self-importing" data. Lexis Nexis Batch is customized to work with the information and format you need.'
		},
		{
			name: 'Lexis Nexis Credit Attributes Interface',
			text: "LexisNexis LogoThis interface provides a comprehensive view of your portfolio and provides flexible options that allow you to select the credit attributes most relevant to your agency's work flow needs. Credit Attributes for Collections can help your agency prioritize collection activities by identifying the customers most likely to pay through credit history, such as summaries of derogatory trades and other indicators of liquidity, including information on open credit and the presence of mortgage trades."
		},
		{
			name: 'NCOA Interface',
			text: ' The NCOA module provides you the capability to process National Change of Address (NCOA) files. The files are created as part of the notice outsourcing process. Agencies which create notice files and forward them to outside vendors often receive back information on changed or incorrect addresses for debtors. The NCOA module will allow you to capture this information electronically.'
		},
		{
			name: 'SunGard’s AvantGard Predictive Metrics',
			text: '   SunGard’s AvantGard Predictive Metrics can help increase profits by enhancing debt recovery success and strategically target accounts for legal. Debt collectors can use statistical scoring models to help prioritize collection efforts and improve collection strategies.'
		},
		{
			name: 'TransUnion® CPE Module',
			text: 'The TransUnion® Collector’s Prioritization Engine (CPE) is a service offered by TransUnion® in which data from collection activity files is analyzed.  TransUnion® uses the data to calculate a score to indicate how “collectable” the debtor’s account(s) are.  In addition, TransUnion® will provide service members with additional information (updated address, tradeline data, and feedback from the debtor) from their data files. Debt$Net® can capture this data from TransUnion® and attach it to the appropriate debtor record.  The debtor score can be used select accounts and reassign them, or used with Debt$Net®’s own work scoring process and used to prioritize collector’s work activities. Additional data is captured in extended references for the debtor.'
		},
		{
			name: 'TransUnion® Collection Triggers',
			text: "The TransUnion®Collection Triggers Interface focuses on monitoring each consumer's credit file on a daily basis. TransUnion® will identify key changes to each consumer's credit file and contact information and compare those changes to a profile created for each customer. Your agency profile would consist of a selection of one or more trigger criteria, along with how often the triggered criteria should be returned to you."
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
		grid-template-columns: 1fr 1fr;
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
