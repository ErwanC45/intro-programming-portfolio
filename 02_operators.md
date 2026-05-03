Section 1 - Concept of Operators

An operator is a symbol used to perfom operations on values or variables. 
There are four categories of operators. The arithmetic operators (/, * , -, +, %) are used to perform calculations while the relational operators (>, <, ==, !=, >=, <=) are used to compare variables or values (operands) turning them into a simple boolean expression (true or false).
We also have logical operators (&& (AND), || (OR), !(NOT)) to combine multiple boolean expressions (operands) to create conditions, and finally the assignment operator (=) used to assign a value to a variable.

There is also "Bitwise and shift operators", but we didn't learn them in class.

It's also important to know the precedence of operators in complex expressions: 
First arithmetic operators (with usual arithmetic precedence), then relational (first >, <, >=, <= then == and !=), logical operators (&&, ||, !) and finally assignment operator (=). 


Section 2 - Syntax

Arithmetic + assignment operator example: 
int a = 3 + 7;  --> First "+" adds 7 to 3, giving 10, and then "=" gives the value of 10 to the variable "a" of integer type.

Relational operators example: 
a % 2 == 0 --> evaluates to true if a is an even number.

Logical example: 
(a % 2 == 0) && (a >= 0 && a < 10) --> evaluates to true if a is an unsigned digit and is even.


Section 3 - Eureka moment

I don't really recall having big difficulties with this concept, but I needed to work on the operator precedence. To be sure that my program works as intended, I used to put too much parenthesis but after practicing I integrated the precedence and got rid of useless parenthesis.

Section 4 - Common beginner mistake

I think my most common mistake was mistaking the assignment operator "=" with the equality one "==" when trying to compare operands. I think it happened because outside programming (for example is basic arithmetics) we use "=" to say that for example "x" equals "y".


Section 5 - Research references

- Classes and assignments
- https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/
- https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/#operator-precedence
