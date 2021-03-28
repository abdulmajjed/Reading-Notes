Operators and Loops.
*/
== is equal to مساوية تماما? 
!= is not equal ?
=== strict equal to ?
!==strict nott equal to
> greaterr than
< les than
>= greater than  or equal to
<= less than or equal to 
----
&& logical and  -> test more than one ccondition               ((2<5)&&(3>=2)) True 
|| lkogical or  -> test at least one condition                 ((2<5)||(3>=2)) True
! logical not   -> take a single boolean value and invert it   !(2<1)  true
_____________________________________________
form structure Of LOGICCAL OPERATORS
<from> : This element should always carry the actionattribute and will usually have a method and id attribute too.
<input> : its used to create several different form controls
<form action="http://www.example.com/login.php">
<p>Username:
 <input type="text" name="username" size="15" 
 maxlength="30" />
</p>
<p>Password:
 <input type="password" name="password" size="15"
 maxlength="30" />
</form>
-------------------------
checkbox

<form action="http://www.example.com/profile.php">
<p>select the button:
 <br />

<input type="checkbox" name="service" 
 value="example" checked="checked" /> example
----------------------
Drop Down List Box

<select> : is used to create a drop down list box.
<select name="examples">
 <option value="ex1">ex1</option>
 <option value="ex2">ex2</option>
 <option value="ex3">ex3</option>
 </select>
______________________________________________________
loops for&while

for will repet untel to got the right answer for condition
for (var i =0; i<10;i++){ document.write(i); }
*/