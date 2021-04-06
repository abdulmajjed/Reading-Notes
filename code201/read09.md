 Forms and Events
---
From the Duckett HTML book:

*Traditionally, the term 'form' has referred 
to a printed document that contains 
spaces for you to fill in information

*The best known form on the web is probably 
the search box that sits right in the middle of 
Google's homepage.

Form Controls: 

1. ADDING TEXT:-Text input (single-line) -Password input -Text area (multi-line)
2. Making Choices:-Radio buttons - Checkboxes - Drop-down boxes 
3. Submitting Forms:-Submit buttons - Image buttons - File upload
4. Uploading Files: 

How Forms Work ??
A user fills in a form and then presses a button 
to submit the information to the server.

< p>Username:
 < input type="text" name="username" size="15" 
 maxlength="30" />
< /p>
< p>Password:
 < input type="password" name="password" size="15" 
 maxlength="30" />
< /p>
 
2.1 Radio Button :
< p>Please select your favorite genre:
 < br />
 < input type="radio" name="genre" value="rock" 
 checked="checked" /> Rock
 < input type="radio" name="genre" value="pop" /> 
 Pop
 < input type="radio" name="genre" value="jazz" /> 
 Jazz
< /p>
2.2 Checkbox : type="checkbox" 
2.3 Drop Down List Box : < select name="example" >
2.4 Multiple Select Box < select>
--
3.1 File Input Box : type="file"
3.2 Submit Button  : type="submit" 
3.3 Image Button   : type="image"
3.4 Button & hidden Controls  : type="hidden" 
----
Labelling Form Controls : < label>
Grouping Form  Elements : < fieldset> < legend>
---------------------------------------------------------------
Chapter 14: “Lists, Tables & Forms”

Bullet Point Styles list-style-type

Unordered Lists . none . disc . circle . square 
Ordered Lists  . decimal . decimal-leading-zero . lower-alpha . upper-alpha . lower-roman . upper-roman 
Images for Bullets list-style-image 
Positioning the Marker list-style-position . outside . inside
List Shorthand list-style 
Table Properties . width . padding . text-transform . letter-spacing, . font-size .border-top, border-bottom  . text-align background-color . :hover 
Border on Empty Cells empty-cells . show . hide . inherit
Gaps Between Cells  . font-size . color background-color . border  . border-radius : focus : hover   . background-image
Styling Submit Buttons 
Styling Fieldsets & Legends
Aligning Form Controls: Problem
Aligning Form Controls: Solution
Cursor Styles cursor
* Web Developer Toolbar 
1: Outlines 
2: Structure
3: CSS styles
-----------------------------------------------------
Duckett JS book:
Chapter 6: “Events”
EVENT DESCRIPTION 
load : Web page has finished loading 
unload : Web page is unloading (usually because a new page was requested) 
error : Browser encounters a JavaScript error or an asset doesn't exist 
resize : Browser window has been resized 
scroll : User has scrolled up or down the page 
KEYBOARD EVENTS:  Occur when a user interacts with the keyboard (see also input event) 
EVENT DESCRIPTION 
keydown : User first presses a key (repeats while key is depressed) 
keyup : User releases a key 
keypress : Character is being inserted (repeats while key is depressed) 
MOUSE EVENTS : Occur when a user interacts with a mouse. trackpad, or touchscreen 
EVENT DESCRIPTION 
click : User presses and releases a button over the same element 
dbl : click User presses and releases a button twice over the same element 
moused : own User presses a mouse button while over an element 
mouseup : User releases a mouse button while over an element 
mousemove : User moves the mouse (not on a touchscreen) 
mouseover : User moves the mouse over an element (not on a touchscreen) 
mouseout  : User moves the mouse off an element (not on a touchscreen) 
EVENT DESCRIPTION 
load W :eb page has finished loading 
unload :Web page is unloading (usually because a new page was requested) 
error :Browser encounters a JavaScript error or an asset doesn't exist 
resize :Browser window has been resized 
scroll :User has scrolled up or down the page 
KEYBOARD EVENTS:  Occur when a user interacts with the keyboard (see also input event) 
EVENT DESCRIPTION 
keydown: User first presses a key (repeats while key is depressed) 
keyup :User releases a key 
keypress: Character is being inserted (repeats while key is depressed) 
MOUSE :EVENTS Occur when a user interacts with a mouse. trackpad, or touchscreen 
EVENT DESCRIPTION 
click :User presses and releases a button over the same element 
dbl :click User presses and releases a button twice over the same element 
moused :own User presses a mouse button while over an element 
mouseup :User releases a mouse button while over an element 
mousemove :User moves the mouse (not on a touchscreen) 
mouseover :User moves the mouse over an element (not on a touchscreen) 
mouseout :User moves the mouse off an element (not on a touchscreen) 

---------
HOW EVENTS TRIGGER JAVASCRIPT CODE
1. Select t he element 
nodes you want the 
script to respond to. 
2. Select t he element 
nodes you want the 
script to respond to. 
3.State the code you want 
to run when the event 
occurs.

Here you can see how event handling can be used to provide feedback to 
users filling in a registration form. It will show an error message if their 
username is too short. 
1. SELECT ELEMENT :The element that users are 
interacting with is the text input 
where they enter the username. 
2. SPEC! FY EVENT : 
When users move out of the 
text input, it loses focus, and the 
blur event fires on this element.  
3. CALL CODE : When the blur event fires 
on the username input, it 
will trigger a function called 
chec kUsername .This function 
checks if the username is less 
than 5 characters. 




