<script>
	export let name;
</script>

<main>
	<h3>WinInfo is back, now in SvelteJS!</h3>
	<p>Note: This app isn't ready yet, check back later!</p>
	
	<button on:click={handleClick}>
	Clicked {count} {count === 1 ? 'time' : 'times'}
	</button>
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
