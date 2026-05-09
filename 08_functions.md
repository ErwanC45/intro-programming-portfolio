Section 1 - Concept of Functions

A function (also named method) is a specific named block of code. A function can either be already built-in the language, or can be made by the user. This is very useful to prevent hard coding and rewriting parts of code used multiple times. There are two different steps regarding function. The first one is the definition, the other one is the call.
First we need to define the function: we need the name of the function, the parameters it takes, the return type and finally the body (the code it will execute).
The name must be written in pascal case notation, and start with a verb indicating what the function does.
The parameters are the variables used by the function. We need the parameters types and names.
The return type is the type of variable value that will be "produced" by the function, if the function does produce a value. If it doesn't (for example it just prints something), we use the return type "void".
In the body of the definition, we need to use "return" followed by the value we want to return (or just return; if of void type) to take the value out of the scope and exit it. 
By convention, we define all the functions at the end of the script.
Once the function is defined, we can use it by calling it. To call a function, we need the name and the actual parameters (arguments).

Section 2 - Syntax

Definition:

returnType FunctionName (parameter1Type parameter1Name, parameter2Type parameter2Name,...) // this is called the header

{

// block of code (function body)

}

Call:

FunctionName (argument1,argument2,...)

Example:

Console.WriteLine(AddTwoNumbers (3, 5)); // will print 8

int AddTwoNumbers (int num1, int num2)

{

  return num1+num2;

}

Section 3 - Eureka moment

Overall I didn't have big difficulties with function specifically, since it's mainly about writing the definition using the others concepts we learnt before. However, I remember in Assignment 9 exercise 2 where we had to define many functions, I often forgot the return for every possible path, not just for the "good one". 

Section 4 - Common beginner mistake

In the header definition, using the wrong return type, because it requires to think about what we want the function to return. This would throw a compile error.

Section 5 - Research references

https://www.w3schools.com/cs/cs_methods.php
