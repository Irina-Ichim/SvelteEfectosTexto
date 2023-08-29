
<script>
</script>

<svelte:head>
	<title>Inicio</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="main-section">
	<h1>
		<span class="typing-title">¡Bienvenida a tu Plan de Vida!</span>
		<br />
		<span class="subtitle">Organiza y sigue tus metas diarias</span>
	</h1>

</section>

<style>
	.main-section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.1;
		background: linear-gradient(45deg, #ff00cc, #3333ff);
		height: 100vh;

	}

	h1 {
		width: 100%;
		text-align: center;
		margin: 0;
		padding: 40px 0;
		font-family: 'Helvetica Neue', sans-serif;
		color: #fff;
		background: linear-gradient(45deg, #ff00cc, #3333ff);
		background-clip: text;
		-webkit-background-clip: text;
	}

	.typing-title {
		font-size: 36px;
		display: inline-block;
		border-right: 3px solid #fff;
		padding-right: 5px;
		animation: typingAnimation 4s steps(30) forwards, blinkCursor 0.75s step-end infinite;
	}

	.subtitle {
		font-size: 24px;
		color: lightgray;
		margin-top: 15px;
	}

	@keyframes typingAnimation {
		from {
			width: 0;
		}
		to {
			width: 100%;
		}
	}

	@keyframes blinkCursor {
		to {
			border-color: transparent;
		}
	}
</style>