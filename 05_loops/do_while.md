Section 1 - Concept of do-while loop

The do-while loop is a variant of the while loop that first executes a block of code, then checks a condition. If the condition is met (true), the loop continues and the block of code is executed again. Otherwise, if the condition isn't met (false), the program breaks out of the do-while loop and continues on the next line of code. Moreover, since the condition is checked at the end of the loop, it means that the block of code will be executed at least once. This type of loop is mainly used when we need to prompt the user for something and verify the answer.

Section 2 - Syntax

do

{

  // block of code

}

while (condition);

Example:

int ans;

do 

{

  Console.WriteLine("Please enter a number between 1 and 9");
  ans = Convert.ToInt32 (Console.ReadLine());

}

while (ans < 1 || ans > 9);

Section 3 - Eureka moment

What was confusing at first was the logic of the while condition. To keep the loop running, the condition must be true, and to break out, it must be false. This becomes counterintuitive because it means that to validate the user input, the answer must be "false" regarding the condition. I remember spending almost 2 hours
on this logical error during the midterm practice "B-Hive", but it helped me get a good grasp on this concept! 

Section 4 - Common beginner mistake

One common beginner mistake can be declaring the variable that need to get checked in the condition inside the scope of the loop. It must be declared outside since the while condition is outside this scope.

Section 5 - Research references

https://www.w3schools.com/cs/cs_while_loop.php


