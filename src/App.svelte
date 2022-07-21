<script>

import ChunkyNav from './lib/chunkyNav.svelte';

import Scroll from './lib/Scroll.svelte'
import Svgs from './lib/svgs.svelte';
import ContactForm from './lib/contact-form.svelte';
import Header from './lib/header.svelte'
import Blob from './lib/blob.svelte';
import { create_animation } from 'svelte/internal';

</script>

<main>
  <Header />
  <Scroll />

  <Svgs  />


  <!-- <ContactForm /> -->
</main>

<style>

@import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,300;0,500;0,800;1,100;1,300&display=swap');


  :root {
    font-family: 'JetBrains Mono', monospace;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }




/* Add the animation: property to whichever element you want to animate */


</style>
