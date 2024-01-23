<script>
	import profilePic from '$lib/assets/profilePic.png';
</script>

<section>
	<div class="about">
		<div class="about-head">
			<p>barbora</p>
			<p>malovana</p>
		</div>
		<p class="text">
			To put it mildly, the advantage of the essential component has become even more significant
			for The Evaluation of Special Facility" (Alan Andersen in The Book of the Application Rules)
			As a matter of fact the lack of knowledge of a small part of the resource management should
			set clear rules regarding every contradiction between the
		</p>
		<p class="text">
			To put it mildly, the advantage of the essential component has become even more significant
			for The Evaluation of Special Facility" (Alan Andersen in The Book of the Application Rules)
			As a matter of fact the lack of knowledge of a small part of the resource management should
			set clear rules regarding every contradiction between the
		</p>
	</div>
	<div class="image-container"><img src={profilePic} alt="profile" /></div>
</section>

<style lang="scss">
	section {
		font-family: 'Inter', sans-serif;
		display: grid;
		grid-template-columns: 1fr 1fr;

		padding: 128px 0px 256px;
	}

	.about {
		padding-right: 128px;
	}

	.about-head {
		font-size: 3em;

		p {
			margin: 0px;

			&:first-child {
				font-weight: 200;
			}
		}
	}

	.subtitle {
		font-size: 1.5em;
		font-weight: 300;

		margin-top: 0px;
	}

	.text {
		font-size: 1.25em;
		text-align: justify;
	}

	.image-container {
		img {
			aspect-ratio: 524/731;
		}
	}
</style>
