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

<style>
        /* --black: #000000ff;
        --rich-black-fogra-39: #111111ff;
        --jet: #333333ff;
        --white: #ffffffff;
        --flickr-blue: #0761d1ff;
        --french-rose: #ea558dff; */
    button{
        font-family: Arial, Helvetica, sans-serif;
        font-size: 2rem;
        padding: 1em;
        background-color: white;
        box-shadow: 10px 10px red;
    }

    .dark{
        background-color: #111111ff ;
        color: white;
        box-shadow:10px 10px #ea558dff;
    }

</style>