<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">

	<main>
		<slot />
	</main>

	<footer class="bg-white">
		<p>2023 Copyright. All Rights Reserved.</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		background-color: #f4eded;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 94rem;
		margin: 0 auto;
		box-sizing: border-box;
		position: relative;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
