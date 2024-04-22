<script>
	import jumpPull from '$lib/assets/Fall.jpg';
	import DNLogo from '$lib/assets/DebtNetclear.png';

	import Ribbon_Svg from '$lib/svg/ribbon_Svg.svelte';
	import Shield_Svg from '$lib/svg/shield_Svg.svelte';
	import MoneyHand_Svg from '$lib/svg/moneyHand_Svg.svelte';
	import Trophy_Svg from '$lib/svg/trophy_Svg.svelte';
	import Crown_Svg from '$lib/svg/crown_Svg.svelte';
	import Medal_Svg from '$lib/svg/medal_Svg.svelte';
</script>

<div class="hero">
	<div class="hero_Background" />
	<h1><img src={DNLogo} alt="" /></h1>
	<p class="glass_Back">
		"Empowering Financial Recovery for Over 45 years: Your Trusted Partner in Ethical Debt
		Collection. Navigate the Path to Financial Resilience with Us."
	</p>

	<form class="glass_Back">
		<h2>Request a demo</h2>
		<p>
			Your Company:
			<input type="text" placeholder="Best Company Ever" />
		</p>
		<p>
			Your Name:
			<input type="text" placeholder="Real Human Name" />
		</p>
		<p>
			Best way to reach you:
			<input type="text" placeholder="Contact Info" />
		</p>
		<p>Comment or questions:</p>
		<p>
			<input class="text_Message" type="textbox" placeholder="Words" />
		</p>

		<button>Submit</button>
	</form>
</div>

<h1>You matter to us!</h1>

<div class="grid">
	<div class="card">
		<h2 class="card-title">Proven Success Record:</h2>
		<svg><Ribbon_Svg /></svg>
		<br />
		<div class="body">Demonstrated track record of successful debt recovery.</div>
	</div>

	<div class="card">
		<h2 class="card-title">Compliance and Ethics:</h2>
		<svg><Shield_Svg /></svg>
		<br />
		<div class="body">
			Adherence to strict legal and ethical standards in debt collection practices.
		</div>
	</div>

	<div class="card">
		<h2 class="card-title">Industry Expertise:</h2>
		<svg><MoneyHand_Svg /></svg>
		<br />
		<div class="body">
			Specialized knowledge and expertise in debt collection within specific industries.
		</div>
	</div>

	<div class="card">
		<h2 class="card-title">Customized Solutions:</h2>
		<svg><Trophy_Svg /></svg>
		<br />
		<div class="body">Tailored debt recovery strategies to meet the unique needs of clients.</div>
	</div>

	<div class="card">
		<h2 class="card-title">Comprehensive Services:</h2>
		<svg><Crown_Svg /></svg>
		<br />
		<div class="body">
			Offering a full range of debt collection services to address various needs.
		</div>
	</div>

	<div class="card">
		<h2 class="card-title">Client-Centric Approach:</h2>
		<svg><Medal_Svg /></svg>
		<br />
		<div class="body">
			Placing clients' interests at the forefront with a customer-centric focus.
		</div>
	</div>
</div>

<div class="text_Block">
	<div class="img_Half">
		<img src={jumpPull} alt="background" />
	</div>

	<div class="text_Block overLay">
		<p class="text_Box glass_Back">
			Indulge in the extraordinary – why wait when a culinary delight is just a bite away?
			Fairgrounds Pizza beckons you to experience pizza perfection now. Picture yourself immersed in
			the heavenly blend of natural ingredients, the tantalizing aroma wafting from our ovens. Don't
			deny your taste buds this symphony of flavors, meticulously crafted to elevate your dining
			experience.
		</p>
		<p class="text_Box glass_Back">
			With every order, you're not just buying pizza – you're investing in a tradition that spans
			over five decades. Satisfy your cravings and order a slice of joy – because at Fairgrounds
			Pizza, every moment you delay is a moment you're missing out on the extraordinary.
		</p>

		<p class="text_Box">
			<a class="coa glass_Back" href="/">Call Now</a>
			<a class="coa glass_Back" style="margin-left: 10vw;" href="/software/"
				>Check out the software!</a
			>
		</p>
	</div>
</div>

<div class="text_Block alt_Color">
	<p class="text_Box">
		Founded in 1987 by principals Tony LaMagna and Gary Grout, the company has developed and
		provides the industry their premier core product, Debt$Net®, as well as supporting software
		modules, training, custom programming and technical support.
	</p>

	<p class="text_Box">
		Debt$Net®, created by The Computer Manager, Inc., has provided collection agencies, law firms,
		debt buyers and in-house collection departments with one of the most comprehensive debt
		collection systems in the industry. Proven in the field, Debt$Net® collection software has
		satisfied the debt recovery requirements for over 1,000 companies specializing in Retail,
		Commercial, Medical, Receivables Management and Check Collections. Debt$Net® users can be found
		throughout the United States and Canada.
	</p>

	<p class="text_Box">
		<a class=" glass_Back" href="/about/">Hear our story</a>
	</p>
