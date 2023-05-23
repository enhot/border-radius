# border-radius
Use DOM for created Border-Radius CSS JS
jS

let r1 = document.querySelector('.rt1'),
    r2 = document.querySelector('.rt2'),
    r3 = document.querySelector('.rt3'),
    r4 = document.querySelector('.rt4'),
    t1 =document.querySelector('.tt1'),
    t2 =document.querySelector('.tt2'),
    t3 =document.querySelector('.tt3'),
    t4 =document.querySelector('.tt4');
   let bl = document.querySelector('.block');

function addSomeEvent() {
    r1.addEventListener('input', ()=>{
        t1.value = r1.value;
        bl.style.borderTopLeftRadius = r1.value +'px';
    })
    r2.addEventListener('input', () =>{
        t2.value = r2.value;
        bl.style.borderTopRightRadius = r2.value +'px'
    })
    r3.addEventListener('input', () =>{
        t3.value = r3.value;
        bl.style.borderBottomLeftRadius = r3.value +'px'
    })
    r4.addEventListener('input', ()=> {
        t4.value = r4.value;
        bl.style.borderBottomRightRadius = r4.value +'px'
    })
}
addSomeEvent()

HTML 
<h1>Code our</h1>
<div>
  <p> Верхний левый угол
    <input type="range" min="0" max="100" value="0" class="rt1">
    <input class="tt1" type="text" value="0">
  </p>
  <p> Верхний правый угол
    <input type="range" min="0" max="100" value="0" class="rt2">
    <input type="text" class="tt2" value="0">
  </p>
  <p> Нижний левый угол
    <input type="range" min="0" max="100" value="0" class="rt3">
    <input type="text" class="tt3" value="0">
  </p>
  <p> Нижгий правый угол
    <input type="range" min="0" max="100" value="0" class="rt4">
    <input type="text" class="tt4" value="0">
  </p>
</div>
<div class="block"></div>
