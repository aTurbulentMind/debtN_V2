<script>
	let items = [
		{
			name: 'CT Center Interface',
			text: ' IATS LogoThe CT Center interface is a fully integrated, multi-faceted communication solution, providing predictive dialing, interactive communication, real-time host integration, skill-based routing and detailed reporting. CT Center from IAT allows your collectors to work larger volumes of calls with inbound and outbound call blending, in addition to keeping the debtors on the phone with speak hold and music on-hold messages. The CT Center system dials the debtor for the collector, only transferring successful connections directly to the collector.'
		},
		{
			name: 'Email Direct',
			text: 'The Email Direct module allows you to send email to clients and debtors from within Debt$Net®, without exiting to another email system. Emails can be sent to clients, prospects and users within your own agency. Reports can be emailed in one of two ways, direct from the report option screen or batched during routine operations.'
		},
		{
			name: 'Internet Dialing Interface',
			text: 'An agency can communicate with debtors quickly and easily with the Internet Dialing Interface. The Internet Dialing Interface will help expand your call volume and success rate by communicating with an unlimited number of debtors anywhere in the world through a messaging interface. Internet dialing sends personalized, automated phone messages to your debtors based on the accounts that you have selected from your active account list in Debt$Net®. Your messaging provider will respond with a return file, detailing the results of each debtor call. You may work the scheduled calls or run collection campaigns.'
		},
		{
			name: 'Notice Outsourcing Interface ',
			text: 'The Notice Outsourcing Interface module lets users export data generated from the Debt$Net® notice program to an outsourcing company specializing in printing notices for collection agencies. Agencies producing high volumes of notices may find that the Notice Outsourcing Interface greatly increases efficiency by eliminating time spent handling notices and by reducing postage and paper costs.'
		},
		{
			name: 'Predictive Dialing Interface ',
			text: 'IATS LogoThe Predictive Dialing Interface module allows agencies to utilize technology designed to increase collector productivity by providing a steady stream of available debtors while eliminating telephone dialing time and time spent talking to message takers or answering machines. A predictive dialing system coupled with the Predictive Dialing Interface module functions by dialing a list of debtors and passing available debtors to the collector. At the same time debtor identification information is transmitted to Debt$Net® so that the debtor automatically displays on the screen.'
		},
		{
			name: 'VoApps Interface',
			text: 'VoApps LogoSend VoApps a list of phone numbers and VoApps will deliver your voicemail displaying your caller ID. Upload and download of the information is integrated creating a seamless process. Live results and progress can be viewed in real-time on the VoApps user portal. As a result of delivering a voicemail, your collection agents will be thrilled to be answering an influx of inbound phone calls from debtors ready to make payments. Collect money while empowering consumers!'
		}
	];
	let selected = 'Full Trust Accounting';
	let select = (name) => (selected = name);
</script>

<h1>ESO's</h1>

<h2>Debtor Contact Enhancements</h2>

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
