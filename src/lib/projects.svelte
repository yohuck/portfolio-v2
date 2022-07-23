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
    <span slot="title">Recycle Better</span>
    <a href="https://yohuck.github.io/wish-cycle/" slot="github" >GitHub Repository</a>
    <a href="https://yohuck.github.io/wish-cycle/" slot="live">Live Site</a>
  </Sticky>
  <Sticky></Sticky>
  <Sticky></Sticky>
  <Sticky></Sticky>
  <Sticky></Sticky>
  <div class="proj"><p>This is four</p></div>
  <div class="proj"><p>This is five</p></div>
  <div class="proj"><p>This is siz</p></div>
  <div class="proj"><p>This is seven</p></div>
  <div class="proj"><p>This is eight</p></div>
</div>
<style>
     .scrollport::-webkit-scrollbar{
  display: none;
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


</style>