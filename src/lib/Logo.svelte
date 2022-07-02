<div class="center">
    <div class="patch">
      <div class="background">
        <div class="foreground">
          <h3 id='eric'>ERIC</h3>
          <h3>LAKE</h3>
          <p>creative developer</p>
        </div>
      </div>
    </div>
</div>

<style>
    * {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}




.center {
  /* height: 100vh; */
  display: flex;
  justify-content: center;
  align-items: center;
  /* background-color:#90CAF9; */
/*     background-color: #e5e5f7; */
/* opacity: 0.8;
background-size: 10px 10px;
background-image: repeating-linear-gradient(50deg, #444cf7 0, #444cf7 1px, #B2CAE9 0, #29B6F6 50%); */
  
}


.foreground{
  width: 200px;
  height: 200px;
  background-color:#0761d1ff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-family: sans-serif;
  border-radius: 9px;
  margin: 0.4rem;
  opacity: 1;
background-size:10px 10px;
background-image: repeating-linear-gradient(45deg, rgba(5, 18, 35, 0.7) 0, rgb(56, 38, 48) 4px, #B2CAE9 0, #29B6F6 5%);
}

.foreground h3 {
  color: #FFC107 ;
  font-size: 3rem;
  -webkit-text-stroke: 2px #204f65 ;
  letter-spacing: 0.3rem;
  line-height: 3rem;
}

.foreground p{
  font-family:monospace;
  font-weight: 900;
  letter-spacing: 0.09rem;
  color: #ffffffff;
}

.background {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #FFC107;
  border-radius: 9px;
  border: 4px dotted #FFF9C4;
  margin: 0.2rem;
}

#eric {
  letter-spacing: 0.60rem;
}


.patch {
  background-color: #EEEEEE;
  display: flex;
  border-radius: 20px;
  border: 4px dotted #FFF9C4;
  margin: 1rem;
}
</style>