<script>
	import LogoFlower from '$lib/assets/logo-flower.svelte';
</script>

<footer>
	<div class="content">
		<div class="grid">
			<div id="left">
				<span>
					Some very inspirational stuff to entertain and enlighten the reader. Also to show some
					other text in the footer than just plain links.
				</span>
				<span>-by me</span>
			</div>
			<div id="center"><LogoFlower strokeColor={'#ffffff'} width={'50px'} /></div>
			<div id="right">
				<a href="">malovbar@gmail.com</a>
				<a href="https://www.instagram.com/malovbar/" target="_blank">instagram</a>
				<a href="">linkedIn</a>
			</div>
		</div>
		<div>© malovbar</div>
	</div>
</footer>

<style src="./footer.scss">
</style>
