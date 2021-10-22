<script>
	import windowslist from './data.js';
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
		background-color: white;
		border-radius: 5pt;
		width: 200px;
		color: white;
		padding: 5px;
	}
</style>
