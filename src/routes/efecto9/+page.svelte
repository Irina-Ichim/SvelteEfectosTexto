<script>
</script>

<svelte:head>
	<title>Inicio</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1 class="title">
		<span class="word">Bienvenido</span>
		<br />
		<span class="word">a tu</span>
		<br />
		<span class="word">Plan de Vida</span>
	</h1>
</section>

<style>
	/* Estilos para el título y la animación de palabras aquí */

	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
		background-color: #f0f0f0;
		height: 100vh;
		overflow: hidden;
	}

	h1 {
		width: 100%;
		text-align: center;
		margin: 0;
		padding: 40px 0;
		font-family: 'Helvetica Neue', sans-serif;
		color: #333;
	}

	.title {
		font-size: 36px;
		animation: move 2s infinite, changeColor 4s infinite;
	}

	.word {
		display: block;
		opacity: 0;
		transform: scale(0.8) rotate(-45deg);
		animation: rotateIn 1s ease-in-out, fadeInUp 1.5s ease-in-out;
		animation-fill-mode: forwards;
	}

	.word:nth-child(2) {
		animation-delay: 0.5s;
	}

	.word:nth-child(3) {
		animation-delay: 1s;
	}

	@keyframes rotateIn {
		0% {
			opacity: 0;
			transform: scale(0.8) rotate(-45deg);
		}
		100% {
			opacity: 1;
			transform: scale(1) rotate(0);
		}
	}

	@keyframes fadeInUp {
		0% {
			opacity: 0;
			transform: translateY(30px);
		}
		100% {
			opacity: 1;
			transform: translateY(0);
		}
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
