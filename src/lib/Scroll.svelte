

<script>
    import Blob from "./blob.svelte";
    import Projects from "./projects.svelte";
    import WorkInfo from "./work-info.svelte";





    
</script>

<div class='container'>
    <!-- <section>
        <img src="/images/logo_1_transparent.png" alt="Eric Lake Logo">
        <h1>Web Developer</h1>
    </section> -->
    <section id="about">
        <Blob />
        <article class="yeller blob">

           
           

            <h4>Hi There! I'm Eric</h4>
            <p>
                I'm a web developer living in Englewood, CO. I love building whimsical, bold UI and drinking coffee until it's time to drink wine.
            </p>
            <p>
                I'm attending the University of Denver Full Stack Bootcamp program and am hoping to land my first job as a web developer.
            </p>

        </article>

    </section>
    <section id="work">

        <Projects />
    </section>
    <section id="data">

            <h6>Thanks for checking out my portfolio, As you can probably tell, I'm still working on it. You can reach me at ericlake@me.com</h6>

            <WorkInfo />
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

    #data{
        position: relative;
    }

    .yeller{

        box-sizing: border-box;
        border-radius: 10px;
        background-color: #FFD23F;
        padding: 2rem;
        width: 90%;
        max-width: 500px;
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
        font-size: clamp(2rem, 2rem + 5vw, 5rem);
        text-align: left;
        line-height: 1em;
        margin: 0rem auto;
        max-width: 800px;
    }

    h6{
        width: 90%;
        margin: 0 auto;
    }

    p{
        width: 100%;
        max-width: 800px;
        font-weight: 300;

    }


#work{
    position: relative;
}




@media only screen and (min-width: 500px) {
    .container{
        scroll-behavior: smooth;
    }
}



</style>