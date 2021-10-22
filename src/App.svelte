<script>
  import windowslist from "./data";
</script>

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
