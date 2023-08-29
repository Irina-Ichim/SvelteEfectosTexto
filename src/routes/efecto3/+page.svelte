<script>
</script>

<svelte:head>
	<title>Inicio</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		<span class="welcome">
			<span class="letter">B</span>
			<span class="letter">I</span>
			<span class="letter">E</span>
			<span class="letter">N</span>
			<span class="letter">V</span>
			<span class="letter">E</span>
			<span class="letter">N</span>
			<span class="letter">I</span>
			<span class="letter">D</span>
			<span class="letter">A</span>
		</span>
		<br />
		<span class="subtitle">A tu</span><br />
		<span class="main-title">Plan de vida</span>
	</h1>

</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
		background-color: #000;
	}

	h1 {
		width: 100%;
		text-align: center;
		margin: 0;
		padding: 40px 0;
		font-family: 'Helvetica Neue', sans-serif;
	}

	.welcome {
		font-size: 48px;
		display: block;
		background-image: linear-gradient(45deg, #f06, #0cf);
		-webkit-background-clip: text;
		color: transparent;
		animation: gradientFlow 2s infinite alternate;
		text-shadow: 0 3px 6px rgba(0, 0, 0, 0.5);
	}

	.letter {
		display: inline-block;
	}

	.subtitle {
		font-size: 24px;
		color: #888;
		margin-bottom: 5px;
	}

	.main-title {
		font-size: 36px;
		color: #fff;
	}

	@keyframes gradientFlow {
		from {
			background-position: 100% 0;
		}
		to {
			background-position: 0 100%;
		}
	}
</style>