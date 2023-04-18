0x12. JavaScript - Warm up
JavaScript
JavaScript is used for many things. Here, you will use JavaScript for 2 reasons:

Scripting (same as we did with Python)
Web front-end
For the moment, and for learning all basic concepts of this language, we will do some scripting. After, we will make our AirBnB project dynamic by using Javascript and JQuery.



Resources
Read or watch:

Writing JavaScript Code
Variables
Data Types
Operators
Operator Precedence
Controlling Program Flow
Functions
Objects and Arrays
Intrinsic Objects
Module patterns
var, let and const
JavaScript Tutorial
Modern JS
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

General
Why JavaScript programming is amazing
How to run a JavaScript script
How to create variables and constants
What are differences between var, const and let
What are all the data types available in JavaScript
How to use the if, if ... else statements
How to use comments
How to affect values to variables
How to use while and for loops
How to use break and continue statements
What is a function and how do you use functions
What does a function that does not use any return statement return
Scope of variables
What are the arithmetic operators and how to use them
How to manipulate dictionary
How to import a file


More Info
Install Node 14
$ curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
$ sudo apt-get install -y nodejs
Install semi-standard
Documentation

$ sudo npm install semistandard --global

Tasks
0. First constant, first print
mandatory
Write a script that prints “JavaScript is amazing”:

You must create a constant variable called myVar with the value “JavaScript is amazing”
You must use console.log(...) to print all output
You are not allowed to use var
JavaScript is amazing
     
1. 3 languages

Write a script that prints 3 lines:

The first line: “C is fun”
The second line: “Python is cool”
The third line: “JavaScript is amazing”
You must use console.log(...) to print all output
You are not allowed to use var
 
C is fun
Python is cool
JavaScript is amazing

     
2. Arguments
mandatory
write a script that prints a message depending of the number of arguments passed:

If no arguments are passed to the script, print “No argument”
If only one argument is passed to the script, print “Argument found”
Otherwise, print “Arguments found”
You must use console.log(...) to print all output
You are not allowed to use var
Reference: process.argv

argument
./2-arguments.js Best
Argument found
 ./2-arguments.js Best School
Arguments found

    
3. Value of my argument
write a script that prints the first argument passed to it:

If no arguments are passed to the script, print “No argument”
You must use console.log(...) to print all output
You are not allowed to use var
You are not allowed to use length
./3-value_argument.js 
No argument
 ./3-value_argument.js School
School
 
   
4. Create a sentence
mandatory

Write a script that prints two arguments passed to it, in the following format: “ is ”

You must use console.log(...) to print all output
You are not allowed to use var
./4-concat.js c cool
c is cool
~/0x12$ ./4-concat.js c 
c is undefined
/0x12$ ./4-concat.js
undefined is undefined
     
5. An Integer
mandatory

Write a script that prints My number: <first argument converted in integer> if the first argument can be converted to an integer:

If the argument can’t be converted to an integer, print “Not a number”
You must use console.log(...) to print all output
You are not allowed to use var
You are not allowed to use try/catch
 
Not a number
./5-to_integer.js 89
My number: 89
guillaume@ubuntu:~/0x12$ ./5-to_integer.js "89"
My number: 89
./5-to_integer.js 89.89
My number: 89
 ./5-to_integer.js School
Not a number
    
6. Loop to languages
mandatory

Write a script that prints 3 lines: (like 1-multi_languages.js) but by using an array of string and a loop

The first line: “C is fun”
The second line: “Python is cool”
The third line: “JavaScript is amazing”
You must use console.log(...) to print all output
You are not allowed to use var
You are not allowed to use any if/else statement
You can use only one console.log
You must use a loop (while, for, etc.)
./6-multi_languages_loop.js 
C is fun
Python is cool
JavaScript is amazing
guillaume@ubuntu:~/0x12$ 
     
7. I love C
mandatory

Write a script that prints x times “C is fun”

Where x is the first argument of the script
If the first argument can’t be converted to an integer, print “Missing number of occurrences”
You must use console.log(...) to print all output
You are not allowed to use var
You can use only two console.log
You must use a loop (while, for, etc.)
 ./7-multi_c.js 2
C is fun
C is fun
./7-multi_c.js 5
C is fun
C is fun
C is fun
C is fun
C is fun
./7-multi_c.js 
Missing number of occurrences
./7-multi_c.js -3
 
     
8. Square
mandatory

