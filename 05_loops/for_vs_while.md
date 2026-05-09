Section 1 - Concept of for and while loops

The while loop works similarly to the do-while loop. The main difference is that the condition is first checked, if it's true the program enters the block of code, then the condition is checked again. We need the condition to be evaluated to false to exit the loop. This also means that if the condition is false from the start, the program never enters the loop.

The for loop is a bit different than the do-while or while loops. This loop will "count" the iterations of the block of code, and will exit the loop if the count reaches a defined amount. It needs 3 statements. The first one will be executed first and one time (usually declaring and initializing the count variable). The second one will be the condition that will allow the program to enter the scope of the loop. The last one will be the incrementation of the count variable.
Once the count of iteration doesn't match the condition anymore, the program exits the loop.

The main difference between these two loops lies in the number of iterations you need. 
When you know how many iterations, use the for loop. When you don't know, use the while loop.


Section 2 - Syntax

While loop:

while (condition)

{

  // block of code

}

Example: 

int ans = 0;

int secretNum = 7;

while (ans != secretNum)

{

  Console.WriteLine("Try to find the secret number!");
  
  ans = Convert.ToInt32(Console.ReadLine());

}

For loop:

for(statement1; statement2; statement3)

{

  // block of code

}

Example:

for(int i=0; i < 6; i++)

{

  Console.WriteLine($"This is iteration number {i+1}")

}



Section 3 - Eureka moment

The use of these loops wasn't really hard, but the main difficulty was to choose the best loop for a given purpose. In the exercises of Assignment 5, I often picked the wrong loop. Reviewing the correction and practising made it easier to identify. I also ask myself if I can easily enumerate the number of iteration I need or not to know which loop I need. 

Section 4 - Common beginner mistake

As a common beginner mistake, I used to miswrite the statements in the for loop. For example using the wrong relational operator (<= instead of <) in the condition statement, or initializing i with 1 instead of 0. This often resulted in an off-by-one error.  

Section 5 - Research references

https://www.w3schools.com/cs/cs_while_loop.php

https://www.w3schools.com/cs/cs_for_loop.php
