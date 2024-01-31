<script lang="ts">
	import LogoFlower from '$lib/assets/logo-flower.svelte';
</script>

<header>
	<a href="/" id="logo-link"><span>malovbar</span><LogoFlower width={`50px`} /></a>
	<nav>
		<a href="/">products</a>
		<a href="/">about</a>
	</nav>
</header>

<style lang="scss">
	@import '$lib/styles/colors';
	@import '$lib/styles/fonts';
	@import '$lib/styles/mixins';

	header {
		position: fixed;
		top: 0;
		width: 100vw;

		display: flex;
		justify-content: center;
		align-items: center;
		background-color: $color-white;
		height: 72px;
		width: 100vw;

		font-family: 'Inter', sans-serif;
		color: $color-dark;

		border-bottom: 1px solid $color-dark;

		pointer-events: none;
	}

	#logo-link {
		font-weight: 500;
		font-size: 48px;
		display: flex;

		color: $color-dark;
		text-decoration: none;

		span {
			margin-right: 8px;
		}
	}

	nav {
		position: absolute;
		right: 0px;

		margin-right: 32px;

		font-size: 1.5em;

		a {
			text-decoration: none;
			color: $color-dark;
		}

		a:not(:last-child) {
			margin-right: 32px;
		}
	}

	@include bp(mobile) {
		nav {
			display: none;
		}
	}
</style>
