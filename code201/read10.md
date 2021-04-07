JavaScript book,
 Ch. 10, “Error Handling & Debugging”
-THE CONSOLE & DEV TOOLS
1. Tools built into the browser 
that help you hunt for errors. 
-COMMON PROBLEMS
1. Common sources of errors, 
and how to solve them.
-HANDLING ERRORS 
1. How code can deal with 
potential errors gracefully. 
---
# ORDER OF EXECUTION
1. To find the source of an error, it helps to know how scripts are processed. 
The order in which statements are executed can be complex; some tasks 
cannot complete until another statement or function has been run: 
# EXECUT.ION CONTEXTS
1. The JavaScript interpreter uses the concept of execution contexts. 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope. 
A. EXECUTION CONTEXT 
1. GLOBAL CONTEXT 
2. FUNCTION CONTEXT
3. EVAL CONTEXT NOT SHOWN 

B. VARIABLE SCOPE
1. GLOBAL SCOPE
2. FUNCTION-LEVEL SCOPE
------------
# FUNCTION-LEVEL SCOPE
1: PREPARE
• The new scope is created 
• Variables, functions, and arguments are created 
• The value of the this keyword is determined
2: EXECUTE 
• Now it can assign values to variables 
• Reference functions and run their code 
• Execute statements 
# UNDERSTANDING SCOPE
1. In the interpreter, each execution context has its own va ri ables object. 
It holds the variables, functions, and parameters available within it. 
Each execution context can also access its parent's v a ri ables object. 
#UNDERSTANDING ERRORS 
1. If a JavaScript statement generates an error, then it throws an exception. 
At that point, the interpreter stops and looks for exception-handl ing code
#ERROR OBJECTS
1. Error objects can help you find where your mistakes are 
and browsers have tools to help you read them. 
#ERROR OBJECTS CONTI NUED 
1. Syntax Error 
2. Ref erenceError
3. Ev alError 
4. UR I Error
5. Type Error
6. RangeError 
7. Error 
8. NaN
# HOW TO DEAL WITH ERRORS 
1. Now that you know what an error is and how the browser treats them, 
there are two things you can do with the errors. 
1. 1: DEBUG THE SCRIPT TO FIX ERRORS
2. 2: HANDLE ERRORS GRACEFULLY
#A DEBUGGING WORKFLOW 
Debugging is about deduction: eliminating potential causes of an error. 
Here is a workflow for techniques you will meet over the next 20 pages. 
Try to narrow down where the problem might be, then look for clues
1. WHERE IS THE PROBLEM? 
1. Look at the error message, it tells you: 
• The relevant script that caused the problem. 
• The line number where it became a problem for 
the interpreter. As you will see, the cause of 
the error may be earlier in a script; but this is the 
point at which the script could not continue. 
• The type of error although the underlying cause 
of the error may be different. 
2. Check how far the script is running. 
Use tools to write messages to the console to tell 
how far your script has executed. 
3. Use breakpoints where things are going wrong. 
They let you pause execution and inspect the values 
that are stored in variables
2.WHAT EXACTLY IS THE PROBLEM?
1. When you have set breakpoints, you can see if the 
variables around them have the values you would 
expect them to. If not, look earlier in the script. 
2. Break down I break out parts of the code to test 
smaller pieces of the functionality. 
• Write values of variables into the console. 
• Calrfunctions from the console to check if they 
are returning what you would expect them to. 
• Check if objects exist and have the methods I 
properties that you think they do. 
3. Check the number of parameters for a function, or 
the number of items in an array.
# BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 
1.The JavaScript console will tell you when there is a problem with a script, 
where to look for the problem, and what kind of issue it seems to be.
1. 1 CHROM E/ OPERA
On a PC, press the F12 key or: 
1. Go to the options menu or three line menu icon 
2. Select Toots or More tools. 
3. Select JavaScript Console or Developer Tools 
On a Mac press Alt + Cmd + J. Or: 
4. Go to the View menu. 
5. Select Developer. 
6. Open the JavaScript Console or Developer Tools 
option and select Console.
#HOW TO LOOK AT ERRORS IN CHROME 
1. 1 The console will show you when there is an 
error in your JavaScript. It also displays the line 
where it became a problem for the interpreter. 
#MORE CONSOLE METHODS 
1. con so 1 e. info can be used 
for general information 
2. consol e.warn can be used 
for warnings 
3. console .er ror can be used 
to hold errors
# GROUPING MESSAGES
1. If you want to write a set of 
related data to the console, you 
can use the console. group  
method to group the messages 
together. You can then expand 
and contract the results. 
2. When you have finished 
writing out the results for the 
group, to indicate the end of the 
group the console .groupEnd  
method is used. 
# WRITING TABULAR DATA 
# WRITING ON A CONDITION
1.  when users leave an 
input, the code checks to see if 
they entered a value that is 10 
or higher. If not, it will write a 
message to the screen. 
2. The second check looks to 
see if the calculated area is a 
numeric value. If not, then the 
user must have entered a value 
that was not a number
#BREAKPOINTS
1. You can pause the execution of a script on any 
line using breakpoints. Then you can check the 
values stored in variables at that point in time. 
1. 1 CHROME 
1. Select the Sources option. 
2. Select the script you are 
working with from the left-hand 
pane. The code will appear to 
the right. 
3. Find the line number you want 
to stop on and click on it. 
4. When you run the script, it 
will stop on this line. You can 
now hover over any variable to 
see its value at that time in the 
script's execution.
#STEPPING THROUGH CODE 
1. A pause sign shows until the interpreter comes across a breakpoint. 
When the interpreter stops on a breakpoint, a play-style button is then 
shown. This lets you tell the interpreter to resume running the code. 
2. Go to the next line of code and step through the lines one-by-one 
rather than running them as fast as possible. 
3. Step into a function call. The debugger will move to the first line in 
that function. 
4. Step out of a function that you stepped into. The remainder of the 
function will be executed as the debugger moves to its parent function.
# CONDITIONAL BREAKPOINTS 
1. You can indicate that a breakpoint should be 
triggered only if a condition that you specify is 
met. The condition can use existing variables. 
1.1 CHROME 
1. Right-click on a line number. 
2. Select Add Conditional 
Breakpoint... 
3. Enter a condition into the 
popup box. 
4. When you run the script, it 
will only stop on this line if the 
condition is true e.g., if area is 
less than 20
# DEBUGGER KEYWORD
1. You can create a breakpoint 
in your code using just the 
debugger keyword. When the 
developer tools are open, this 
will automatically create a 
breakpoint
# HANDLING EXCEPTIONS 
1. If you know your code might fail, use try, catch, and finally. 
Each one is given its own code block. 
# THROWING ERRORS
1.  If you know something might cause a problem for your script, you can 
generate your own errors before the interpreter creates them.
# THROW ERROR FOR NaN 
1. If you try to use a string in a 
mathematical operation other 
than in addition, you do not get 
an error, you get a special value 
called NaN not a number. 
# DEBUGGING TIPS 
1. Here are a selection of practical tips that you 
can try to use when debugging your scripts. 
1. 1 ANOTHER BROWSER
1. 2 SEARCH 
1. 3 VALIDATION TOOLS 
1. 4 ADD NUMBERS
1. 5 CODE PLAYGROUNDS 
1. 6 STRIP IT BACK
1. 7 EXPLAINING THE CODE 


