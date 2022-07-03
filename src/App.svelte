<script>
  import logo from './assets/logo_1_transparent.png'
import IfBlocks from './lib/IfBlocks.svelte';
import ChunkyNav from './lib/chunkyNav.svelte';
import Logo from './lib/Logo.svelte'
</script>

<main>
  <IfBlocks />
  <!-- <ChunkyNav /> -->
  <div class="wrapper">
    <img src={logo} alt="Svelte Logo" />
    
  </div>
</main>

<style>
  :root {
    font-family: monospace;
  }

  main {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-align: center;
    padding: 1em;
    margin: 0 auto;
    background-color: rgb(219, 229, 236);
  }

  .wrapper{
    position: absolute;
    top: 0;
    left: 0;
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: rgba(219, 229, 236, 0.936);
    z-index: -1;
  }

  img{
    max-width: 300px;
  }

  h1 {
    color: #0761d1ff;
    text-transform: uppercase;
    font-size: 4rem;
    font-weight: 100;
    line-height: 1.1;
    margin: 2rem auto;
    max-width: 14rem;
  }

  p {
    max-width: 14rem;
    margin: 1rem auto;
    line-height: 1.35;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }

  ifBlocks{
    position: absolute;
    top: 0;

  }
</style>
