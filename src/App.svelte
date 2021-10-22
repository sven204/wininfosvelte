<script>
	// This array has all of the information in the website.
	let windowslist = [
		{
			"name": "Windows 11 22000.194",
			"version": "21H2",
			"codename": "Sun Valley",
			"released": "2021",
			"eol": "N/A"
		},
		{
			"name": "Windows 10",
			"version": "21H1",
			"codename": "Redstone",
			"released": "2015",
			"eol": "2025"
		},
		{
			"name": "Windows 7",
			"version": "NT 6.1",
			"codename": "Blackcomb",
			"released": "2009",
			"eol": "2020"
		},
	]
</script>
<h1>Test!</h1>
{#each windowslist as windows}
<div class="card">
	{windows.name} <br> {windows.version} <br> Released in {windows.released}
</div>
<br>
{/each}
<style>
	.card {
		height: 100px;
		background-color: orange;
		width: 200px;
		color: white;
		padding: 5px;
	}
</style>
