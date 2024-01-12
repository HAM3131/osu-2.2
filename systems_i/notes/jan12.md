# Lecture 3

## Compilation (or Build) System
 - `Source file` - hello.c
 - `Preprocessor` - hello.i - `#includes` are expanded and `#defines` are replaced, comments are removed
 - `Compiler` - hello.s - C syntax parser generates assembler source code
 - `Assembler` - hello.o - generates an object file with unresolved symbols
 - `Linker` - a.out (default name) - resolves symbols and generates an executable by combining the object file with libraries
 - `Executable file` - hello

## C
### Basic Data Types
None of these sizes are absolutely fixed other than `char`. The others may vary by system and processor architecture. The `int` and `double` are the defaults for constants in your code.
 - `char` - character. 1 byte. this datatype can contain more than just ASCII characters.
 - `short` - 2 bytes typically.
 - `int` - 4 bytes typically. default type for integers.
 - `long` - 8 bytes typically. represents addresses (pointers).
 - `long long` - at least 8 bytes, sometimes 16. only supported in C99 and onwards.
 - `float` - about 4 bytes usually. single precision. about 6 decimal digits.
 - `double` - usually 8 bytes. double precision. about 15 decimal digits.
 - `long double` - usually 16 bytes. about 30 decimal digits.
### Derived Types
 - `arrays`
 - `pointers`
 - `structs`
 - `unions`
### Special Characters
Typing | Character
--- | ---
\a | alert (bell) character
\b | backspace
\f | formfeed
\n | newline
\r | carriage return
\t | horizontal tab
\v | vertical tab
\\\\ | backslash
\\? | question mark
\\' | single quote
\\" | double quote
\ooo| octal number
\xhh| hex number

### Constants
Declaring a constant can either be done by putting `const` before or after the type of the variable. You can also do this with the `#define` preprocessor directive. All of the following are acceptable.
```
#define PI 3.141593
const float PI = 3.141593
float const PI = 3.141593
```
Other features of the `#define` preprocessor directive include being able to expand a macro with parameters.
```
#define AREA(r) (3.141593 * r * r)
```

### Variable Declarations
You can declare/define one or multiple variables in a single line with commas. ie
```
int i, j=5, k;
char code, category;
int i = 123;
```
#### Type casting
You can cast a primitive to another primitive type with parentheses. For example:
```
int i = 65;
char ch;
ch = (char) i;
```
### Identifier Naming Style
Only a-z, A-Z, 0-9, and _ can be used. NO OTHER CHARACTERS can be used for function or variable names.
There is no guarantee that any value past the 31st character will be recognized.