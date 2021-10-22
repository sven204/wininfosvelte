<script>
  import windowslist from "./data";
</script>

<h1>Test!</h1>
{#each windowslist as windows}
  <div class="card">
    <p>
      {windows.name} <br/>
      Build: {windows.build} 
      <br/> 
      Released: {windows.rel}
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
