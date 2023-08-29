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

	.title {
		text-align: center;
		margin: 0;
		padding: 40px 0;
		font-family: 'Helvetica Neue', sans-serif;
		font-size: 24px;
		color: #333;
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
</style>

