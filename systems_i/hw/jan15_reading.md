# Week 1 Reading

## Prata 711-722 & 725-736 - The C Preprocessor and C Library

The Preprocessor looks at the program before it is compiled and expands symbolic abbreviations into the directions they represent. The preprocessor can also include other files.
 - All preprocessor directives are indicated by a '#' at the line start
 - #define - three constituent parts. `macro expansion` is the translation from the macro to the body
    - `#define` - preprocessor directive
    - `macro` - the abbreviation being used
    - `body` - the abbreviated
 - #define with arguments - `function-like macros`
    - `#define MACRO(X,Y) X*Y` - the macro takes arguments `X` and `Y` and expands them into the function
 - #include - replaced by the contents of the file named. Takes one argumetn
    - `#include` - preprocessor directive
    - `file name` - the file to be included
        - `<>` - angle brackets search standard directories
        - `""` - quotes search working directory first

**More Directives**
 - `#undef` - undefines a given #define
 - `#ifdef` - block gets done if argument is defined
    - `#ifdef MAVIS` - gets done if `MAVIS` is defined
 - `#ifndef` - block gets done if argument is NOT defined
 - `#else` - functions as an else to the #ifdef
 - `#endif` - ends the #ifdef block
 - `#if` - behave more like standard C if
    - `#if SYS == 1` - executes if SYS is equal to one
 - `#elif` - extends #if

## B&O Chapter 1-1.3

Nothing considerable not covered in class.