<script>
</script>

<svelte:head>
	<title>Inicio</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		<span class="typing-title">¡Bienvenido a tu Plan de Vida!</span>
		<br />
		<span class="subtitle typing-subtitle">Organiza y sigue tus metas diarias</span>
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

	.typing-title,
	.typing-subtitle {
		display: inline-block;
		overflow: hidden;
		white-space: nowrap;
		border-right: 2px solid #fff;
		letter-spacing: 2px;
		animation: typing 3s steps(40, end), blink-caret 0.75s step-end infinite;
	}

	.typing-subtitle {
		animation: typing 3s steps(40, end), blink-caret 0.75s step-end infinite, delay 3s ease-out;
	}

	@keyframes typing {
		from {
			width: 0;
		}
		to {
			width: 100%;
		}
	}

	@keyframes blink-caret {
		from,
		to {
			border-color: transparent;
		}
		50% {
			border-color: #fff;
		}
	}

	@keyframes delay {
		from {
			visibility: visible;
		}
		to {
			visibility: hidden;
		}
	}
</style>