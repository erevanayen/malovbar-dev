<script>
	import Header from '$lib/components/header/Header.svelte';
	import Footer from '$lib/components/footer/Footer.svelte';
	import '$lib/styles/style.scss';
</script>

<Header hideable={false} />

<main>
	<slot />
</main>

<Footer />

<style>
	main {
		padding: 0px;
	}
</style>
