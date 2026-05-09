Section 1 - Concept of foreach

The foreach is a specific loop used to read through elements in an array. The foreach loop uses a temporary variable to refer to the element and will iterate as many times as elements sitting in the array, stopping automatically at the end of the array (no out of bound error). It doesn't need any control variable (like "i" in for loops). For each element in the array (each iteration) it will execute a block of code. Note that this loop cannot manipulate the values in the array, it's used to read only. We chose foreach over for loop when we only need to read an array.


Section 2 - Syntax

foreach (varType varName in arrayName)

{

  // block of code

}

Example:

int [] arrayOfNum = {1,2,3};

foreach (int num in arrayOfNum)

{

  Console.WriteLine(num);  // will print every number sitting inside arrayOfNum

}

Section 3 - Eureka moment

No particular difficulty in foreach loops. It's a pretty simple tool to use. 

Section 4 - Common beginner mistake

A beginner mistake could be trying to modify the values of the array with a foreach loop. if you try to do so, you will have a compile error since the temporary-value is read only.

Section 5 - Research references

https://www.w3schools.com/cs/cs_foreach_loop.php

https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/statements/iteration-statements

