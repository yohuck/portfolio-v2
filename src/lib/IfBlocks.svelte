<script>


    let user = { darkMode: false }
    $: lightMode = user.darkMode ? 'dark' : 'light'

    let toggle = () => {
        user.darkMode = !user.darkMode;
    }
</script>

<button on:click={toggle} class={lightMode}>
    Turn on {user.darkMode ? 'light mode' : 'dark mode' }
</button>

{#if user.darkMode}
<p class={lightMode + 'paragraph'}>This block of text should only show in dark mode. Pretty cool, huh? </p>
{/if}

<style>
        /* --black: #000000ff;
        --rich-black-fogra-39: #111111ff;
        --jet: #333333ff;
        --white: #ffffffff;
        --flickr-blue: #0761d1ff;
        --french-rose: #ea558dff; */
    button{
        font-family:monospace;
        font-size: 0.8rem;
        padding: 1em;
        background-color: white;
        box-shadow: 4px 4px #0761d1ff;
        transition: 200ms;
    }

    .dark{
        background-color: #111111ff ;
        color: white;
        box-shadow:4px 4px #ea558dff;
    }

    .darkparagraph{
        margin: 2rem auto;
        padding: 1rem;
        max-width: 500px;
        font-size: 1.2rem;
        font-weight: 200;
        background-color: #111111ff;
        color: white;
    }

</style>