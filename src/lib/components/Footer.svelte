<script lang="ts">
	import LogoFlower from '$lib/assets/logo-flower.svelte';
</script>

<footer>
	<div class="grid">
		<div id="left">
			<span>
				Some very inspirational stuff to entertain and enlighten the reader. Also to show some other
				text in the footer than just plain links.
			</span>
		</div>
		<div id="center"><LogoFlower strokeColor={'#ffffff'} width={'50px'} /></div>
		<div id="right">
			<a href="/">malovbar@gmail.com</a>
			<a href="https://www.instagram.com/malovbar/" target="_blank">instagram</a>
			<a href="/">linkedIn</a>
		</div>
	</div>
</footer>

<style lang="scss">
	@import '$lib/styles/colors';
	@import '$lib/styles/fonts';
	@import '$lib/styles/mixins';

	footer {
		width: 100vw;
		display: flex;
		justify-content: center;

		font-family: 'Roboto', sans-serif;

		background-color: $color-magenta;
		color: $color-white;

		padding-top: 64px;

		a {
			text-decoration: none;
			color: $color-white;
		}
	}

	.grid {
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;

		width: 60%;

		> div {
			min-height: 200px;
		}
	}

	#left {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;

		span {
			max-width: 80%;
			margin-bottom: 1.5em;
		}
	}

	#center {
		display: flex;
		justify-content: center;
		align-items: center;
	}

	#right {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-end;

		a {
			margin-bottom: 1.5em;
		}
	}

	@include bp(mobile) {
		.grid {
			width: 100%;
			grid-template-columns: 1fr;

			#left,
			#center,
			#right {
				align-items: center;
			}

			#left {
				span {
					max-width: 50%;
				}
			}
		}
	}
</style>
