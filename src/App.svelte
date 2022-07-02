<script>
  import logo from './assets/logo_1_transparent.png'
import IfBlocks from './lib/IfBlocks.svelte'
import Logo from './lib/Logo.svelte'
</script>

<main>
  <img src={logo} alt="Svelte Logo" />
  <Logo />
  <h1>creative developer</h1>


  <p>
    Visit <a href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte
    apps.
  </p>

  <p>
    Check out <a href="https://github.com/sveltejs/kit#readme">SvelteKit</a> for
    the officially supported framework, also powered by Vite!
  </p>
  
  <IfBlocks />
</main>

<style>
  :root {
    font-family: monospace;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
    background-color: rgb(236, 221, 219);
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
</style>
