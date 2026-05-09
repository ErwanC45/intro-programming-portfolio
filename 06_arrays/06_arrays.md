Section 1 - Concept of arrays

An array is a collection of elements (values) stored sequentially. Like variables, they need to be declared and initialized. When declaring an array, we need to give its type (the type of the elements inside), its name and its length (the number of elements it can contain). You can declare and initialize with specific values right away, or declare and give values later. Note that if you don't immediately give values to the array, it will still be initialized with default values (for example "0" for an array of integers).
We can change the values in the array, but not its length. To access a specific value inside an array, we use its index. The index is the "location" of the value in the array. The index starts at 0 and goes to the array's length minus 1.
We usually operate through array with for loops. 


Section 2 - Syntax

Declaring:

arrType [] arrName = new arrType [length];

Declaring and initializing:

arrType [] arrName = {value1, value2, value3};

Accessing a value:

arrName [index];

Example:

int [] arrOfInt = new int [5]; // declaring an array of 5 integer (with the default values 0)

int [] arrOfInt2 = {1, 2, 3, 4, 5}; // declaring and initializing

Console.WriteLine($"This is the value held at index 4 : {arrOfInt2[4]}"); // outputs "5"

Section 3 - Eureka moment

At first, the main difficulty was manipulating array elements correctly using the for loop. The exercise 3 of Assignment 7, where we had to print an array in reverse order and copy its content reversed into a new array, helped me a lot to understand how to combine the array length and the index together. For example using length - 1 - i to navigate the array backwards.

Section 4 - Common beginner mistake

The most common mistake I made was probably mixing up the indexes and the number of values, because it's counterintuitive that the first value lies at index 0. It resulted in out of bound errors.

Section 5 - Research references

https://www.w3schools.com/cs/cs_arrays.php

https://www.w3schools.com/cs/cs_arrays_loop.php

