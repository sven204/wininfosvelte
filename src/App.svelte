<script>
  import windowslist from "./data";
  import themelist from "./themelist";
  let selectedTheme = "w11dark";
</script>

<div class="container {selectedTheme}">  
  <label for="theme">Theme</label>
  <select name="theme" id="theme" bind:value={selectedTheme}>
    {#each themelist as theme}
      <option value={theme}>{theme}</option>
    {/each}
  </select>
  <h1>WinInfo by JaydenDevelopment</h1>
  <p>Dynamic WebApp with information about Windows builds.</p>
  {#each windowslist as windows}
    <div class="card {selectedTheme}">
      <p>
        {windows.name}
        <br />
        Build: {windows.build}
        <br />
        Released: {windows.rel}
        <br />
        EOL: {windows.eol}
        <br />
        <!-- Last Update: {windows.last} -->
      </p>
    </div>
    <br />
  {/each}
</div>

<style>
  /* button {
    border-radius: 5pt;
  } */
  
  * {
    color: white;
  }
  
  .container {
    width: 100vw;
    min-height: 100vh;
    padding: none;
    margin: none;
  }
  
  .card {
    height: 100%;
    width: 100%;
    background-color: white;
    border-radius: 5pt;
    width: 200px;
    color: black;
    padding: 5px;
  }

</style>
