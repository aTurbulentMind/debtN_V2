<script>
	import Left_Eye from '$lib/assets/imgNum2.jpg';
	import Right_Eye from '$lib/assets/imgNum9.jpg';

	let focused = ' ';
	let focusElement = (id) => (focused = id);

	let pwritems = [
		{ pwrName: 'pwr-addon-1', text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit...' },
		{
			pwrName: 'pwr-addon-2',
			text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Suscipit eaque blanditiis nam libero assumenda quod!'
		},
		{
			pwrName: 'pwr-addon-3',
			text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Suscipit eaque blanditiis nam libero assumenda quod!'
		}
	];
	let pwrSelected = 'pwr-addon-1';
	let pwrSelect = (pwrName) => (pwrSelected = pwrName);

	let items = [
		{ name: 'Prest-addon-4', text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit...' },
		{
			name: 'Prest-addon-5',
			text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Suscipit eaque blanditiis nam libero assumenda quod!'
		},
		{
			name: 'Prest-addon-6',
			text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Suscipit eaque blanditiis nam libero assumenda quod!'
		}
	];
	let selected = 'Prest-addon-4';
	let select = (name) => (selected = name);
</script>

<h1>Software</h1>

<div class="text_Block">
	<p class="text_Box">
		There are two Debt$Net® collection software products: Debt$Net® Prestige, a SQL client server
		system designed for mid to large sized agencies and Debt$Net® Power, designed to optimize
		business operations on a local area network.
	</p>
	<p class="text_Box">
		Licenses for either product can be purchased outright or we also offer a month to month
		subscription program called Running Start. Our products are module, and you may even purchase a
		Venture, feature-block system if you don't require a full system. Add on modules called Extended
		Service Options allow you to expand the business features of the core product to accommodate
		agency needs such as skip tracing or letter outsourcing.
	</p>
	<p class="text_Box">
		The sales quotes for a Debt$Net® system can offer cash, credit card, lease, subscription and
		contract terms. Typical sales quotes will include a base system, additional user licenses as
		required, add on modules, training, technical support and initial set-up. Data conversions, if
		necessary, may also be included.
	</p>
	<p class="text_Box">
		Below are further descriptions of the product and purchasing options available:
	</p>
</div>

<div class="img_container">
	<button
		class={focused === 'img_Left' ? 'focused' : 'unfocused'}
		on:click={() => focusElement('img_Left')}
	>
		<img src={Left_Eye} alt="money graph" />
		<p>
			PowerS
			<br /> <br />
			Debt$Net® Power, the flagship product from Debt$Net® Collection Software, has served collection
			agencies for over 20 years. Now enhanced with more features, it provides a high-performance local
			area network system with cost-effective, modular design. Delivering unmatched value, it ensures
			business success with low start-up and maintenance costs. Explore Debt$Net® Power's comprehensive
			features for a closer look at its capabilities.
		</p>
	</button>

	<button
		class={focused === 'img_Right' ? 'focused' : 'unfocused'}
		on:click={() => focusElement('img_Right')}
	>
		<img src={Right_Eye} alt="background" />
		<p>
			Prestige 2023
			<br /> <br />
			Debt$Net® Prestige, the latest from Debt$Net® Collection Software, is a powerful SQL-based solution
			designed for mid-sized to large agencies. Offering flexibility, business features, and robust security,
			Prestige ensures unparalleled data integrity. With modular design and two decades of expertise,
			it maximizes efficiency, guaranteeing production, profit, and top value.
		</p>
	</button>
</div>

{#if focused === 'img_Left'}
	<h3>PowerS Features</h3>

	<div class="grid">
		<div class="card">
			<h2 class="card-title">Michael L</h2>
			<br />
			<div class="body">
				I go here relatively often, and I'm always impressed. They have a great $6 deal, and their
				pizzas are incredibly delicious. They always make sure to put a lot of toppings on, and the
				prices are not bad for what you get. It's a relatively informal establishment, but I think
				that adds to the charm. 10/10 pizza place.
			</div>
		</div>

		<div class="card">
			<h2 class="card-title">Michael R</h2>
			<br />
			<div class="body">
				We discovered this place last month, and we only get pizza from here now. The pizza is at a
				better price than most chain pizza places, and the quality is better as well. I really like
				that they have pizza sizes for all occasions to include a huge party size pizza. Update: You
				don't need to know anything except this. I found this place a month ago, and now I refuse to
				get pizza anywhere else. Price = Amazing Quality = Better than amazing
			</div>
		</div>

		<div class="card">
			<h2 class="card-title">Jenny</h2>
			<br />
			<div class="body">
				We where first timers the other night. I ordered the Veggie lovers and the chicken, bacon,
				ranch. Man these pizzas where so good, zero complaints, they where loaded. The service was
				great and everything was done correctly. Look forward to trying more of your menu.
				Recommend!
			</div>
		</div>

		<div class="card glass_Back">
			<h2 class="card-title">Larry</h2>
			<br />
			<div class="body">
				Fairgrounds Pizza is amazing! I've tried a couple different kinds of there pizza but I
				definitely recommend the Works! Toppings are great and so is the crust (which is a rare
				combination) Currently my favorite local pizza place! Staff is courteous and professional!
			</div>
		</div>

		<div class="card glass_Back">
			<h2 class="card-title">Anna</h2>
			<br />
			<div class="body">
				Great pizza! We were looking for traditional, affordable, cravable pizza (which we have
				found surprisingly hard to find since we moved here) and definitely found it at Fairgrounds.
				Delicious crust and cooked to perfect golden crispness 😋 Breadsticks are wonderful too! The
				gentleman working last Saturday 2/4 was very accommodating and provided great customer
				service too.
			</div>
		</div>

		<div class="card glass_Back">
			<h2 class="card-title">Noel</h2>
			<br />
			<div class="body">
				THE BEST PIZZA IN KITSAP COUNTY!!! The cheese was perfect. The marinara was deculate. The
				crust was nice and crisp. This will be the only pizza i'll ever order from now on. They have
				made me see the light!!
			</div>
		</div>
	</div>

	<h3>PowerS Info</h3>

	<div class="text_Block">
		<p class="text_Box">
			Debt$Net® Power is also premise based and licensed on a per user basis. This version of the
			software is designed to optimize business operations on a local area network. Debt$Net® Power
			starts at $4,000.
		</p>
	</div>

	<h3>PowerS Add-ons</h3>

	<ul class="add-ons">
		{#each pwritems as pwrItem (pwrItem.pwrName)}
			<li
				class={pwrSelected === pwrItem.pwrName ? 'pwrSelected' : ''}
				on:click={() => pwrSelect(pwrItem.pwrName)}
			>
				{pwrItem.pwrName}
				<p class={pwrSelected === pwrItem.pwrName ? '' : 'hidden'}>
					{pwrItem.text}
				</p>
			</li>
		{/each}
	</ul>

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
{/if}

{#if focused === 'img_Right'}
	<h3>Prestige 2023 Features</h3>
	<div class="grid">
		<div class="card glass_Back">
			<h2 class="card-title">Noel</h2>
			<br />
			<div class="body">
				THE BEST PIZZA IN KITSAP COUNTY!!! The cheese was perfect. The marinara was deculate. The
				crust was nice and crisp. This will be the only pizza i'll ever order from now on. They have
				made me see the light!!
			</div>
		</div>

		<div class="card glass_Back">
			<h2 class="card-title">Larry</h2>
			<br />
			<div class="body">
				Fairgrounds Pizza is amazing! I've tried a couple different kinds of there pizza but I
				definitely recommend the Works! Toppings are great and so is the crust (which is a rare
				combination) Currently my favorite local pizza place! Staff is courteous and professional!
			</div>
		</div>

		<div class="card glass_Back">
			<h2 class="card-title">Anna</h2>
			<br />
			<div class="body">
				Great pizza! We were looking for traditional, affordable, cravable pizza (which we have
				found surprisingly hard to find since we moved here) and definitely found it at Fairgrounds.
				Delicious crust and cooked to perfect golden crispness 😋 Breadsticks are wonderful too! The
				gentleman working last Saturday 2/4 was very accommodating and provided great customer
				service too.
			</div>
		</div>

		<div class="card">
			<h2 class="card-title">Michael R</h2>
			<br />
			<div class="body">
				We discovered this place last month, and we only get pizza from here now. The pizza is at a
				better price than most chain pizza places, and the quality is better as well. I really like
				that they have pizza sizes for all occasions to include a huge party size pizza. Update: You
				don't need to know anything except this. I found this place a month ago, and now I refuse to
				get pizza anywhere else. Price = Amazing Quality = Better than amazing
			</div>
		</div>

		<div class="card">
			<h2 class="card-title">Jenny</h2>
			<br />
			<div class="body">
				We where first timers the other night. I ordered the Veggie lovers and the chicken, bacon,
				ranch. Man these pizzas where so good, zero complaints, they where loaded. The service was
				great and everything was done correctly. Look forward to trying more of your menu.
				Recommend!
			</div>
		</div>

		<div class="card">
			<h2 class="card-title">Michael L</h2>
			<br />
			<div class="body">
				I go here relatively often, and I'm always impressed. They have a great $6 deal, and their
				pizzas are incredibly delicious. They always make sure to put a lot of toppings on, and the
				prices are not bad for what you get. It's a relatively informal establishment, but I think
				that adds to the charm. 10/10 pizza place.
			</div>
		</div>
	</div>

	<h3>Prestige 2023 Info</h3>

	<div class="text_Block">
		<p class="text_Box">
			Debt$Net® Prestige is premise based and licensed on a per user basis. This award-winning
			collection software was developed with enterprise agencies in mind. It does require SQL server
			software and starts at $6,000.
		</p>
	</div>

	<h3>Prestige 2023 Add-ons</h3>

	<ul class="add-ons">
		{#each items as item (item.name)}
			<li class={selected === item.name ? 'selected' : ''} on:click={() => select(item.name)}>
				{item.name}
				<p class={selected === item.name ? '' : 'hidden'}>
					{item.text}
				</p>
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
{/if}

<div class="img_container">
	<button
		class={focused === 'img_Left' ? 'focused' : 'unfocused'}
		on:click={() => focusElement('img_Left')}
	>
		<h2>PowerS</h2>
	</button>

	<button
		class={focused === 'img_Right' ? 'focused' : 'unfocused'}
		on:click={() => focusElement('img_Right')}
	>
		<h2>Prestige23</h2>
	</button>
</div>

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
	<p class="text_Box">
		Debt$Net® Venture is the perfect product for both start-up agencies and existing agencies
		wishing to expand their operations. As a derivative product, Venture provides all the core
		functions of Debt$Net® required to jump-start your collection agency. Starting at $1,600,
		Debt$Net® Venture can also be built up to a fully powered Debt$Net® system as your company
		grows by adding in blocks of features.
	</p>
	<p class="text_Box">
		Debt$Net® Running Start also offers the ability to subscribe to award-winning Debt$Net®
		collection software on a month-by-month basis. Running start will equip you with a fully
		functional, fully licensed copy of Debt$Net® for only $195 per month, allowing you to jumpstart
		your collections business while at the same time keeping overhead costs low.
	</p>
</div>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	h1,
	h3 {
		width: fit-content;
		position: flex;
		padding: 10vh 0 10vh 15vw;
	}

	.img_container {
		display: relative;
		justify-content: space-around;
		margin: 1vh 2.5vw;

		.img_Left,
		.img_Right {
			transition: all 0.5s ease;
		}

		button {
			border-radius: var(--rad);
			cursor: pointer;

			img {
				width: 60vw;
			}

			p {
				font-size: var(--f_m);
				margin-top: 0;
			}
		}

		.focused {
			background: var(--back_Alt);
			color: var(--back_Main);
			transform: scale(1);
		}

		.unfocused {
			transform: scale(0.6);
			background-color: var(--back_Tre);
			color: var(--back_Main);
			margin: 5vh 15vw;

			p,
			.text_Box {
				display: none;
			}
		}

		p {
			padding: 3%;
		}
	}

	.add-ons {
		list-style-type: none;
		width: 90vw;
		margin: 2vw 5vw;

		.pwrSelected,
		.selected {
			border: var(--bord);
			border-radius: var(--rad);
			background-color: var(--back_Alt);
			color: var(--back_Main);
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
				padding: 2%;
				margin: 0 5vw;
				cursor: default;
			}
		}

		.hidden {
			display: none;
		}
	}

	.requirements-table {
		width: 50vw;
		border-collapse: collapse;
		margin: 5vh 0;

		caption {
			font-weight: bold;
			text-align: center;
			padding: 10px;
			background-color: var(--text_Alt);
		}

		th,
		td {
			border: 1px solid var(--text_Alt);
			padding: 8px;
		}

		th {
			background-color: var(--back_Alt);
			color: var(--back_Main);
		}

		td {
			svg {
				margin: 0 5vw 0 10vw;
			}
		}

		tbody tr:nth-child(even) {
			background-color: var(--text_Alt);
		}
	}

	.compari {
		margin: 5vh auto;
	}

	@media only screen and (min-width: 980px) {
		h1,
		h3 {
			width: fit-content;
			position: flex;
			padding: 18vh 0 5vh 46vw;
		}

		.img_container {
			margin: 0 15vw;
			display: flex;
			justify-content: space-around;

			.img_Left,
			.img_Right {
				transition: all 0.5s ease;
			}

			button {
				border-radius: var(--rad);
				cursor: pointer;
				h2 {
					padding: var(--pad);
				}

				img {
					width: 30vw;
				}

				p {
					font-size: var(--f_m);
					margin-top: 0;
				}
			}

			.focused {
				background: var(--back_Alt);
				color: var(--back_Main);
				transform: scale(1);
				margin: 0 10vw;
			}

			.unfocused {
				transform: scale(0.6);
				background-color: var(--back_Tre);
				color: var(--back_Main);
				margin: 0 5vw;

				p,
				.text_Box {
					display: none;
				}
			}
			p {
				padding: 3%;
			}
		}

		.add-ons {
			margin: 20vh 25vw;
			list-style-type: none;
			width: 50vw;

			.pwrSelected,
			.selected {
				border: var(--bord);
				border-radius: var(--rad);
				background-color: var(--back_Alt);
				color: var(--back_Main);
			}

			li {
				font-size: var(--f_lg);
				padding: 1%;
				margin: 2vh 0;
				background-color: var(--highlight);
				border: var(--bord);
				border-radius: var(--rad);
				cursor: pointer;
				width: fit-content;

				p {
					font-size: var(--f_m);
					padding: 2%;
					margin: 0 8vw;
					cursor: default;
				}
			}

			.hidden {
				display: none;
			}
		}

		.grid {
			grid-template-columns: repeat(auto-fit, minmax(420px, 1fr));
			grid-template-rows: repeat(auto-fit, minmax(220px, 1fr));
		}

		.sys_Reqs img {
			width: 40vw;
			margin: 0 30vw 5vh;
		}

		.requirements-table {
			width: 50vw;
			margin: 10vh 25vw;
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
				padding: 8px;
			}

			th {
				background-color: var(--back_Alt);
				color: var(--back_Main);
			}

			td {
				svg {
					margin: 0 5vw 0 10vw;
				}
			}

			tbody tr:nth-child(even) {
				background-color: var(--text_Alt);
			}
		}
	}
</style>
