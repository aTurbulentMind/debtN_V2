<div class="navbar">
	<a href="/" class="logo"><h1>DEBT$NET</h1></a>
	<nav>
		<!--this is the main navigation menu-->
		<ul>
			<li>
				<a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ/">CALL NOW</a>
			</li>

			<li>
				<a href="/software/">Software</a>
			</li>
			<li>
				<a href="/reviews/">Reviews</a>
			</li>
			<li>
				<a href="/about/">About</a>
			</li>
			<li>
				<a href="/Contact/">Contact</a>
			</li>
			<li>
				<a href="/">Home</a>
			</li>
		</ul>
	</nav>
	<div>
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
			><path
				d="M169.7 .9c-22.8-1.6-41.9 14-47.5 34.7L110.4 80c.5 0 1.1 0 1.6 0c176.7 0 320 143.3 320 320c0 .5 0 1.1 0 1.6l44.4-11.8c20.8-5.5 36.3-24.7 34.7-47.5C498.5 159.5 352.5 13.5 169.7 .9zM399.8 410.2c.1-3.4 .2-6.8 .2-10.2c0-159.1-128.9-288-288-288c-3.4 0-6.8 .1-10.2 .2L.5 491.9c-1.5 5.5 .1 11.4 4.1 15.4s9.9 5.6 15.4 4.1L399.8 410.2zM176 208a32 32 0 1 1 0 64 32 32 0 1 1 0-64zm64 128a32 32 0 1 1 64 0 32 32 0 1 1 -64 0zM96 384a32 32 0 1 1 64 0 32 32 0 1 1 -64 0z"
			/></svg
		>
	</div>
</div>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	:global(*) {
		box-sizing: border-box;
	}

	.navbar {
		background-color: var(--back_Alt);
		width: 100vw;
		display: flex;
		justify-content: space-between;
		position: fixed;
		height: 5rem;
		z-index: 950;
		box-shadow: var(--box_Shadow);
		transition: transform 0.2s ease-in-out;

		a,
		select {
			color: var(--text_Alt);
			font-size: var(--f_lg);
			text-shadow: var(--text_Shadow);
		}

		select {
			background: var(--back_Tre);
		}
	}

	.logo {
		h1 {
			font-size: var(--f_lg);
			margin: var(--marg);
		}
	}

	ul {
		flex-direction: row;
	}

	@media only screen and (max-width: 767px) {
		.navbar {
			height: 3rem;
		}

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
	}

	.logo {
		h1 {
			font-size: var(--f_m);
		}
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
			p {
				margin-top: 1vh;
				margin-bottom: 1vh;
				font-size: var(--f_sm);
				color: var(--highlight);
				text-shadow: var(--text_Shadow);
			}
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

	.burger {
		height: 30px;
		width: 30px;
		aspect-ratio: 1;
		background-color: transparent;
		margin-top: 1vh;
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

	@media only screen and (min-width: 768px) {
		.burger {
			display: none;
		}

		ul {
			flex-direction: row;
		}

		.space {
			margin-right: 2vw;
		}
	}

	@media only screen and (min-width: 740px) {
	}

	@media only screen and (min-width: 980px) {
	}
</style>
