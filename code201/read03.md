Duckett HTML book:

Chapter 3: “Lists”

Ordered Lists < ol>
< li> come inside < ol> to order the list.

Unordered Lists < ul> 
< li> come inside < ul> to unorder the list.

Definition Lists < dl> < dt> < dd>

Nested Lists  ul>li( nested)>li( 0nested)>ul>li 

 -------------------------

Chapter 13: “Boxes”

Box Dimensions
width, height

Limiting Width
min-width, 
max-width 

Limiting Height
min-height, 
max-height

Overflowing Content
hidden
scroll
< p class="one"> 
p.one {
overflow: hidden;}

Border Width

thin
medium
thick

< p class="one">   
p.one {
border-width: 2px;}

Border Style
html < p class="one">Wurlitzer Electric Piano</ p>
 
css
p.one {border-style: solid;}
p.two {border-style: dotted;}
p.three {border-style: dashed;}
p.four {border-style: double;}
p.five {border-style: groove;}
p.six {border-style: ridge;}
p.seven {border-style: inset;}
p.eight {border-style: outset;}

Border Color
< p class="one"> 
p.one {
border-color: #0088dd;}

Change Inline/Block
html
< ul>
< li>Home</ li>
< li>Products</ li>
< li class="coming-soon">Services</ li>
< li>About</ li>
< li>Contact</ li>
</ ul>

css
li {
display: inline; 
margin-right: 10px;}
li.coming-soon {
display: none;}


CSS3: Elliptical Shapes

< p class ="one"></ p>
p.one {
border-top-left-radius: 80px 50px;
-moz-border-radius-top-left: 80px 50px;
-webkit-border-radius-top-left: 80px 50px;}

______________________________________________________________
Duckett JS book: 

Chapter 2: “Basic JavaScript Instructions”

ARRAYS An array is a special type of variable. It doesn't  just store one value; it stores a list of values. 
CREATING AN ARRAY 
var colors; 
colors ['white', 'black', ' custom']; 
var el document.getElementByld('col ors'); 
el . textContent = col ors[O];

II Create the array 
var colors = ['white', 
'black' , 
'custom']; 
c02/ js/ update-array.js 
II Update the third item in the array 
colors[2] = 'beige ' ; 
II Get the element with an id of col ors 
var el = document .getElementByid(' colors') ; 
II Replace with third item from the array 
el .textContent = colors[2]; 
-----------------------
Chapter 4: “Decisions and Loops” from switch statements on


#Switch statement.

let vairable=promt(qustion or condition);

switsh(variable){
case 'value1':
    do code...;
    break;

case 'value2';
    do code...;
    break;
  
default:
do code...;
break;

--------------
#while loop

le  i= 0;
while(i<9, i++){
console.log(pass)};