Write a script that prints a square

The first argument is the size of the square
If the first argument can’t be converted to an integer, print “Missing size”
You must use the character X to print the square
You must use console.log(...) to print all output
You are not allowed to use var
You must use a loop (while, for, etc.)

Missing size
 ./8-square.js School
Missing size
./8-square.js 2
XX
XX
 ./8-square.js 6
XXXXXX
XXXXXX
XXXXXX
XXXXXX
XXXXXX
XXXXXX
    
9. Add
mandatory

Write a script that prints the addition of 2 integers

The first argument is the first integer
The second argument is the second integer
You have to define a function with this prototype: function add(a, b)
You must use console.log(...) to print all output
You are not allowed to use var
guillaume@ubuntu:~/0x12$ ./9-add.js 
NaN
./9-add.js 1
NaN
 ./9-add.js 1 7
8
./9-add.js 13 89
102
 
     
10. Factorial
mandatory

Write a script that computes and prints a factorial

The first argument is integer (argument can be cast as integer) used for computing the factorial
Factorial of NaN is 1
You must do it recursively
You must use a function
You must use console.log(...) to print all output
You are not allowed to use var
 
1
./10-factorial.js 3
6
 ./10-factorial.js 89
1.6507955160908452e+136
 ./10-factorial.js 333
Infinity
 11. Second biggest!
mandatory

Write a script that searches the second biggest integer in the list of arguments.

You can assume all arguments can be converted to integer
If no argument passed, print 0
If the number of arguments is 1, print 0
You must use console.log(...) to print all output
You are not allowed to use var
guillaume@ubuntu:~/0x12$ ./11-second_biggest.js 
0
0
./11-second_biggest.js 4 2 5 3 0 -3
4
 
    
12. Object
mandatory

Update this script to replace the value 12 with 89:

You are not allowed to use var
 cat 12-object.js
#!/usr/bin/node
const myObject = {
  type: 'object',
  value: 12
};
console.log(myObject);
/*
YOUR CODE HERE
*/
console.log(myObject);

./12-object.js
{ type: 'object', value: 12 }
{ type: 'object', value: 89 }
 
     
13. Add file
mandatory

Write a function that returns the addition of 2 integers.

The function must be visible from outside
The name of the function must be add
You are not allowed to use var
Tip

cat 13-main.js
#!/usr/bin/node
const add = require('./13-add').add;
console.log(add(3, 5));
 ./13-main.js
8

    
14. Const or not const
#advanced

Write a file that modifies the value of myVar to 333


#!/usr/bin/node
myVar = 89;
require('./100-let_me_const')
console.log(myVar);
./100-main.js
333



Do you get it? Tweet! Post! Talk about it!

Hint: Scope

This exercise doesn’t pass semistandard so don’t worry about it.

   
15. Call me Moby
#advanced
Score: 56.88% (Checks completed: 87.5%)
Write a function that executes x times a function.

The function must be visible from outside
Prototype: function (x, theFunction)
You are not allowed to use var
 cat 101-main.js
#!/usr/bin/node
const callMeMoby = require('./101-call_me_moby').callMeMoby;
callMeMoby(3, function () {
  console.log('C is fun');
});
./101-main.js
C is fun
C is fun
C is fun
 
     
16. Add me maybe

Write a function that increments and calls a function.

The function must be visible from outside
Prototype: function (number, theFunction)
You are not allowed to use var
cat 102-main.js
#!/usr/bin/node
const addMeMaybe = require('./102-add_me_maybe').addMeMaybe;
addMeMaybe(4, function (nb) {
  console.log('New value: ' + nb);
});
 ./102-main.js
New value: 5
 
     
17. Increment object
#advanced

Update this script by adding a new function incr that increments the integer value.

You are not allowed to use var

#!/usr/bin/node
const myObject = {
  type: 'object',
  value: 12
};
console.log(myObject);
/*
YOUR CODE HERE
*/
myObject.incr();
console.log(myObject);
myObject.incr();
console.log(myObject);
myObject.incr();
console.log(myObject);

./103-object_fct.js 
{ type: 'object', value: 12 }
{ type: 'object', value: 13, incr: [Function] }
{ type: 'object', value: 14, incr: [Function] }
{ type: 'object', value: 15, incr: [Function] }
