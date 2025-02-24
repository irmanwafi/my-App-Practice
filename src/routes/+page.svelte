<script>
	// JavaScript: Define a title and description for the card
	let title = "Flexbox Cardio";
	let description = "This is an example of a centered card using flexbox.";
</script>

<!-- Flex Container (Outer div) -->
<div class="flex-container">
	<!-- Card inside the flex container -->
	<div class="card">
		<h2>{title}</h2> <!-- Display title from JavaScript -->
		<p>{description}</p> <!-- Display description from JavaScript -->
		<button>Click Me</button> <!-- Button inside the card -->
	</div>
</div>

<!-- Another div with a paragraph and button -->
<div class="normal-div">
    <p>Wow</p>
    <button>Click Me</button>
</div>

<div class="test">
	ceyddd
</div>

<h3>Testing	dsfsfsfsf</h3>

<style>
	/* Flex container (outer) */
	.flex-container {
		display: flex;
		justify-content: center; /* Center items horizontally */
		align-items: center; /* Center items vertically */
		height: 100vh; /* Full viewport height */
		border: 5px solid red; /* Red border to visualize */
		background-color: #f0f0f0;
	}

	/* Card inside flex container */
	.card {
		padding: 20px;
		border: 5px solid blue; /* Blue border to see the card */
		background: white;
		box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.2);
		text-align: center;
	}

	/* Normal div (outside flex) */
	.normal-div {
		/* margin-top: 0px;
		padding: 0px; */
		border: 5px solid green; /* Green border around normal div */
	}

	/* Button Styling */
	button {
		padding: 10px;
		margin-top: 10px;
		border: 3px solid purple; /* Purple border around buttons */
		background-color: lightgray;
		cursor: pointer;
	}

	.test {
		border: 3px solid purple;
	}
</style>
