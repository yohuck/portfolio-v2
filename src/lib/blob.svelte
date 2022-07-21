<svg class = 'one' viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <path fill="#70585a71" d="M41.5,-66.5C53.4,-56.8,62.5,-44.8,71.5,-30.9C80.5,-17.1,89.5,-1.5,89.7,14.5C90,30.5,81.4,46.8,69.1,58.3C56.7,69.8,40.6,76.5,24.1,80.8C7.6,85.1,-9.3,87,-24.6,83C-40,78.9,-53.9,68.8,-62.3,55.8C-70.8,42.8,-73.8,26.9,-75.1,11.4C-76.4,-4.1,-76,-19.3,-72,-34.9C-68.1,-50.5,-60.5,-66.5,-47.9,-75.8C-35.3,-85.2,-17.7,-87.9,-1.4,-85.7C14.8,-83.4,29.5,-76.2,41.5,-66.5Z" transform="translate(100 100)" />
</svg>


<style>
  .one{
    /* transform: translateY(4rem) rotate(50deg) scale(40%); */
    position: absolute;
    z-index: 1;
    animation: move 20s ease-in-out infinite;
    color: #70585a71;
    
}

@keyframes move {
  0%   { transform: scale(0.3) translate(90%, 90%) rotate(0deg); }
  15%  { transform: scale(0.3) translate() rotate(); }
  30%  { transform: scale(0.3) translate() rotate(); }
  45%  { transform: scale(1, 0.3) translate() rotate(-900deg); }
  50%  { transform: scale(0.3) translate(-200%, -20%) rotate(-200deg); }
  85%  { transform: scale(0.3) translate(90%, -90%) rotate(200deg); }
  100%  { transform: scale(0.3) translate(90%, 90%) rotate(0deg); }
}

/* .two{
    transform: translateY(50rem) rotate(50deg) scale(40%);
} */



</style>