<script lang="ts">
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/Facilities-1.jpg';
	import logowelcome from '$lib/images/svelte-welcome.png';
	import welcomeFallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>This is Irman Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<h1>Testing the color out here but it seems doesnt change at all</h1>

<section>
	<h1>
		<span class="images_styles_1">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src={welcomeFallback} alt="Welcome" />
			<picture>			
		</span>
		Use outline if you don’t want to change element dimensions.
		<br />SvelteKit app
		<br />tapi kan
	</h1>
	<h1>Testing the color out here but it seems doesnt change at all</h1>
	<Counter />
</section>

<style>
* {
    border: 1px solid rgb(255, 0, 208); /* See all element boxes */
}

section {
    display: flex;
    flex-direction:row;
    justify-content: center;
    align-items: start;
    flex: 1.0;
}

h1 {
    color: black;
    font-family: 'Courier New', Courier, monospace;
    width: 100%;
    border: 1px dashed rgb(122, 187, 227); /* Highlights h1 */
}
.images_styles_1 {
    display: block;
    position: relative;
    width: 100%;
    height: 0;
    padding: 0 0 calc(100% * 495 / 2048) 0;
    border: 3px solid orange; /* See i mage box */
}
.images_styles_1 img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    display: block;
    border: 2px solid blue; /* See actual image */
}
</style>

<!-- <style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items:center;
		flex: 0.6;
	}

	h1 {
		color: cyan;
		font: Helvetica, sans-serif;
		width: 100%;
	}

	.images_styles_2 {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.images_styles_2 img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}

	.images_styles_1 {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.images_styles_1 img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style> -->


