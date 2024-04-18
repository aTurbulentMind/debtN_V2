<script>
	let items = [
		{
			name: 'Batch RCK Interface',
			text: ' The Batch RCK Interface module allows an agency to electronically redeposit NSF checks prior to normal collections on accounts. The process is done in batch form, which reduces data entry. The module creates an outgoing file which is sent to an Automated Clearing House service and receives the return file which automatically enters any transactions needed on successful checks. The cost of collections will be reduced with less contact and less paper being sent.'
		},
		{
			name: 'Check Verification',
			text: 'The Check Verification Module allows an agency to download the status of NSF check collection accounts into the check verification system. The module produces a file containing the new checks to be added to the verification system�s negative database, in addition to a list of paid checks to be deleted. The Check Verification Module supports a number of check verification vendors and provides you with a menu selection to create the download file. The Check Verification Module simplifies the maintenance of your verification system. As NSF accounts are placed or paid off, Debt$Net tracks and reports that information to the verification system.'
		},
		{
			name: 'Judgment Tracking Module',
			text: 'The Judgment Tracking module allows users to record judgment information and to indicate which accounts were included in the judgment. The module maintains records of original judgment amounts, including principal, interest and legal fees. Debt$Net® updates these fields as payments are posted to the appropriate accounts.'
		},
		{
			name: 'Legal Accounting Module ',
			text: 'The Legal Accounting module provides line item tracking of legal expenses incurred during the collection process. Users may track expenses incurred by the agency as well as those prepaid by the client and can instantly tell if a legal expense payment was received from a debtor and whether the client was reimbursed.'
		},
		{
			name: 'MICR Reader Module ',
			text: 'The MICR Reader module simplifies the input of NSF checks into Debt$Net®. The MICR Reader allows the check to be scanned during the account add process. Debt$Net® then checks existing debtors to find matches to the bank routing number and account number combination.'
		},
		{
			name: 'MICR Scanner Module',
			text: "The MICR Scanner module is the interface for a check scanner (MAGTEK MICR-scanner) with Debt$Net®. The scanner allows you to scan check information and store that information on the debtor's accounts. When this ESO is combined with the Document Imaging module, you can view the image of the check on the account screen, which can then be used in notices to your debtors."
		}
	];
	let selected = 'Full Trust Accounting';
	let select = (name) => (selected = name);
</script>

<h1>ESO's</h1>

<h2>Specialization</h2>

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
