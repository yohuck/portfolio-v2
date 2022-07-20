

<script>
    import Blob from "./blob.svelte";
</script>

<div class='container'>
    <section>
        <img src="/images/logo_1_transparent.png" alt="Eric Lake Logo">
        <h1>Web Developer</h1>
    </section>
    <section id="about">
        <h4>Hi There! I'm Eric</h4>
        <p>
            I'm a web developer living in Englewood, CO. I love building whimsical, bold, clever UI and drinking coffee until it's time to drink wine.
        </p>
        <p>
            I'm a graduate of the University of Denver Full Stack Bootcamp program and am hoping to land my first job as a web developer.
        </p>
        <p>
            I've spent the last decade working in customer operations for a sports technology startup and have built teams and processes from the ground up through aquisition.
        </p>
        <p>
           I'm proficient with HTML, CSS, JavaScript, Node.JS, Express, MongoDB, SQL, React, and Svelte. I have experience with Bootstrap, Tailwind, and Bulma, but I'm just as happy writing custom css like you'll find here.
        </p>
        <p>
            In my free time I'm a DJ, musician, tabletop gamer, and seltzer water enthusiast.
        </p>
        <p>
           Check out my project gallery, my GitHub Data, or my Social Media Profiles. I'm a big proponent of Learning in Public and hope to continue on my development journey working with you.
        </p>

    </section>
    <section id="work">
        <div class="scrollport">
            <div class="proj" id="one"><p>This is one</p></div>
            <div class="proj" id="two"><p>This is two</p></div>
            <div class="proj" id="three"><p>This is three</p></div>
            <div class="proj"><p>This is four</p></div>
            <div class="proj"><p>This is five</p></div>
            <div class="proj"><p>This is siz</p></div>
            <div class="proj"><p>This is seven</p></div>
            <div class="proj"><p>This is eight</p></div>

        </div>

    </section>
    <section id="data">
        <h4>Hi There! I'm Eric</h4>
        <p>
            I'm a web developer living in Englewood, CO. I love building whimsical, bold, clever UI and drinking coffee until it's time to drink wine.
        </p>
        <p>
            I'm a graduate of the University of Denver Full Stack Bootcamp program and am hoping to land my first job as a web developer.
        </p>
        <p>
            I've spent the last decade working in customer operations for a sports technology startup and have built teams and processes from the ground up through aquisition.
        </p>
        <p>
           I'm proficient with HTML, CSS, JavaScript, Node.JS, Express, MongoDB, SQL, React, and Svelte. I have experience with Bootstrap, Tailwind, and Bulma, but I'm just as happy writing custom css like you'll find here.
        </p>
        <p>
            In my free time I'm a DJ, musician, tabletop gamer, and seltzer water enthusiast.
        </p>
        <p>
           Check out my project gallery, my GitHub Data, or my Social Media Profiles. I'm a big proponent of Learning in Public and hope to continue on my development journey working with you.
        </p>
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
        /* -ms-overflow-style: none;  */
         scrollbar-width: none;  
    }

   .container::-webkit-scrollbar{
  display: none;
}

.container::-webkit-scrollbar {
    display: none;
}



    section:nth-of-type(1){
        background-color: yellow;
        background-color: #EE4266;
    }
    section:nth-of-type(2){
        background-color: #FFD23F;
    }
    section:nth-of-type(3){
    background-color: #3BCEAC;
    /* overflow-x: auto;
    overscroll-behavior-x: contain;
    display: flex;
    flex-direction: row;
    gap: 2rem;
    align-items: center;
    justify-content: center;
    padding: 5rem; */

    }

.scrollport{


    height: 100%;
    width: 90%;
    max-width: 100vw;
    overflow-x: auto;
    /* overscroll-behavior-x: contain; */
    display: flex; 
    flex-direction: row; 
    /* gap: 2rem; */
    align-items: center;
    justify-content: start;
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

    h4{
        font-size: 5rem;
        text-align: left;
        line-height: 4rem;
        margin: 1rem auto;
        max-width: 80%;
    }

    p{
        width: 80%;
        max-width: 800px;
    }


 .proj {
    height: calc(90vw - 2rem);
    max-height: 500px;
    aspect-ratio: 1;
    padding: 1rem;
    /* margin: 1rem; */
  /* block-size: 80%; */
  background-color: #ee4267bb;
}

.proj + .proj {
    margin-left: 1rem;
}



</style>