

<script>
    import Blob from "./blob.svelte";
</script>

<div class='container'>
    <section>
        <img src="\src\assets\logo_1_transparent.png" alt="Eric Lake Logo">
        <h1>Web Developer</h1>
    </section>
    <section>
        <h1>Page Two</h1>

    </section>
    <section>
        <h1>Page Three</h1>

    </section>
    <section>
        <h1>Page Four</h1>
    </section>
</div>

<style>
    body{
        width: 100vw;
        height: 100vh;
        margin: 0;
        padding: 0;
    }

    img{
    width: clamp(200px, 30%, 800px);
}



    .container{
        width: 100vw;
        height: 100vh;
        scroll-behavior: smooth;
        background-color: green;
        scroll-snap-type: y mandatory;
        overflow-y: scroll;
        /* display: flex; */
    }


    section{
        flex: none;
        scroll-snap-align: start;
        height: 100%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    section:nth-of-type(1){
        background-color: yellow;
        background-color: #ffd23f;
    }
    section:nth-of-type(2){
        background-color: #540D6E;
    }
    section:nth-of-type(3){
        background-color: #3BCEAC;
    }
    section:nth-of-type(4){
        background-color: #EE4266;
    }

    h1{
        text-align: center;
        font-family: monospace;
        font-size: 1rem;
        line-height: 0.8 em;
    }
</style>