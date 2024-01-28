<script lang="ts">
	import LogoFlower from '$lib/assets/logo-flower.svelte';
	import '$lib/styles/style.scss';
	import { onDestroy, onMount } from 'svelte';

	export let scrollNavBar = 60;
	export let hideable = true;

	let show = false;

	onMount(() => {
		if (!hideable) {
			show = true;
			return;
		}

		window.onscroll = () => {
			if (window.scrollY > scrollNavBar) {
				show = true;
			} else {
				show = false;
			}
		};
	});
</script>

<header class:scrolled={show}>
	<div></div>
	<a id="logo-link" href="/"><span>malovbar</span><LogoFlower width={'50px'} /></a>
	<nav>
		<a href="#">products</a>
		<a href="/about">about</a>
	</nav>
</header>

<style src="./header.scss">
</style>
