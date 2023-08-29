<svelte:head>
	<title>Efecto1</title>
	<meta name="description" content="About this app" />
</svelte:head>


<script>
</script>

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
		background-color: #f7f7f7;
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
		color: #ff00cc;
		margin-bottom: 20px;
	}

	.letter {
		display: inline-block;
		transform: translateY(-100%);
		animation: slideInTop 0.5s ease-in-out forwards;
		opacity: 0;
		color: #ff00cc;
		font-size: 48px;
	}

	.subtitle {
		font-size: 24px;
		color: #666;
		margin-bottom: 5px;
		opacity: 0;
		animation: fadeIn 1s ease-in-out forwards;
	}

	.main-title {
		font-size: 36px;
		color: #333;
		opacity: 0;
		animation: fadeIn 1s ease-in-out forwards;
	}

	@keyframes slideInTop {
		to {
			transform: translateY(0);
			opacity: 1;
		}
	}

	@keyframes fadeIn {
		to {
			opacity: 1;
		}
	}
</style>
