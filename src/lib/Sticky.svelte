  
  
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
        <a href="http://ericallenlake.com" class="msising">Unknown Link</a>
      </slot>
    </div>

    <div class="description">
      <br>
      <code>
        <span name="description" class="missing">Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae repellat nulla, distinctio quasi reiciendis sint quae beatae tempore sapiente vitae nobis dolor neque eaque excepturi similique repudiandae eius necessitatibus natus.</span>
      </code>
    </div>
    <div class="visual">
      <img class='screen' src="/images/placeholder-image.png" alt="">
    </div>

    <h5>Technologies used:
      <slot name="tech">
         <br><span class="missing">HTML, CSS, JavaScript, API</span>
      </slot>
    </h5>

  </article>

  <style>
    .proj{
      height: calc(90vw - 2rem);
    max-height: 500px;
    aspect-ratio: 1;
    padding: 1rem;
    /* margin: 1rem; */
  /* block-size: 80%; */
  background-color: rgb(214, 160, 245);
  box-shadow: 5px 5px 7px rgba(33,33,33,.7);
  margin: 1rem;
    }

    .visual{
      margin-top: 1rem;
      display: flex;
      border: 1px solid black;
      width: 50%;
    }

    .screen{
      width: 100%;
    }
  </style>