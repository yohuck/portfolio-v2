<svg class = 'one' viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <path fill="#70585a71" d="M41.5,-66.5C53.4,-56.8,62.5,-44.8,71.5,-30.9C80.5,-17.1,89.5,-1.5,89.7,14.5C90,30.5,81.4,46.8,69.1,58.3C56.7,69.8,40.6,76.5,24.1,80.8C7.6,85.1,-9.3,87,-24.6,83C-40,78.9,-53.9,68.8,-62.3,55.8C-70.8,42.8,-73.8,26.9,-75.1,11.4C-76.4,-4.1,-76,-19.3,-72,-34.9C-68.1,-50.5,-60.5,-66.5,-47.9,-75.8C-35.3,-85.2,-17.7,-87.9,-1.4,-85.7C14.8,-83.4,29.5,-76.2,41.5,-66.5Z" transform="translate(100 100)" />
</svg>


<svg class = 'two' viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <path fill=#cc626b71 d="M48.6,-61.5C63.4,-56.1,76.1,-42.5,74.2,-28.7C72.3,-15,55.7,-1.1,45.3,9.7C34.9,20.6,30.7,28.5,24.2,35.1C17.7,41.7,8.8,46.9,0,46.9C-8.9,47,-17.8,41.8,-24.7,35.4C-31.7,29,-36.6,21.2,-47.4,10.2C-58.2,-0.9,-74.8,-15.3,-73.9,-25.8C-73,-36.4,-54.6,-43,-39.3,-48.3C-24.1,-53.6,-12,-57.6,2.4,-60.9C16.9,-64.2,33.8,-67,48.6,-61.5Z" transform="translate(100 100)" />
</svg>

<svg class = "three" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <path fill="#beb8b971" d="M40.2,-67.1C52,-62.8,61.6,-51.9,68,-39.6C74.4,-27.4,77.7,-13.7,78.6,0.5C79.6,14.8,78.2,29.5,71.7,41.7C65.2,53.8,53.6,63.3,40.8,66.4C28,69.5,14,66.2,1.4,63.7C-11.1,61.2,-22.3,59.5,-32,54.7C-41.7,49.8,-50,41.7,-60.4,32.1C-70.8,22.5,-83.2,11.2,-84.6,-0.8C-85.9,-12.8,-76.2,-25.6,-67.7,-38.6C-59.3,-51.6,-52.2,-64.9,-41.2,-69.7C-30.1,-74.5,-15,-70.7,-0.4,-70C14.2,-69.2,28.3,-71.4,40.2,-67.1Z" transform="translate(100 100)" />
</svg>


<style>
  .one{
    /* transform: translateY(4rem) rotate(50deg) scale(40%); */
    position: absolute;
    z-index: 1;
    animation: move 10s ease-in-out infinite;
    color: #beb8b971;
    
}
  .two{
    /* transform: translateY(4rem) rotate(50deg) scale(40%); */
    position: absolute;
    z-index: 1;
    animation: move2 14s ease-in-out infinite;
    color: #62cc7971;
    
}
  .three{
    /* transform: translateY(4rem) rotate(50deg) scale(40%); */
    position: absolute;
    z-index: 1;
    animation: move2 40s ease-in-out infinite;
    color: #cc626b71;
    
}

@keyframes move {
  0%   { transform: scale(1) translate(-100%, 0%) rotate(0deg); }
  30%  { transform: scale(0.5) translate(30%, 50vh) rotate(); }
  100%  { transform: scale(1) translate(100%, 0%) rotate(360deg); }
}


@keyframes move2 {
  0%   { transform: scale(4) translate(50%, 0%) rotate(0deg); }
  30%  { transform: scale(0.5) translate(30%, 50vh) rotate(); }
  100%  { transform: scale(3) translate(-100%, 0%) rotate(360deg); }
}
@keyframes move3 {
  0%   { transform: scale(0.6) translate(10%, 40vh) rotate(0deg); }
  30%  { transform: scale(0.5, 2) translate(30%, 50vh) rotate(); }
  100%  { transform: scale(1) translate(100%, -40vh) rotate(-300deg); }
}

/* .two{
    transform: translateY(50rem) rotate(50deg) scale(40%);
} */



</style>