<script>
	import Phone_icon from '$lib/svg/phone_Svg.svelte';
	import Mail_Svg from '$lib/svg/mail_Svg.svelte';
	import Support_Svg from '$lib/svg/support_Svg.svelte';
	import Doc_Svg from '$lib/svg/doc_Svg.svelte';

	import Right_Eye from '$lib/assets/imgNum9.jpg';
</script>

<h1>About</h1>

<div class="text_Block">
	<p class="text_Box">
		Fairgrounds Pizza unfolds a remarkable five-decade tale, woven with passion, tradition, and a
		commitment to serving the community. In 1973, our founders, Maria and Tony, embarked on a
		culinary journey, transforming a modest corner into what would become the heart of the
		neighborhood. From the very beginning, their dedication to crafting exceptional pizzas and
		fostering a welcoming atmosphere laid the foundation for Fairgrounds Pizza's enduring legacy.
	</p>

	<p class="text_Box glass_Back">
		As the years unfolded, Fairgrounds Pizza became a cherished gathering place for families,
		friends, and pizza enthusiasts alike. The aroma of our freshly baked pies became synonymous with
		the warmth and camaraderie that filled the air. Through the ups and downs of the decades, the
		pizzeria evolved, adapting to changing tastes while staying true to its roots.
	</p>

	<p class="text_Box">
		In the midst of the Great Robot War of 1993, Fairgrounds Pizza stood resilient, a beacon of
		normalcy in tumultuous times. Despite the challenges posed by the robotic uprising, our
		dedicated team continued to roll out dough, spread sauce, and sprinkle toppings, offering a
		haven where the community could find solace and comfort. The pizzeria became a symbol of
		perseverance, turning each pizza into a testament of resilience and a slice of hope during those
		challenging days.
	</p>

	<div class="img_Gap">
		<img src={Right_Eye} alt="background" />
	</div>

	<p class="text_Box glass_Back">
		Throughout the fifty-year journey, Fairgrounds Pizza has been more than a place to enjoy
		delicious food; it's a living testament to the power of community and the enduring appeal of a
		slice of the past. From the original recipes passed down through generations to the smiling
		faces that have walked through our doors, each element contributes to the rich tapestry that is
		the story of Fairgrounds Pizza. As we celebrate this half-century milestone, we look back with
		gratitude for the memories shared, the challenges overcome, and the joy found in every
		pizza-loving moment.
	</p>

	<p class="text_Box">
		Today, as we continue our tradition of serving mouthwatering pizzas, Fairgrounds Pizza remains a
		cornerstone of the neighborhood, a place where families create new memories and friends come
		together over a shared love for exceptional pizza. Here's to the next fifty years of
		deliciousness, community, and the timeless joy of Fairgrounds Pizza.
	</p>

	<p class="text_Box glass_Back">
		Throughout the fifty-year journey, Fairgrounds Pizza has been more than a place to enjoy
		delicious food; it's a living testament to the power of community and the enduring appeal of a
		slice of the past. From the original recipes passed down through generations to the smiling
	</p>
</div>

<div id="affiliates" class="head_Line">
	<h3>Affiliates</h3>
</div>

<div class="grid">
	<div class="card">
		<svg><Phone_icon /></svg>
		<h2 class="card-title">Collection Comp 1</h2>
	</div>

	<div class="card">
		<svg><Mail_Svg /></svg>
		<h2 class="card-title">Collection Comp 2</h2>
	</div>

	<div class="card">
		<svg><Support_Svg /></svg>
		<h2 class="card-title">Collection Comp 3</h2>
	</div>

	<div class="card">
		<svg><Doc_Svg /></svg>
		<h2 class="card-title">Collection Comp 4</h2>
	</div>

	<div class="card">
		<svg><Phone_icon /></svg>
		<h2 class="card-title">Collection Comp 1</h2>
	</div>

	<div class="card">
		<svg><Mail_Svg /></svg>
		<h2 class="card-title">Collection Comp 2</h2>
	</div>

	<div class="card">
		<svg><Support_Svg /></svg>
		<h2 class="card-title">Collection Comp 3</h2>
	</div>

	<div class="card">
		<svg><Doc_Svg /></svg>
		<h2 class="card-title">Collection Comp 4</h2>
	</div>
</div>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	h1 {
		padding: 10vh 0 5vh 6vw;
		width: fit-content;
		position: flex;
		font-size: var(--f_lg);
	}

	h3 {
		padding: 10vh 0 5vh 15vw;
	}

	.img_Gap {
		img {
			width: 60%;
			margin: 0 20%;
		}
	}

	.grid {
		grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
		grid-template-rows: repeat(auto-fit, minmax(100px, 1fr));
		gap: 5px;
		border-radius: var(--rad);
		position: relative;
		margin-bottom: 20vh;

		.card {
			margin: 25px 10px;
			box-shadow: none;

			svg {
				width: 7vw;
				height: 7vh;
				margin: 1vh 10vw;

				text-align: center;
			}

			.card-title {
				font-size: var(--font);
				text-align: center;
			}
		}
	}

	@media only screen and (min-width: 980px) {
		h1 {
			padding: 18vh 0 5vh 46vw;
			width: fit-content;
			position: flex;
		}

		.grid {
			grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
			grid-template-rows: repeat(auto-fit, minmax(100px, 1fr));
			gap: var(--pad_xl);
			border: var(--bord);
			position: relative;
			margin-bottom: 20vh;

			.card {
				margin: 25px 20px;
				svg {
					width: 12vw;
					height: 7vh;
					margin: 1vh;
					align-items: center;
				}

				.card-title {
					font-size: var(--f_lg);
					text-align: center;
				}
			}
		}

		.head_Line {
			margin: 8vh 0 -13.7vh 45vw;
			background: var(--back_Main);
			z-index: 901;
			border-radius: var(--rad);
			border: var(--bord);
			width: fit-content;
			position: relative;

			h3 {
				padding: var(--pad);
				font-size: var(--f_lg);
			}
		}
	}
</style>
