Section 1 - Concept of nested loops.

A loop placed inside another loop is called a nested loop. The loop inside is called inner loop and the loop outside outer loop. Each loop will serve its own purposes. For one iteration of the outer loop, all possible iterations of the inner loop will occur. The total number of iterations equals the outer loop count (usually variable i) multiplied by the inner loop count (usually variable j).  While we can use all types of loop in nested loops, it's most common to use for loops. Nested for loops are useful to create patterns and work with 2D arrays.

Section 2 - Syntax

for (statement1; statement2; statement3) // outer loop 

{

  // outer loop block of code

  for (statement1; statement2; statement3) // inner loop 

  {

  // inner loop block of code

  }

}

Example:
  
for (int i = 0; i < 3; i++)

{

  for (int j = 0; j < 3; j++)

  {

  Console.WriteLine($"This is outer loop iteration number {i+1} and inner loop iteration number {j+1}");

  }

}

Section 3 - Eureka moment

The main difficulty with nested loops is to keep track and control of what happens to be able to do what we intend. The best way to understand how a nested loop works is to trace it as we did in the assignment. Also the Patterns exercise in the Assignment 6 made me visualize and understand better how it works. 

Section 4 - Common beginner mistake

I think my most common mistake was mixing up i and j in the nested loops, as a result of an unclear understanding of the loop I was working on and/or bad program flow tracking. It resulted in wrong outputs and even sometimes infinite loops. 

Section 5 - Research references

https://www.w3schools.com/cs/cs_for_loop.php

Assignment sheet


