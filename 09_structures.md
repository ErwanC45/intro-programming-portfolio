Section 1 - Concept of Structures

A structure is an object that can contain multiple variables called fields. It is defined with the key word struct followed by the name of the structure in pascal case notation. Then we define the different fields inside the scope of the structure giving them the variable type and the name. We need to use the keyword "public" before the fields to makes them accessible from outside the structure. The fields of the structure can be of different type (int, string, char...). Once defined, the structure is used as a variable and we can instantiate it like we declare a variable. We can access the fields using a dot notation (structName.fieldName).
Structures are useful to group multiple different but related variables.

Section 2 - Syntax

Defining a Struct:

struct StructName

{

  public varType1 FieldName1; // pascal case notation
  
  public varType2 FieldName2;

}

Instantiating a Struct variable:

structName varName; // this is the declaration

varName.FieldName1 = x;

varName.FieldName2 = y;

Example:

struct Student

{

  public string Name;
  
  public int Age;
  
  public double GPA;

}

Student s1; // declaration

s1.Name = "Erwan";

s1.Age = 33;

s1.GPA = 4.0;

Section 3 - Eureka moment

What was confusing at first was keeping track on the different "layers" and names (struct name, instance name, field names, struct as a type...). I'd sometimes get lost with the different terms. Doing simple defining exercises and then simple instantiating exercises helped me see clearer in all these terms before going a bit further in the structure concepts.

Section 4 - Common beginner mistake

A beginner mistake I made was forgetting the public while defining the field, this keyword being new for me. This would result in a compile error saying that the code is inaccessible and the program wouldn't start

Section 5 - Research references

https://www.youtube.com/watch?v=cy1vaWSuRtk

https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/struct
