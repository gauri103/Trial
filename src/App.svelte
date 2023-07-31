<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Trial from './trial.svelte'

</script>
<h1>Vite + Svelte</h1>
<div class="logo">
    <a href="https://vitejs.dev" target="_blank" rel="noreferrer">
      <img src={viteLogo} class="logo1" alt="Vite Logo" />
    </a>
    <a href="https://svelte.dev" target="_blank" rel="noreferrer">
      <img src={svelteLogo} class="logo2" alt="Svelte Logo" />
    </a>
  </div>


    <p>
    <Trial/>

  </p>


<style>
  .logo {
    height:100px;
    /* width:300px; */
    padding: 50px;
    display:flex;
    will-change: filter;
    transition: filter 300ms;
    position:relative;
    bottom: 50px;
    right: 50px;
    

    }
    h1{
      font-size: 80px;
      margin:0;
      box-sizing: border-box;
      text-align: center;
      align-items: center;
      width:500px;
      height: 100px;
      display:flex;
      float:left;
      border-style: solid;
      border-color: aqua;


    }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
</style>
