<script>
	let activeTab = 'power'; // Set default active tab

	// Function to switch active tab
	function switchTab(tab) {
		activeTab = tab;
	}

	let items = [
		{
			name: 'Prest-Special Feature-4',
			text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit...'
		},
		{
			name: 'Prest-Special Feature-5',
			text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Suscipit eaque blanditiis nam libero assumenda quod!'
		},
		{
			name: 'Prest-Special Feature-6',
			text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Suscipit eaque blanditiis nam libero assumenda quod!'
		}
	];
	let selected = 'Prest-Special Feature-4';
	let select = (name) => (selected = name);
</script>

<h1>Software</h1>

<div class="text_Block">
	<p class="text_Box cut_Box">
		There are two Debt$Net® collection software products: Debt$Net® Prestige, a SQL client server
		system designed for mid to large sized agencies and Debt$Net® Power, designed to optimize
		business operations on a local area network.
	</p>
	<p class="text_Box cut_Box">
		Licenses for either product can be purchased outright or we also offer a month to month
		subscription program called Running Start. Our products are module, and you may even purchase a
		Venture, feature-block system if you don't require a full system. Add on modules called Extended
		Service Options allow you to expand the business features of the core product to accommodate
		agency needs such as skip tracing or letter outsourcing.
	</p>
	<p class="text_Box cut_Box">
		The sales quotes for a Debt$Net® system can offer cash, credit card, lease, subscription and
		contract terms. Typical sales quotes will include a base system, additional user licenses as
		required, add on modules, training, technical support and initial set-up. Data conversions, if
		necessary, may also be included.
	</p>
	<p class="text_Box cut_Box">
		Below are further descriptions of the product and purchasing options available, click to view
		information:
	</p>
</div>

<div class="tab-container">
	<!-- Power tab -->
	<div class="tab {activeTab === 'power' ? 'active' : ''}" on:click={() => switchTab('power')}>
		Power
	</div>

	<!-- Prestige tab -->
	<div
		class="tab {activeTab === 'prestige' ? 'active' : ''}"
		on:click={() => switchTab('prestige')}
	>
		Prestige
	</div>
</div>

