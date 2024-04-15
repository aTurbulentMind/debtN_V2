<script>
	import Phone_icon from '$lib/svg/phone_Svg.svelte';
	import Mail_Svg from '$lib/svg/mail_Svg.svelte';
	import Support_Svg from '$lib/svg/support_Svg.svelte';
	import Doc_Svg from '$lib/svg/doc_Svg.svelte';
</script>

<h4>Hello :)</h4>

<div class="head_Line">
	<h1>CONTACT</h1>
</div>

<div class="grid">
	<div class="card">
		<h2 class="card-title">Call</h2>
		<svg><Phone_icon /></svg>
		<br />
		<div class="body">
			Swift solutions at your fingertips. Call now for expert assistance in resolving your financial
			concerns.
			<br />
			Toll Free: <a href="/"> 1-800-552-8397</a>
			<br />
			Fax: <a href="/">1-253-204-2349</a>
		</div>
	</div>

	<div class="card">
		<h2 class="card-title">Email</h2>
		<svg><Mail_Svg /></svg>
		<br />
		<div class="body">
			Reach out effortlessly. Send us an email to start the conversation about your debt management
			needs to <a href="/">info@debtnet5.com</a>
		</div>
	</div>

	<div class="card">
		<h2 class="card-title">Support</h2>
		<svg><Support_Svg /></svg>
		<br />
		<div class="body">
			Dedicated support team ready to guide you. Our experts are here to assist you every step of
			the way.
			<br />
			Toll Free: <a href="/"> 1-800-552-8397</a>
		</div>
	</div>

	<div class="card">
		<svg><Doc_Svg /></svg>
		<h2 class="card-title">Documentation</h2>
		<br />
		<div class="body">
			Access comprehensive resources. Explore our documentation for valuable insights on debt
			management and financial recovery.
		</div>
	</div>
</div>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	.grid {
		border: var(--bord);
		.card {
			box-shadow: none;
			svg {
				width: 20%;
				margin: -50px 40%;
			}

			.card-title {
				font-size: var(--font);
			}

			.body {
				font-size: var(--f_sm);
			}
		}
	}

	.head_Line {
		background: var(--back_Main);
		z-index: 901;
		margin: 8vh auto;
		font-size: var(--f_sm);
		border-radius: var(--rad);
		border: var(--bord);
		padding: var(--pad);
		width: fit-content;
		position: relative;

		h1 {
			padding: 0;
		}
	}

	@media only screen and (min-width: 980px) {
		.grid {
			grid-template-columns: repeat(auto-fit, minmax(620px, 1fr));
			grid-template-rows: repeat(auto-fit, minmax(420px, 1fr));
			gap: var(--pad_xl);
			position: relative;
			margin-bottom: 6.9vh;

			.card {
				svg {
					width: 12vw;
					height: 7vh;
					margin: 2vh 10vw;
				}

				.card-title {
					font-size: var(--f_lg);
					margin: var(--marg);
				}

				.body {
					font-size: var(--f_m);
				}
			}
		}

		.head_Line {
			margin: 8vh 0 -13.7vh 45vw;
			h1 {
				padding: 0;
				width: fit-content;
			}
		}
	}
</style>
