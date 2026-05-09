Section 1 - Concept of 2D arrays

A 2D array is a multidimensional array. It is, in a way, an array of arrays. It's used to store data in a table and create matrices, as it allows us to manipulate data with rows and columns. We create a 2D array the same way we create an array, but inside the empty brackets we put a comma [,]. Before the comma will be the number of rows, after the comma the number of columns. In fact, we can add more dimensions to an array by adding more commas. 
To access an element, we specify the row and the column (before and after the comma).
We iterate through a 2D array with nested for loops. Like regular arrays, the indexes starts at 0 for both rows and columns.
However, to use the length of a 2d array, we can't use array.Length. Instead we use array.GetLength() with the "number" of the dimension between the parenthesis (0 for rows, 1 for columns).

Section 2 - Syntax

Section 2 - Syntax

Declaring:

arrType [,] arrName = new arrType [numberOfRows,numberOfColumns];

Declaring and initializing:

arrType [,] arrName = {{value1, value2, value3}, {value4,value5,value6},{...}}; // the inner curly brackets represent a row, the numbers of value in each row is the number of columns

Accessing a value:

arrName [indexOfRow,indexOfColumn];

Examples:

int [,] tableOfInt = new int [2,3]; // declaring an array of 2 rows and 3 column of integers (with the default values 0)

int [,] tableOfInt2 = {{1, 2, 3}, {4, 5,6}}; // declaring and initializing

Console.WriteLine($"This is the value held at row 0, column 1: {tableOfInt2[0,1]}"); // outputs "2"

for (int i = 0; i < tableOfInt2.GetLength(0); i++)

{

  for (int j = 0; j < tableOfInt2.GetLength(1); j++)

  {

  Console.WriteLine($"This is the value held at row {i}, column {j}: {tableOfInt2[i,j]}");

  }

}

Section 3 - Eureka moment

I found 2D arrays pretty tricky. When it came to operations in a 2D array, I  had a hard time identifying in which loop I needed to compute, print or store a value. For example, in the exercise 12 of Assignment 7 we had to compute and print the sum of the rows and columns. Doing this exercise helped me visualize how it worked.

Section 4 - Common beginner mistake

A simple beginner mistake I made was using array.Length instead of array.GetLength(), as a bad habit from working with simple arrays. This would instead give the total of elements in the array (rows x columns) causing an out of bounds error. 

Section 5 - Research references

Class materials and Assignments

https://www.w3schools.com/cs/cs_arrays_multi.php

https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/arrays#single-dimensional-arrays
