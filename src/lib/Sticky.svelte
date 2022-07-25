  
  
  <article class="proj">
    <h3>
      <slot name="title">
        <span class="missing">Unknown Title</span>
      </slot>
    </h3>

    <div class="Links">
      <slot name="github">
        <a href="http://ericallenlake.com" class="missing" >Unknown Link</a>
      </slot>
      <slot name="live">
        <a href="http://ericallenlake.com" class="missing">Unknown Link</a>
      </slot>
    </div>

    <div class="description">
      <br>
      <slot name="description" >
      <code>
        <span class="missing">Lorem ipsum dolor sit amet consectetur adipisicing elit. </span>
      </code>
    </slot>
    </div>
    <div class="row">
      <div class="visual">
        <img class='screen' src="/images/placeholder-image.png" alt="">
      </div>




    </div>
    <div class="info-panel">
      <p>Technologies used: </p>
      <slot name="tech">
        <br><p class="missing">HTML, CSS, JavaScript, API</p>
         </slot>
    </div>
  </article>

  <style>

@import url('https://fonts.googleapis.com/css2?family=Rock+Salt&display=swap');

    .proj{
      height: calc(90vw - 2rem);
    max-height: 500px;
    aspect-ratio: 1;
    padding: 1rem;
    /* margin: 1rem; */
  /* block-size: 80%; */
  background-color: #ccf;
  box-shadow: 5px 5px 7px rgba(33,33,33,.7);
  margin: 1rem;
  position: relative;
    }

    .row{
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .info-panel{
      position: absolute;
      width: 100%;
      bottom: 0;
      left: 0;
      width: 100%;
      background-color: #ffd23ff6;
      padding: 1rem 0;
    }

    .info-panel p {
      margin: 0 0.4rem;
      line-height: 0.5rem;
      padding: 0;
    }

    .visual{
      justify-content: center;
      align-items: center;
      margin-top: 1rem;
      display: flex;
      border: 1px solid black;
      width: 30%;
    }

    .screen{
      width: 100%;
    }


  </style>