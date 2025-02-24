<script lang="ts">
	import Header from './Header.svelte';
	import '../app.css';

	let { children } = $props();
</script>

<div class="app">
	<Header />

	<main>
		{@render children()}
	</main>

	<footer>
		<p>
			visit <a href="https://svelte.dev/docs/kit">svelte.ddev/docs/kit</a> 
			to learn about SvelteKit take me take me
			<b> wow </b>
		</p>
	</footer>
</div>

<style>
	* {
    border: 3px solid rgb(77, 255, 0); /* See all element boxes */
	}

	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		border: 10px solid rgb(85, 0, 255);
	}

	main {
		/* flex: 1; */
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 640rem;
		margin: 0 auto;
		box-sizing: border-box;
		border: 1px solid rgb(255, 0, 68);
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
		border:20px solid rgb(85, 0, 255);
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}

	footer b{
		font-size: extra-large;
		border:20px solid rgb(85, 0, 255);
	}
</style>
