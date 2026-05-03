Section 1 - Concept of If statement

The "if statement" allows the program to read a specific snippet of code if a certain condition is satisfied. The condition is a simple or complex boolean expression. If it evaluates to true, the program enters the code between the curly brackets ("{}"), executes it and then goes to the next reachable line of code after the if statement. 
If it evaluates to false, the program skips the brackets and goes directly to the next reachable line of code.

You can add more conditions in an "if statement" to make your program access different blocks of code with "else if". It's important to note that after accessing a block of code when a condition is met, the program exits the whole if statement. It means that if multiple conditions can be met, only the first block of code accessed will be read, the rest will be skipped.

You can also add an "else" block if you want to define what the program will do if none of the conditions are met.

Section 2 - Syntax

if (condition 1)  --> if condition 1 is met, the program executes the code block 1
{
// code block 1
}
else if (condition 2) --> if condition 2 is met AND not condition 1, executes the code block 2
{
// code block 2
}
else --> if neither condition 1 or 2 are met, executes block 3. Note that we don't necessarily need the "else" block.
{
// code block 3
}

Example: 

Let's consider an integer "num".

if (num > 0)
{
Console.WriteLine("This is a positive number!");
}
else 
{
Console.WriteLine("This is not a positive number!");
}

Section 3 - Eureka moment



Section 4 - Common beginner mistake


Section 5 - Research references

https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/statements/selection-statements
