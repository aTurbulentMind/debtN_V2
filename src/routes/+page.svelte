<script>
	import jumpPull from '$lib/assets/imgNum8.jpg';

	import Ribbon_Svg from '$lib/svg/ribbon_Svg.svelte';
	import Shield_Svg from '$lib/svg/shield_Svg.svelte';
	import MoneyHand_Svg from '$lib/svg/moneyHand_Svg.svelte';
	import Trophy_Svg from '$lib/svg/trophy_Svg.svelte';
	import Crown_Svg from '$lib/svg/crown_Svg.svelte';
	import Medal_Svg from '$lib/svg/medal_Svg.svelte';
</script>

<div class="hero">
	<div class="hero_Background" />
	<h1 class="glass_Back">DEBT$net</h1>
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
			Specialized knowledge and expertise in debt collection within specific industries..
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
		Our commitment to exceptional taste starts with the careful selection of natural, high-quality
		ingredients. We believe that great pizza begins with the finest elements, and that's why we
		source locally whenever possible. From the rich, vine-ripened tomatoes in our savory sauce to
		the premium, locally-sourced cheeses that blanket our dough, each ingredient is chosen with care
		and consideration.
	</p>

	<p class="text_Box">
		Our passion to natural goodness isn't just about taste; it's about providing you with a dining
		experience that is fresh, wholesome, and free from unnecessary additives. Every slice is a
		testament to our dedication to crafting pizzas that not only delight your taste buds but also
		nourish your body with the goodness that only natural ingredients can provide.
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

	.hero {
		display: flex;
		position: relative;
		background-image: url('$lib/assets/imgNum7.jpg');
		background-repeat: no-repeat;
		background-attachment: fixed;
		background-position: center;
		background-size: cover;
		z-index: 990;
		height: 100vh;
		width: 100vw;

		h1 {
			position: absolute;
			top: 10vh;
			left: 5vw;
			font-size: var(--f_lg);
			text-transform: uppercase;
		}

		p {
			position: absolute;
			top: 25vh;
			left: 5vw;
			width: 90vw;
			font-size: var(--font);
		}

		form {
			position: absolute;
			top: 45vh;
			left: 5vw;
			width: 90vw;
			height: 50vh;

			h2 {
				font-size: var(--f_m);
			}

			p {
				position: relative;
				top: 1vh;
				left: 0.01vw;
				margin-top: 4.5vh;
			}

			input {
				position: absolute;
				right: 7vw;
				width: 55vw;
				height: 3vh;
				font-size: var(--font);
				margin-top: 3vh;
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

	h1 {
		padding: 8vh 0 5vh 6vw;
		width: fit-content;
		position: flex;
		font-size: var(--f_lg);
	}

	.grid {
		grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
		gap: 15px;
		margin: 5vh 5vw;

		.card {
			margin: 5vh auto;
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
		background-color: var(--extra);
		color: var(--back_Main);
	}

	.overLay {
		margin-top: -100vh;

		a {
			font-size: var(--f_lg);
			margin-bottom: 20vh;
		}
	}

	@media only screen and (min-width: 740px) {
		h1 {
			padding: 18vh 0 5vh 46vw;
		}

		.hero {
			height: 110vh;
			h1 {
				position: absolute;
				left: 1vw;
				font-size: var(--f_xl);
			}

			p {
				top: 40vh;
				left: 1vw;
				margin: 0 3vw;
				font-size: var(--f_m);
			}

			a {
				left: 25vw;
				font-size: var(--f_lg);
			}
		}

		.grid {
			margin: 15vh auto;
			grid-template-rows: repeat(auto-fit, minmax(280px, 1fr));
			grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
			gap: 35px;

			svg {
				margin: 5% 35%;
			}
		}

		.alt_Color {
			margin: 1.5vh 0;
			height: 100vh;
			padding: 10vh 0;
		}
	}

	@media only screen and (min-width: 980px) {
		.hero {
			display: flex;
			height: 100vh;

			h1 {
				position: absolute;
				left: 10vw;
				font-size: var(--f_xxl);
			}

			p {
				position: absolute;
				left: 10vw;
				width: 40vw;
				font-size: var(--f_xl);
			}

			form {
				top: 40vh;
				margin-left: 50vw;
				width: 40vw;
				height: 55vh;

				h2 {
					font-size: var(--f_xl);
				}

				p {
					top: 4vh;
					margin-top: 3vh;
				}

				input {
					right: 5vw;
					width: 15vw;
					height: 4vh;
					margin-top: 0.5vh;
					font-size: var(--f_lg);
				}

				.text_Message {
					margin-top: -6vh;
				}

				button {
					width: 10vw;
					bottom: 5vh;
					left: 15vw;
					font-size: var(--f_xl);
				}
			}
		}

		.text_Block {
			height: 100vh;
			margin-bottom: 0;
		}

		.grid {
			margin: 15vh 10vw;

			.card {
				svg {
					margin: 3vh 35%;
				}

				.body {
					font-size: var(--f_m);
				}
			}
		}

		.overLay {
			display: relative;
			position: absolute;
			width: 40vw;
			right: 5vw;
			margin-top: -100vh;

			a {
				font-size: var(--f_xl);
			}
		}
	}

	@media only screen and (min-width: 1280px) {
		.hero {
			p {
				left: 5vw;
				width: 40vw;
				font-size: var(--f_xl);
			}
			form {
				height: 45vh;
				h2 {
					font-size: var(--f_lg);
				}

				p {
					font-size: var(--f_m);
				}

				input {
					font-size: var(--f_m);
				}

				button {
					font-size: var(--f_m);
				}
			}
		}

		.grid {
			margin: 10vh 10vw;

			.card {
				svg {
					margin: 1vh 35%;
				}

				.body {
					font-size: var(--f_m);
				}
			}
		}

		.text_Block {
			margin: 1.5vh 0vw;
		}

		.overLay {
			right: 1vw;
			margin-top: -95vh;

			p {
				font-size: var(--font);
			}

			a {
				font-size: var(--f_m);
			}
		}
	}
</style>
