Section 1 - Concept Switch statement

The switch statement is quite similar to the if statement, but instead of using boolean expressions as conditions, it uses the value of a variable or an expression by giving different possible paths (cases) based on this value. Unlike if statement, switch statement can only be used with int, char and string.
First the expression is evaluated, and then it is compared with the values of each case. If there is a match, the block of code associated is executed.
The default case acts similarly as the "else" in if statement, if there is no match, it's the default case that is executed.
Note that since all cases are enclosed in the same scope (curly brackets), after executing the block of code of the matching case, a "break;" is needed to break out
of the switch statement. It also means that like the if statement, only one matching case can be executed. 


Section 2 - Syntax

switch (expression)

{

  case x:

  // code block

  break;
    
  case y:
  
  // code block
    
  break;
  
  default:
  
  // code block
  
  break;
  
}

Example :

int d = 5;

switch (d)

{

  case 1:
  
  Console.WriteLine("Monday");
    
  break;
    
  case 2:
  
  Console.WriteLine("Tuesday");
    
  break;
    
  case 3:
  
  Console.WriteLine("Wednesday");
    
  break;
    
  case 4:
  
  Console.WriteLine("Thursday");
    
  break;

  case 5:
  
  Console.WriteLine("Friday");
    
  break;
    
  case 6:
  
  Console.WriteLine("Saturday");
    
  break;
    
  case 7:
  
  Console.WriteLine("Sunday");
    
  break;

  default:

  Console.WriteLine("Wrong entry");

  break;
  
}

Section 3 - Eureka moment

It was a bit hard at first to understand when it was better to use a switch statement instead of an if statement. Once I understood that switch statement is 
all about comparing a simple variable value to an according case, it became clearer and the exercise 9 of Assignment 4 (switch menu) helped me understand that.


Section 4 - Common beginner mistake

I think that the most common mistake I made was forgetting the "break;" after a case, resulting in a compiling error and preventing the program to run.
Since it's not necessary in the if statement, I had to take on the habit. 

Section 5 - Research references

https://www.w3schools.com/cs/cs_switch.php

https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/statements/selection-statements#the-switch-statement