<!-- Tab content -->
{#if activeTab === 'power'}
	<div class="tab-content">
		<h3>PowerS Info</h3>

		<div class="text_Block">
			<p class="text_Box cut_Box">
				Debt$Net® Power is also premise based and licensed on a per user basis. This version of the
				software is designed to optimize business operations on a local area network. Debt$Net®
				Power starts at $4,000.
			</p>
		</div>

		<h3>PowerS Special Features</h3>

		<div class="grid">
			<div class="card">
				<h2 class="card-title">Feature-1</h2>
				<br />
				<div class="body">
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium omnis laborum dicta
					aut voluptatibus molestias totam voluptate molestiae iusto distinctio quis expedita dolor
					nulla earum tenetur, temporibus, vitae fugiat dolorum pariatur? Vitae.
				</div>
			</div>

			<div class="card">
				<h2 class="card-title">Feature-2</h2>
				<br />
				<div class="body">
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis aspernatur porro enim
					aliquam expedita iste distinctio odit laudantium non minima, quos amet recusandae
					accusantium pariatur nisi sapiente temporibus?
				</div>
			</div>

			<div class="card">
				<h2 class="card-title">Feature-3</h2>
				<br />
				<div class="body">
					Lorem ipsum dolor sit amet consectetur, adipisicing elit. Facilis voluptatum nobis laborum
					odio aperiam facere blanditiis fuga fugit inventore consectetur ab assumenda corrupti
					maxime delectus vel beatae harum dolorem exercitationem ex, dicta, similique quisquam.
					Eligendi minima reiciendis eos.
				</div>
			</div>
		</div>
		<h3>Add-ons</h3>

		<a class="eso" href="/software/eso">Extended Service Options</a>

		<h3>PowerS System Reqs</h3>

		<!-- Server Requirements Table -->
		<table class="requirements-table">
			<caption>Power Server Requirements</caption>
			<thead>
				<tr>
					<th>Component</th>
					<th>Minimum</th>
					<th>Recommended</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>Windows Operating System</td>
					<td>Windows 7 or Higher</td>
					<td>Server 2008 or Higher</td>
				</tr>
				<tr>
					<td>Processor</td>
					<td>1GHz or Faster</td>
					<td>2GHz or Faster</td>
				</tr>
				<tr>
					<td>RAM</td>
					<td>8GB or Higher</td>
					<td>16GB or Higher</td>
				</tr>
				<tr>
					<td>Free HD Space</td>
					<td>20GB or More</td>
					<td>40GB or More</td>
				</tr>
			</tbody>
		</table>

		<!-- Workstation Requirements Table -->
		<table class="requirements-table">
			<caption>Power Workstation Requirements</caption>
			<thead>
				<tr>
					<th>Component</th>
					<th>Minimum</th>
					<th>Recommended</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>Windows Operating System</td>
					<td>Windows 7 or Higher</td>
					<td>Windows 7 or Higher</td>
				</tr>
				<tr>
					<td>Processor</td>
					<td>1.0 GHz or Faster</td>
					<td>2.0 GHz or Faster</td>
				</tr>
				<tr>
					<td>RAM</td>
					<td>2GB or Higher</td>
					<td>4GB or Higher</td>
				</tr>
				<tr>
					<td>Free HD Space</td>
					<td>1.5GB or More</td>
					<td>4GB or More</td>
				</tr>
			</tbody>
		</table>
	</div>
{/if}

{#if activeTab === 'prestige'}
	<div class="tab-content">
		<h3>Prestige 2023 Info</h3>

		<div class="text_Block">
			<p class="text_Box cut_Box">
				Debt$Net® Prestige is premise based and licensed on a per user basis. This award-winning
				collection software was developed with enterprise agencies in mind. It does require SQL
				server software and starts at $6,000.
			</p>
		</div>

		<h3>Prestige 2023 Special Features</h3>

		<ul class="add-ons">
			{#each items as item (item.name)}
				<li>
					<button
						class={selected === item.name ? 'selected' : ''}
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

		<h3>Prestige System Reqs</h3>

		<!-- Server Requirements Table -->
		<table class="requirements-table">
			<caption>Prestige Server Requirements</caption>
			<thead>
				<tr>
					<th>Component</th>
					<th>Minimum</th>
					<th>Recommended</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>Windows Operating System</td>
					<td>Windows 7 or Higher</td>
					<td>Server 2008 or Higher</td>
				</tr>
				<tr>
					<td>SQL Server</td>
					<td>2005 Standard or Newer</td>
					<td>2008 Standard or Newer</td>
				</tr>
				<tr>
					<td>Processor</td>
					<td>1GHz or Faster</td>
					<td>2GHz or Faster</td>
				</tr>
				<tr>
					<td>RAM</td>
					<td>8GB or Higher</td>
					<td>16GB or Higher</td>
				</tr>
				<tr>
					<td>Free HD Space</td>
					<td>20GB or More</td>
					<td>40GB or More</td>
				</tr>
			</tbody>
		</table>

		<!-- Workstation Requirements Table -->
		<table class="requirements-table">
			<caption>Prestige Workstation Requirements</caption>
			<thead>
				<tr>
					<th>Component</th>
					<th>Minimum</th>
					<th>Recommended</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>Windows Operating System</td>
					<td>Windows 7 or Higher</td>
					<td>Windows 7 or Higher</td>
				</tr>
				<tr>
					<td>Processor</td>
					<td>1.0 GHz or Faster</td>
					<td>2.0 GHz or Faster</td>
				</tr>
				<tr>
					<td>RAM</td>
					<td>2GB or Higher</td>
					<td>4GB or Higher</td>
				</tr>
				<tr>
					<td>Free HD Space</td>
					<td>2GB or More</td>
					<td>5GB or More</td>
				</tr>
			</tbody>
		</table>
	</div>
{/if}

<h3>Comparison</h3>

<table class="requirements-table compari">
	<thead>
		<tr>
			<th>Features</th>
			<th>PowerS</th>
			<th>Prestige23</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>this reason</td>
			<td
				><svg xmlns="http://www.w3.org/2000/svg" height="16" width="18" viewBox="0 0 576 512"
					><path
						d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"
					/></svg
				></td
			>
			<td
				><svg xmlns="http://www.w3.org/2000/svg" height="16" width="18" viewBox="0 0 576 512"
					><path
						d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"
					/></svg
				></td
			>
		</tr>
		<tr>
			<td>that reason</td>
			<td
				><svg xmlns="http://www.w3.org/2000/svg" height="16" width="18" viewBox="0 0 576 512"
					><path
						d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"
					/></svg
				></td
			>
			<td
				><svg xmlns="http://www.w3.org/2000/svg" height="16" width="18" viewBox="0 0 576 512"
					><path
						d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"
					/></svg
				></td
			>
		</tr>
		<tr>
			<td>another</td>
			<td></td>
			<td
				><svg xmlns="http://www.w3.org/2000/svg" height="16" width="18" viewBox="0 0 576 512"
					><path
						d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"
					/></svg
				></td
			>
		</tr>
		<tr>
			<td>And another</td>
			<td></td>
			<td
				><svg xmlns="http://www.w3.org/2000/svg" height="16" width="18" viewBox="0 0 576 512"
					><path
						d="M316.9 18C311.6 7 300.4 0 288.1 0s-23.4 7-28.8 18L195 150.3 51.4 171.5c-12 1.8-22 10.2-25.7 21.7s-.7 24.2 7.9 32.7L137.8 329 113.2 474.7c-2 12 3 24.2 12.9 31.3s23 8 33.8 2.3l128.3-68.5 128.3 68.5c10.8 5.7 23.9 4.9 33.8-2.3s14.9-19.3 12.9-31.3L438.5 329 542.7 225.9c8.6-8.5 11.7-21.2 7.9-32.7s-13.7-19.9-25.7-21.7L381.2 150.3 316.9 18z"
					/></svg
				></td
			>
		</tr>
	</tbody>
</table>

<h3>Other Products</h3>

<div class="text_Block">
	<p class="text_Box cut_Box">
		Debt$Net® Venture is the perfect product for both start-up agencies and existing agencies
		wishing to expand their operations. As a derivative product, Venture provides all the core
		functions of Debt$Net® required to jump-start your collection agency. Starting at $1,600,
		Debt$Net® Venture can also be built up to a fully powered Debt$Net® system as your company
		grows by adding in blocks of features.
	</p>
	<p class="text_Box cut_Box">
		Debt$Net® Running Start also offers the ability to subscribe to award-winning Debt$Net®
		collection software on a month-by-month basis. Running start will equip you with a fully
		functional, fully licensed copy of Debt$Net® for only $195 per month, allowing you to jumpstart
		your collections business while at the same time keeping overhead costs low.
	</p>
</div>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	//phone
	.tab-container {
		display: flex;
		justify-content: center; /* Center the tabs horizontally */
	}

	.tab {
		cursor: pointer;
		padding: 10px;
		border: var(--bord);
		border-radius: 5px 5px 0 0;
	}

	.tab.active {
		background-color: var(--text_Alt);
		border-bottom: 1px solid var(--text_Alt);
	}

	.tab-content {
		margin: 0 0 0 5vw;
		width: 90vw;
		border-radius: var(--rad);
		background-color: var(--text_Alt);

		p {
			margin-right: 0;
		}
	}

	.add-ons {
		width: 80vw;
		margin: 2vw 0;
	}

	.eso {
		padding: 10vh 0 5vh 6vw;
	}

	.requirements-table {
		width: 60vw;
		border-collapse: collapse;
		margin: 5vh 0 5vh 5vw;
		background: var(--back_Main);

		caption {
			font-weight: bold;
			text-align: center;
			padding: 10px;
			background-color: var(--text_Alt);
		}

		th,
		td {
			width: 20vw;
			border: 1px solid var(--text_Alt);
			padding: 3px;
		}

		th {
			background-color: var(--back_Alt);
			color: var(--back_Main);
		}

		td {
			padding: 0 5%;
			svg {
				margin: 0 0 0 5vw;
			}
		}

		tbody tr:nth-child(even) {
			background-color: var(--back_Alt);
			color: var(--back_Main);
		}
	}

	.compari {
		margin: 5vh auto;
	}

	@media only screen and (min-width: 426px) {
		.grid {
			grid-template-columns: repeat(auto-fit, minmax(420px, 1fr));
			grid-template-rows: repeat(auto-fit, minmax(220px, 1fr));
			width: 80vw;
			margin-left: 10vw;
		}

		.requirements-table {
			width: 60vw;
			margin: 10vh 20vw;
			border-collapse: collapse;

			caption {
				font-weight: bold;
				text-align: center;
				padding: 10px;
				background-color: var(--text_Alt);
			}

			th,
			td {
				border: 1px solid var(--text_Alt);
				padding: 8px 0;
			}

			th {
				color: var(--back_Main);
			}

			td {
				svg {
					margin: 0 5vw 0 10vw;
				}
			}

			tbody tr:nth-child(even) {
				background-color: var(--text_Alt);
				color: var(--text_Main);
			}
		}
	}

	@media only screen and (min-width: 769px) {
		.tab {
			cursor: pointer;
			padding: 10px;
			border: var(--bord);
			border-radius: 5px 5px 0 0;
		}

		.tab.active {
			background-color: var(--text_Alt);
			border-bottom: 1px solid var(--text_Alt);
		}

		.tab-content {
			margin: 0 0 0 7vw;
			width: 85vw;
			border-radius: var(--rad);
			background-color: var(--text_Alt);

			p {
				margin-right: 0;
			}

			.add-ons {
				grid-template-columns: 1fr;
				color: var(--text_Main);
				text-align: center;

				li,
				button {
					color: var(--text_Main);
					width: 40vw;
					background-color: transparent;
				}

				p {
					width: 37vw;
				}
			}
		}

		.grid {
			margin: 0 3vw;
		}

		.eso {
			margin-left: 20vw;
		}

		.requirements-table {
			width: 50vw;
			border-collapse: collapse;
			margin: 5vh 0 5vh 17vw;
			background: var(--back_Main);
		}
	}
</style>
