<script>
import Sticky from './Sticky.svelte'
let box;

let isDown = false;
let starting;
let ending;
let moved;

  const scrollPosition = (e) => {
    if (isDown == true) {
      console.log(e.clientX)
      console.log(box.scrollLeft)
      box.scrollLeft = moved ? moved + ( (starting-e.clientX)*1.4 ) : (starting-e.clientX)*1.4
    } else return
  }

  const startMoving = (e) => {
    moved = box.scrollLeft
    starting = e.clientX
    isDown = true;
    console.log(isDown)
    box.style.cursor = '-webkit-grabbing'
  }

  const stopMoving = (e) => {

    ending = e.clientX;
    moved = starting-ending
    isDown = false;
    console.log(isDown)
    box.style.cursor = 'pointer'
  }







</script>

<h2>Check out my work!</h2>

<div class="scrollport"
on:mousedown="{startMoving}"
on:mousemove="{scrollPosition}"
on:mouseup="{stopMoving}"
bind:this={box}>



  <Sticky>
    <span slot="title">Habit Stack</span>
    <a href="https://github.com/yohuck/habit-map" slot="github" target="_blank">GitHub Repository</a>
    <a href="https://habitstack.herokuapp.com/" slot="live" target="_blank">Live Site</a>
    <span slot="description" class="description">A simple and satisfying full-stack habit tracking tool that utilizes a custom CSS/JavaScript data visualization. <br> Check out my walkthrough video over there  <span class="pointer">👉</span></span>
    <p slot="tech" >Node.Js, Handlebars, Express, Sequelize, Custom CSS</p>
    
  </Sticky>
  <div class="proj">
    <div class="row">
      <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:ugcPost:6965074918954741760?compact=1" height="399" width="710" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>
    </div>
  </div>
  <Sticky>
    <span slot="title">Recycle Better</span>
    <a href="https://github.com/yohuck/wish-cycle" slot="github" target="_blank" >GitHub Repository</a>
    <a href="https://yohuck.github.io/wish-cycle/" slot="live" target="_blank">Live Site</a>
    <span slot="description" class="description">A mobile-first application to help conscious consumers quickly and easily find out whether household items are recyclable and how/where to properly dispose of those items.</span>
 
  </Sticky>
  <Sticky></Sticky>
  <Sticky></Sticky>
  <Sticky></Sticky>
  
  <div class="proj"><p>This is five</p></div>
  <div class="proj"><p>This is siz</p></div>
  <div class="proj"><p>This is seven</p></div>
  <div class="proj"><p>This is eight</p></div>
</div>
<style>


@import url('https://fonts.googleapis.com/css2?family=Nothing+You+Could+Do&display=swap');

     .scrollport::-webkit-scrollbar{
  display: none;
}

.description{
  font-size: 1rem;
}

iframe{
  max-width: 100%;
  max-height: 100%;
}




.scrollport{
    cursor: grab;


    height: calc(100vw - 2rem);
    max-height: 600px;
    width: 100%;
    max-width: 100vw;
    overflow-x: auto;
    /* overscroll-behavior-x: contain; */
    display: flex; 
    flex-direction: row; 
    /* gap: 2rem; */
    align-items: center;
    justify-content: start;
    /* border: 1px solid green */
}


.proj {
    height: calc(90vw - 2rem);
    max-height: 500px;
    aspect-ratio: 1;
    padding: 1rem;
    /* margin: 1rem; */
  /* block-size: 80%; */
  background-color: #ccf;
  box-shadow: 5px 5px 7px rgba(33,33,33,.7);
  margin: 1rem;
}

.proj + .proj {
    margin-left: 1rem;
}

a{
  font-size: 0.8rem;
}

.row{
  background-color: black;
  height: 100%;
  display: grid;
  place-items: center;
  overflow: hidden;
}



p {
      font-size: 1rem;
      margin: 0rem 1rem;
      line-height: 1rem;
      padding: 0;
    }






</style>