</div>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	@use 'style/baseCamp';
	:global(*) {
		box-sizing: border-box;
	}
	//Phone
	.hero {
		display: flex;
		position: relative;
		background-image: url('$lib/assets/Mt.jpg');
		background-repeat: no-repeat;
		background-attachment: fixed;
		background-position: center;
		background-size: cover;
		z-index: 990;
		height: 100vh;
		width: 100vw;

		h1 {
			position: absolute;
			top: 0;
			left: 0;

			img {
				position: absolute;
				top: 3vh;
				left: 37vw;
				width: 50vw;
			}
		}

		p {
			position: absolute;
			top: 25vh;
			left: 5vw;
			width: 90vw;
			font-size: var(--f_m);
		}

		form {
			position: absolute;
			top: 45vh;
			left: 5vw;
			width: 90vw;
			height: 50vh;

			h2 {
				font-size: var(--f_m);
				margin: 0;
				margin-top: -10vh;
			}

			p {
				position: relative;
				top: -5vh;
				left: 0.01vw;
				margin-top: 4.25vh;
				padding: 0 5vw 0 0;
				text-align: left;
			}

			input {
				position: absolute;
				right: 7vw;
				width: 55vw;
				height: 3vh;
				font-size: var(--font);
				margin-top: 4vh;
			}

			.text_Message {
				margin-top: -3vh;
			}

			button {
				position: absolute;
				background: var(--highlight);
				width: fit-content;
				padding: 1%;
				bottom: 4vh;
				left: 35vw;
				font-size: var(--f_m);
				border-radius: var(--rad);
				font-weight: 700;

				&:hover {
					transition: all 0.3s ease-in-out;
					transform: scale(1.1);
					cursor: pointer;
					box-shadow: var(--box_Light);
				}
			}
		}
	}

	.grid {
		grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
		gap: var(--gap);
		margin: var(--full_blk);

		.card {
			margin: 5vh auto;

			svg {
				width: 15vw;
				margin: 1vh 40%;
			}
			.card-title {
				font-size: var(--f_m);
			}
		}
	}

	.text_Box {
		.coa {
			font-size: var(--f_m);
		}
	}

	.alt_Color {
		padding: 10vh 0;
	}

	.overLay {
		margin: -120vh 0 0 0;
		a {
			font-size: var(--f_lg);
			margin-bottom: 25vh;
		}
	}

	// Tablet
	@media only screen and (min-width: 426px) {
		.hero {
			height: 110vh;
			h1 {
				position: absolute;
				left: 1vw;
				font-size: var(--f_xl);
			}

			p {
				top: 25vh;
				left: 2vw;
				margin: 0 3vw;
				font-size: var(--f_m);
			}

			form {
				left: 5vw;
			}

			a {
				left: 25vw;
				font-size: var(--f_lg);
			}
		}

		.grid {
			margin: 10vh 2.5vw;
			grid-template-columns: 1fr 1fr;
			gap: 35px;

			.card {
				svg {
					width: 10vw;
					margin: 5% 35%;
				}
			}
		}

		.alt_Color {
			margin: 0;
			height: 115vh;
			padding: 10vh 0;
		}
	}

	// Laptop
	@media only screen and (min-width: 769px) {
		.hero {
			display: flex;
			height: 100vh;

			p {
				position: absolute;
				left: 27.5vw;
				top: 20vh;
				width: 40vw;
				font-size: var(--f_lg);
			}

			form {
				top: 50vh;
				margin-left: 10vw;
				width: 70vw;
				height: 50vh;

				h2 {
					font-size: var(--f_xl);
					margin: 0;
					margin-top: -10vh;
				}

				p {
					top: 0;
					margin-top: 3vh;
				}

				input {
					right: -15vw;
					width: 25vw;
					height: 4vh;
					margin-top: 0.5vh;
					font-size: var(--f_lg);
				}

				.text_Message {
					margin-top: -6vh;
				}

				button {
					width: 10vw;
					bottom: 3vh;
					left: 30vw;
					font-size: var(--f_lg);
				}
			}
		}

		.grid {
			margin: 15vh 10vw;

			.card {
				svg {
					width: 10vw;
					margin: 3vh 35%;
				}
			}
		}

		.text_Block {
			height: 60vh;
			margin-bottom: 0;

			.overLay {
				display: relative;
				position: absolute;
				width: 80vw;
				right: 10vw;
				margin-top: -160vh;

				p {
					margin-top: 3vh;
				}

				a {
					font-size: var(--f_xl);
				}
			}

			.img_Half {
				margin: 5vh 0;
				img {
					width: 100vw;
					margin-bottom: 5vh;
				}
			}
		}

		.alt_Color {
			color: var(--text_Main);
			background: var(--back_Main);
			margin-top: 120vh;
			margin-left: 10vw;
		}
	}

	//LgScrn
	@media only screen and (min-width: 1440px) {
		.hero {
			h1 {
				img {
					left: 0;
					padding: 0;
					margin: 0;
				}
			}

			p {
				top: 45vh;
				left: 4vw;
				width: 40vw;
				font-size: var(--f_xl);
			}
			form {
				top: 45vh;
				left: 40vw;
				width: 40vw;
				h2 {
					padding: 20% 20% 5% 5%;
					font-size: var(--f_lg);
				}

				p,
				input,
				button {
					font-size: var(--f_m);
				}

				input,
				button {
					left: 20vw;
					width: 15vw;
				}
			}
		}

		.grid {
			margin: 10vh 10vw;
			grid-template-columns: 1fr 1fr 1fr;

			.card {
				svg {
					width: 5vw;
					margin: 1vh 35%;
				}

				.body {
					font-size: var(--f_m);
				}
			}
		}

		.text_Block {
			margin: 1.5vh 0vw;

			.img_Half {
				margin: 5vh 0;
				img {
					width: 40vw;
					margin-bottom: 5vh;
				}
			}
			.overLay {
				right: 1vw;
				margin: -100vh 5vw 0 0;
				width: 50vw;

				p {
					font-size: var(--f_lg);
				}

				a {
					font-size: var(--f_m);
				}
			}
		}

		.alt_Color {
			color: var(--back_Main);
			background: var(--back_Alt);
			height: fit-content;
			margin-top: 60vh;
			margin-left: 0;
			margin-bottom: 0;

			.text_Box {
				margin: 10% 10% 0 10%;
			}
		}
	}
</style>
