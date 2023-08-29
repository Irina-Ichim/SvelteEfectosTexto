

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
		background-color: #1e1e1e;
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
		background-image: linear-gradient(45deg, #ff00cc, #3333ff);
		-webkit-background-clip: text;
		color: transparent;
		margin-bottom: 20px;
		animation: gradientFade 2s infinite alternate;
	}

	.letter {
		display: inline-block;
	}

	.subtitle {
		font-size: 24px;
		color: #999;
		margin-bottom: 5px;
		opacity: 0.8;
	}

	.main-title {
		font-size: 36px;
		color: #fff;
	}

	@keyframes gradientFade {
		from {
			-webkit-background-clip: text;
			color: transparent;
		}
		to {
			-webkit-background-clip: unset;
			color: inherit;
		}
	}
</style>