let boxOfBoxes = document.querySelector('#boxOfBoxes');
let boxes = document.querySelectorAll('.box');
let rows = document.querySelectorAll('.row');


function rainbow(){
  let r = Math.floor(Math.random() * 256);
  let g = Math.floor(Math.random() * 256);
  let b = Math.floor(Math.random() * 256);
  
  return "rgb("+r+","+g+","+b+")";
}







  
  

function removeGrid(){
  let rows = Array.from(document.getElementsByClassName('row'));
  for(i = 0; i < rows.length; i++){
    rows[i].remove();    
  }
}








const reset = document.querySelector('#reset');
reset.addEventListener('click', toggly);
function toggly(){
  gridSize = prompt('what\'s next?');
  removeGrid();
  newGrid(gridSize);
 
 };


function newGrid(gridSize){
  
  let newRow;
  let newBox;
  for(i = 0; i < gridSize; i++){
    let rowdiv = document.createElement('div');
    newRow = boxOfBoxes.appendChild(rowdiv);
    newRow.classList.add('row');
    for(j = 0; j < gridSize; j++){
      let boxdiv = document.createElement('div');
      newBox = newRow.appendChild(boxdiv);
      newBox.classList.add('box');
      
    }
    
  }
  let boxes = document.querySelectorAll('.box');
  boxes.forEach(box => {box.addEventListener('mouseover', () =>
                   box.style.backgroundColor = rainbow())});
}