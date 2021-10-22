<script>
  import windowslist from "./data";
  import Notifications from 'svelte-notifications';
	import Child from './child.svelte';
</script>


<Notifications>
	<Child />
</Notifications>

<h1>WinInfo by JaydenDevelopment</h1>
<p> Dynamic WebApp with information about Windows builds.</p>
{#each windowslist as windows}
  <div class="card">
    <p>
      {windows.name} 
      <br>
      Build: {windows.build} 
      <br> 
      Released: {windows.rel}
      <br>
      EOL: {windows.eol}
      <br>
      Last Update: {windows.last}
    </p>
  </div>
  <br />
{/each}

<style>
  button {
    border-radius: 5pt;
  }
  * {
    color: white;
  }
  .card * {
    color: black;
  }
  .card {
    height: 100px;
    background-color: white;
    border-radius: 5pt;
    width: 200px;
    color: black;
    padding: 5px;
  }
</style>
