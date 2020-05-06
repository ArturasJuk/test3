<script>
	export let name;
	let count = 0;

	const handler = e => {
		count += 1;
		console.log('Counted: ' + count)
	}
</script>

<main>
	<h1>Hello {name}, {count}</h1>
	<button on:click={handler}>Click me</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>