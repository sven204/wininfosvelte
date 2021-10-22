<script>
	// This array has all of the information in the website.
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
<h1>Test!</h1>
<!-- This is #each loop in Svelte. It loops over the array of objects, in the variable called "windowslist".-->
{#each windowslist as windows}
<div class="card">
	{windows.name} <br> {windows.version} <br> Released in {windows.released}
</div>
<br>
{/each}
<!-- PLEASE change these styles. (if you use this help of course) -->
<style>
	.card {
		height: 100px;
		background-color: orange;
		width: 200px;
		color: white;
		padding: 5px;
	}
</style>
