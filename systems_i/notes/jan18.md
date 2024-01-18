# Lecture 6
**Bitwise Operators:**
 - `>>` - Right shift
    - Right shift has two modes, `Arithmetic shifting` and `Logical shifting`
    - Arithmetic shift is for signed values - Adds copies of the most significant bit when right shifting
    - Logical shift is for unsigned values - Adds 0s from the left
 - `<<` - Left shift
 - `&` - Bitwise AND
 - `|` - Bitwise OR
 - `^` - Bitwise XOR
 - `~` - Bitwise NOT  

**Logical Operators:**
 - `&&` - Logical AND
 - `||` - Logical OR
 - `!` - Logical NOT   

`&&` and `||` are short-circuited operators, meaning that because conditions are checked left to right, the outcome can sometimes be known just from the first of the two conditions joined by the operator. ie for `x && y` if `x=false` then the whole operation will be false, so `y` is not executed. Same for `||` but when the first argument is true.  

**Relational Operators:**
 - `<` - Less than
 - `>` - Greater than
 - `<=` - Less than equals
 - `>=` - Greater than equals
 - `==` - Equals
 - `!=` - Not equal

