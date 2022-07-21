  
  
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
  </style>