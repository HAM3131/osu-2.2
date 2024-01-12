# Lecture 2

C is procedural, not object oriented.  
It is fully compiled to machine code.  
It allows direct manipulation of memory.  
No garbage collection.  
Better.  

## What C doesn't do

C does not support classes or objects.  
It does not support encapsulation.  
It does not support polymorphism, virtual function, inheritance, operator overloading, namespace concepts, etc.  
It is not object oriented.  

## Compile time vs Run time

We separate events in computer science between can happen when we compile the code, and what can happen when we run it.
Compile time events are often referred to as `static`, and run time events are `dynamic`.
Errors which occur at run time are `semantic/dynamic errors`. 

## Big picture
There are four general categories of statements in computer languages. These encompass everything you can write in a programming language.
 - **Declarations**
    - These are optional in some languages like Python
 - **Data Movement**
    - Memory to function variables
    - Function variables to function variables
    - Function variables to memory
 - **Arithmentic/Logical Operations**
    - Compare something
    - Calculate something
 - **Control-Flow**
    - Procedure/function calls
    - Looping
    - Conditionals

## Preprocessor

The lines in a .c file with `#` at the start are called `preprocessor directives.`  
Preprocessor directives DO NOT end with a semicolon.
The `preprocessor` prepares a .c file for the compiler.  
Input goes from `src.c` to `src.i`.  
Strips all comments from the source code.  
Using any `#include file` directives in the source file, it copies the full contents into `src.i.`  

### Include Statements
 - `include <file>` - A global include following the path `/usr/include/file`
 - `include "file"` - A local include statement following the path `file`

## Functions

Functions have prototypes in c. This is a function declaration or definition which includes the meta details of a function without code. ie
```
float add_floats(float a, float b); // This ends with a ';' rather than '{}'
```
In general, C passes arguments to functions by value.  
But, if we want to pass arguments by reference we use `pointers.`

## Declaration vs Definition

`Declaration` - A variable or functions which is given it's type, but not it's exact value or code.  
`Definition` - A variable or functions which is given a value or code when it is declared.  

## 