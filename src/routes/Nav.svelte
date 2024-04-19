<script>
	import Dollar_Svg from '../lib/svg/money_Svg.svelte';

	import DNLogo from '$lib/assets/DebtNetclear.png';
	let isMenuOpen = false;

	function toggleMenu() {
		isMenuOpen = !isMenuOpen;
	}

	let current = 0;
</script>

<div class="navbar">
	<a href="/" class="logo"><img src={DNLogo} alt="" /></a>
	<nav class:open={isMenuOpen}>
		<!--this is the main navigation menu-->
		<ul>
			<li>
				<button on:click={() => (isMenuOpen = false)} on:keydown={() => (isMenuOpen = false)}>
					<a class:current={current === 0} on:click={() => (current = 0)} href="/software/"
						>Software</a
					>
				</button>
			</li>
			<li>
				<button on:click={() => (isMenuOpen = false)} on:keydown={() => (isMenuOpen = false)}>
					<a class:current={current === 1} on:click={() => (current = 1)} href="/reviews/"
						>Reviews</a
					>
				</button>
			</li>
			<li>
				<button on:click={() => (isMenuOpen = false)} on:keydown={() => (isMenuOpen = false)}>
					<a class:current={current === 2} on:click={() => (current = 2)} href="/Contact/"
						>Contact</a
					>
				</button>
			</li>
			<li>
				<button on:click={() => (isMenuOpen = false)} on:keydown={() => (isMenuOpen = false)}>
					<a class:current={current === 3} on:click={() => (current = 3)} href="/about/">About</a>
				</button>
			</li>
			<li>
				<button on:click={() => (isMenuOpen = false)} on:keydown={() => (isMenuOpen = false)}>
					<a class:current={current === 4} on:click={() => (current = 4)} href="/services"
						>Services</a
					>
				</button>
			</li>
			<li>
				<button on:click={() => (isMenuOpen = false)} on:keydown={() => (isMenuOpen = false)}>
					<a class:current={current === 5} on:click={() => (current = 5)} href="/">Home</a>
				</button>
			</li>
		</ul>
	</nav>
	<button on:click={toggleMenu} on:keydown={() => (isMenuOpen = false)}>
		<div class="burger">
			<svg> <Dollar_Svg /></svg>
		</div>
	</button>
</div>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	:global(*) {
		box-sizing: border-box;
	}

	//phone
	nav {
		display: none;
	}

	nav.open {
		display: block;
		position: absolute;
		top: 100%;
		left: 0;
		background-color: var(--extra);
		width: 100%;
	}

	.navbar {
		button {
			all: unset;
		}

		background-color: var(--back_Alt);
		width: 100vw;
		display: flex;
		justify-content: space-between;
		position: fixed;
		height: 5rem;
		z-index: 950;
		box-shadow: var(--box_Shadow);
		transition: transform 0.2s ease-in-out;

		.logo {
			img {
				width: 30vw;
				padding: 1%;
				margin: 5%;
				background-color: var(--back_Main);
				border-radius: var(--rad);
			}
		}

		a,
		select {
			color: var(--text_Alt);
			font-size: var(--f_lg);
			text-shadow: var(--text_Shadow);
		}

		select {
			background: var(--back_Tre);
		}

		ul {
			display: flex;
			flex-direction: column;
			justify-content: space-between;
			align-items: center;
			gap: 5vh;
			margin-top: 2vh;
			margin-bottom: 4vh;
			list-style: none;
			font-size: var(--font);

			li {
				button {
					all: unset;
				}
				p {
					margin-top: 1vh;
					margin-bottom: 1vh;
					font-size: var(--f_sm);
					color: var(--highlight);
					text-shadow: var(--text_Shadow);
				}
			}
		}

		.burger {
			height: 15%;
			width: 50%;
			aspect-ratio: 1;
			background-color: transparent;
			margin-right: 6vw;
			display: flex;
			align-items: center;
			justify-content: center;

			&:hover {
				cursor: pointer;
				transition: transform 0.1s ease-in-out;
				transform: scale(1.2);
			}
		}

		.burger > div {
			height: 2px;
			width: 14px;
			background-color: var(--highlight);
			position: absolute;
		}
	}

	.current {
		position: relative;
	}

	.current::after {
		content: '';
		position: absolute;
		bottom: 0;
		left: 0;
		width: 100%;
		height: 2px;
		background-color: var(--back_Main);
	}

	//laptop
	@media only screen and (min-width: 769px) {
		nav {
			display: flex;
		}

		.navbar {
			button {
				all: unset;
			}

			height: 4rem;

			.burger {
				display: none;
			}

			.logo {
				img {
					width: 15vw;
					padding: 3%;
					margin-left: 1vw;
				}
			}

			ul {
				flex-direction: row;
				margin: 2vh -20vw 2vh 0;
			}

			a {
				font-size: var(--f_md);
			}
		}
	}

	@media only screen and (min-width: 1440px) {
		.navbar {
			.logo {
				img {
					width: 10vw;
					padding: 0;
					margin-left: 1vw;
				}
			}

			ul {
				flex-direction: row;
				margin: 2vh -40vw 2vh 0;
			}

			a {
				font-size: var(--f_lg);
			}
		}
	}
</style>
