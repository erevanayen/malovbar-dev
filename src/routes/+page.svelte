<script>
	import heroImage from '$lib/assets/heroImage.png';
	import LogoFlower from '$lib/assets/logo-flower.svelte';
	import Footer from '$lib/components/footer/Footer.svelte';
	import Header from '$lib/components/header/Header.svelte';
	import { onMount } from 'svelte';

	let middle = 100;

	onMount(() => {
		middle = window.innerHeight / 2;
	});
</script>

<Header scrollNavBar={middle}></Header>

<section class="hero">
	<div class="text-logo">
		<span>malovbar</span>
		<LogoFlower width={'50px'} />
	</div>
	<img src={heroImage} alt="hero" />
</section>

<section class="content">show products here</section>

<Footer />

<style lang="scss">
	@import '../lib/styles/fonts';
	@import '../lib/styles/colors';

	body {
		margin: 0px;
	}

	.hero {
		height: 100svh;
		position: relative;
		img {
			width: 100vw;
			height: 100%;
			object-fit: cover;
			position: fixed;
			z-index: -1;
		}
	}

	.text-logo {
		display: flex;
		align-items: center;
		position: absolute;
		left: 50%;
		top: 50%;
		transform: translate(-50%, -50%);

		font-weight: 500;
		font-size: 3em;
		font-family: 'Inter', sans-serif;

		span {
			margin-right: 8px;
		}
	}

	.content {
		height: 100svh;
		background-color: $color-white;
	}
</style>
