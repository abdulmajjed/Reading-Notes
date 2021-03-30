Ch.4 “Links”

Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.
Writing Links < a href=" url " > < / a >

Directory Structure :
Structure => The diagram on the right shows 
the directory structure for a fictional entertainment listings website called ExampleArts. 

Relationships => The relationship between 
files and folders on a website is described using the same terminology as a family tree.  

Homepages => 
The main homepage of a site 
written in HTML and the homepages of each section in a child folder is called index . html .

-----
Relative Link Type :
Same Folder => To link to music reviews from the music homepage:
< a href="reviews.html ">Reviews< /a>

Child Folder => To link to music listings from the homepage:
< a href=  "music/listings.html"> Listings< /a>

Grandchild Folder => To link to DVD reviews from the homepage:
< a href="movies/dvd/reviews.html">
Reviews< /a>

Parent Folder => To link to the homepage from the music reviews:
< a href="../index.html">Home< /a> 


GrandParent Folder => To link to the homepage from the DVD reviews:
< a href="../../index.html">Home< /a>

Email Links mailto:  < a href="mailto:jon@example.org">Email Jon< /a>

Opening Links in a New Window target 
< a href="http://www.imdb.com" target ="_blank">
Internet Movie Database< /a>

Linking to a Specific Part of the Same Page: id =
--------------
Chapter 15: “Layout” 

X Controlling the position of elements
Key Concepts in Positioning Elements
Block-level elements
start on a new line ; Examples include:
< h1>  < p> < ul> < li>

Inline elements
flow in between 
surrounding text
Examples include:
< img> < b> < i>

X Containing Elements 
Normal flow  Relative Positioning 
Creating site layouts  Absolute positioning   Fixed Positioning    Fixed Positioning 

Normal Flow            position:static 
Relative Positioning   position:relative 
Absolute Positioning   position:absolute
Fixed Positioning      position:fixed 
Overlapping Elements   z-index
Floating Elements      float
Clearing Floats        clear atc...

X Designing for different sized screens
A Fixed Width Layout : To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too).
A Liquid Layout   :   The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen.

------------------------------------
Duckett JS book: 

Chapter 3 first part: “Functions, Methods, and Objects”

WHAT IS A FUNCTION? Functions let you group a series of statements together to perform a specific task. I
A BASIC FUNCTION 
1. declaring a function
document . write  'hello! '  ;
2. calling a function 
sayHello  ;
3. declaring functions that need information 
return getArea width, height 
return width * height ;

4. calling functions that need information 
function calculateArea  W , H  
var  area = W * H ;
retuen area;

5. gtetting multiple values out of a function

----



