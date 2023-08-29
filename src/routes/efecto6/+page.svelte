<script>
</script>

<svelte:head>
	<title>Inicio</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		<span class="title">¡Bienvenido a tu</span>
		<br />
		<span class="title highlight">Plan de Vida!</span>
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
		height: 100vh;
	}

	h1 {
		width: 100%;
		text-align: center;
		margin: 0;
		padding: 40px 0;
		font-family: 'Helvetica Neue', sans-serif;
		color: #fff;
	}

	.title {
		font-size: 36px;
		animation: move 2s infinite, changeColor 4s infinite;
	}

	.title.highlight {
		font-size: 48px;
		animation: move 2s infinite reverse, changeColor 4s infinite reverse;
	}

	@keyframes move {
		0%, 100% {
			transform: translateY(0);
		}
		25% {
			transform: translateY(-10px);
		}
		50% {
			transform: translateY(0);
		}
		75% {
			transform: translateY(10px);
		}
	}

	@keyframes changeColor {
		0% {
			color: #ff00cc;
		}
		25% {
			color: #3333ff;
		}
		50% {
			color: #00ff00;
		}
		75% {
			color: #ff0000;
		}
		100% {
			color: #ff00cc;
		}
	}
</style>