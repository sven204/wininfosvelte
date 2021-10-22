<script>
	export let name;
	let count 0
	function handleClick() {
    		count++;
	}	
		let windowslist = [
	{
		"name": "Windows 11",
		"version": "Sun Valley",
		"released": "2021"
	},
	{
		"name": "Windows 10",
		"version": "Redstone",
		"released": "2015"
	},
	{
		"name": "Windows 7",
		"version": "Something IDK",
		"released": "2009 or something"
	},
	]
</script>

<main>
	<h3>WinInfo is back, now in SvelteJS!</h3>
	<p>Note: This app isn't ready yet, check back later!</p>
	
	<button on:click={handleClick}>Clicked {count} {count === 1 ? 'time' : 'times'}</button>
	<br>
	<br>
	{#each windowslist as windows}
	<div class="card">
	{windows.name} <br> {windows.version} <br> Released in {windows.released}
	</div>
	<br>
	{/each}
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
