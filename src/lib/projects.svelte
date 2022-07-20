<script>
let box;

let isDown = false;
let starting;
let ending;
let moved;

  const scrollPosition = (e) => {
    if (isDown == true) {
      console.log(e.clientX)
      console.log(box.scrollLeft)
      box.scrollLeft =  starting-e.clientX
    } else return
  }

  const startMoving = (e) => {
    starting = e.clientX
    isDown = true;
    console.log(isDown)
  }

  const stopMoving = (e) => {

    ending = e.clientX;
    moved = starting-ending
    isDown = false;
    console.log(isDown)
  }


let test = '500px';




</script>


<div class="scrollport"
on:mousedown="{startMoving}"
on:mousemove="{scrollPosition}"
on:mouseup="{stopMoving}"
scrolLeft = "{test}"

bind:this={box} 

>
  <div class="proj" id="one"><p>This is one</p></div>
  <div class="proj" id="two"><p>This is two</p></div>
  <div class="proj" id="three"><p>This is three</p></div>
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


    height: calc(90vw - 2rem);
    max-height: 550px;
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