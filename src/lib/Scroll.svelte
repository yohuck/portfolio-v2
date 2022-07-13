<div class='container'>
    <section>
        <h1>Page One</h1>
    </section>
    <section>
        <h1>Page Two</h1>
    </section>
    <section>
        <h1>Page Three</h1>
    </section>
</div>

<style>
    body{
        width: 100vw;
        height: 100vh;
        margin: 0;
        padding: 0;
    }

    .container{
        width: 100vw;
        height: 100vh;
        background-color: green;
        scroll-snap-type: x mandatory;
        overflow-x: scroll;
        display: flex;
    }


    section{
        flex: none;
        scroll-snap-align: start;
        height: 100%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    section:nth-of-type(1){
        background-color: yellow;
    }
    section:nth-of-type(2){
        background-color: green;
    }
    section:nth-of-type(3){
        background-color: purple;
    }
    section:nth-of-type(4){
        background-color: blue;
    }

    h1{
        font-family: monospace;
        font-size: 10rem;
    }
</style>