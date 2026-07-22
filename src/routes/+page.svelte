<script>
	let message = $state('hello world');

	function handleClick() {
		const now = new Date();
		const timeString = now.toLocaleTimeString();
		message = `you clicked me at ${timeString}`;
	}
</script>

<main>
	<h1>{message}</h1>
	<button onclick={handleClick}>click me</button>
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
		background-color: #fafafa;
	}

	h1 {
		font-size: 2rem;
		margin-bottom: 2rem;
		color: #1a1a1a;
		font-weight: 600;
	}

	button {
		padding: 12px 24px;
		font-size: 1rem;
		font-weight: 500;
		background-color: #0066cc;
		color: white;
		border: none;
		border-radius: 6px;
		cursor: pointer;
		transition: all 0.2s ease;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
	}

	button:hover {
		background-color: #0052a3;
		box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
		transform: translateY(-1px);
	}

	button:active {
		background-color: #003d7a;
		transform: translateY(0);
	}
</style>
