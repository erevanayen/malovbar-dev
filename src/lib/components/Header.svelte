<header>
	<a id="logo-link" href="#">malovbar</a>
	<nav>
		<a href="#">products</a>
		<a href="#">about</a>
	</nav>
</header>

<style lang="scss">
	header {
		position: relative;

		display: flex;
		justify-content: center;
		align-items: center;
		background-color: #ffffff;
		height: 64px;
	}

	#logo-link {
	}

	nav {
		position: absolute;
		right: 0px;

  margin-right: 32px;

  a:not(:last-child) {
  margin-right: 32px;
  }
	}
</style>
