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
		<div class="box">
			<p>
				visit <a href="https://svelte.dev/docs/kit">svelte.ddev/docs/kit</a> 
			</p>
			<p>
				visit <a href="https://svelte.dev/docs/kit">svelte.ddev/docs/kit</a> 
			</p>
			<p>
				visit <a href="https://svelte.dev/docs/kit">svelte.ddev/docs/kit</a> 
			</p>
		</div>

		<div class="box">
			<p>	
				visit <a href="https://svelte.dev/docs/kit">svelte.ddev/docs/kit</a> 
				visit <a href="https://svelte.dev/docs/kit">svelte.ddev/docs/kit</a> 
				visit <a href="https://svelte.dev/docs/kit">svelte.ddev/docs/kit</a> 
			</p>
		</div>

	</footer>

</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		border: 5px solid rgb(0, 255, 238);
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
		border: 1 px solid rgb(172, 58, 13);
	}

	/* footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
		border:3px solid rgb(85, 0, 255);
	} */

	footer {
	display: flex;
	flex-direction: row; /* Arrange items in a row */
	justify-content: space-between; /* Ensures boxes take full width */
	border: 3px solid rgb(0, 255, 89);
	}

	.box {
	flex: 1; /* Make both boxes take up equal space */
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	background-color: rgb(228, 213, 213);
	border: 3px solid red;
	font-weight: bold;
	}

	footer a {
		font-weight: bold;
		/* border:5px solid rgb(85, 0, 255); */
	}
	
	/*
	footer b{
		font-size: extra-large;
		border:5px solid rgb(85, 0, 255);
	}
	*/
</style>
