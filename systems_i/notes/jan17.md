# Data Representation

Modern computers store and process information as two-values signals.  
 - `Byte` - 8 bits

There are numerous ways to interpret any given sequence of bytes.
 - `Unsigned Integer` - All digits represent a positive power of 2
 - `Signed Integer` - The digits are in 2's complement representation
    - First bit is a negative (b'1000' = -8)
    - All other bits are positive  

**Cool Tip** - If you want a condition to only allow integers that are positive but under an upper bound, you can avoid the ">0" check by casting to an unsigned integer.

Hexadecimal can be used as shorthand for four bits.
Binary | Hex | Binary | Hex
---: | :--- | ---: | :---
0000 | 0 | 1000 | 8
0001 | 1 | 1001 | 9
0010 | 2 | 1010 | A
0011 | 3 | 1011 | B
0100 | 4 | 1100 | C
0101 | 5 | 1101 | D
0110 | 6 | 1110 | E
0111 | 7 | 1111 | F

