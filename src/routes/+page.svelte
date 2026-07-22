<script>
	let message = 'hello world';

	function handleClick() {
		const now = new Date();
		const timeString = now.toLocaleTimeString();
		message = `you clicked me at ${timeString}`;
	}
</script>

<main>
	<h1>{message}</h1>
	<button on:click={handleClick}>click me</button>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100vh;
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu,
			Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
	}

	h1 {
		font-size: 2rem;
		margin-bottom: 2rem;
		color: #333;
	}

	button {
		padding: 12px 24px;
		font-size: 1rem;
		background-color: #0066cc;
		color: white;
		border: none;
		border-radius: 4px;
		cursor: pointer;
		transition: background-color 0.2s;
	}

	button:hover {
		background-color: #0052a3;
	}

	button:active {
		background-color: #003d7a;
	}
</style>
