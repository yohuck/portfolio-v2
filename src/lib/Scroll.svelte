

<script>
    import Blob from "./blob.svelte";
    import Projects from "./projects.svelte";





    
</script>

<div class='container'>
    <section>
        <img src="/images/logo_1_transparent.png" alt="Eric Lake Logo">
        <h1>Web Developer</h1>
    </section>
    <section id="about">
        <Blob />
        <article class="yeller blob">

           
           

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

        </article>

    </section>
    <section id="work">
        <Projects />
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
        /* scroll-behavior: smooth; */
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








    section:nth-of-type(1){
        background-color: yellow;
        background-color: #EE4266;
    }
    section:nth-of-type(2){
        background-color: #eeeadc;
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

    #about{
        position: relative;
        overflow: hidden;
        background-color: #af42ee;
    }

    .yeller{

        box-sizing: border-box;
        border-radius: 10px;
        background-color: #FFD23F;
        padding: 2rem;
        width: 90%;
        max-width: 800px;
        z-index: 3;
        box-shadow: 10px 10px rgba(10, 9, 9, 0.795);
    }



    
    section:nth-of-type(4){
        background-color: #EE4266;
    }

    h1{
        text-align: left;
        font-size: 1rem;
        line-height: 0.8 em;
    }

    h4{
        font-size: clamp(2rem, 2rem + 5vw, 7rem);
        text-align: left;
        line-height: 1em;
        margin: 1rem auto;
        max-width: 800px;
    }

    p{
        width: 80%;
        max-width: 800px;
        font-weight: 300;

    }






</style>