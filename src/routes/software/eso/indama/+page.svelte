<script>
	let items = [
		{
			name: 'Client Upload/Client Input',
			text: ' The Client Upload/Input Module allows for electronic loading of debtors and accounts into Debt$Net® with various file formats. The Client Input portion of the module gives your clients an interface which allows them to easily provide you with a file on diskette or via modem which contains their debtor/account information. Client Upload is then used to read the files and create debtor and account records in Debt$Net®.'
		},
		{
			name: 'CMS 1500 Medical Form Interface',
			text: 'The CMS 1500 Medical Form Interface module allows users to enter debtor information on the CMS 1500 insurance claim form and print the form from Debt$Net®. Once completed, the form may be submitted to the appropriate insurance company.'
		},
		{
			name: 'Collector Monitor Module',
			text: 'The Collector Monitor module assists users in supervising collector productivity. The Collector Monitor module allows users to produce reports documenting collector performance statistics and view the current activities of designated collectors while they work in Debt$Net®. These features facilitate collector supervision and training and lets users analyze collector productivity and accountability.'
		},
		{
			name: 'Document Imaging Module',
			text: 'The Document Imaging Modulee lets users scan images (such as letterhead logos, NSF checks, etc.) directly into Debt$Net®. The scanned images are saved in the debtor, account, client, or contact manager files, where they may be accessed through Debt$Net® as needed.'
		},
		{
			name: 'FoxFire! Report Writer Interface',
			text: 'The FoxFire! Report Writer Interface module provides users with the tools to create and customize their own reports. Satisfy special client reporting requirements by using FoxFire! to filter out data items and to sort or group specified debtor, account, client and transaction information.'
		},
		{
			name: 'TriVium Call Recording Interface',
			text: "Established in 1996, TriVium Systems is a leading provider of call recording and reporting applications for the account receivables marketplace. We serve hundreds of collection agencies and law firm customers and are affiliated with the industry's leading associations including ACA, NARCA and DBA. www.collections-callrecording.com"
		},
		{
			name: 'UB04 Medical Form Interface',
			text: 'The UB04 Medical Form Interface module allows you to enter debtor information on the UB04 health insurance claim form and to print the form directly from Debt$Net®. Once completed, the form may be submitted to the appropriate insurance company.'
		}
	];
	let selected = 'Full Trust Accounting';
	let select = (name) => (selected = name);
</script>

<h1>ESO's</h1>

<h2>Information & Data Management</h2>

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
