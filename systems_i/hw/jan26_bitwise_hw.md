BY SUBMITTING THIS FILE TO CARMEN, I CERTIFY THAT I HAVE STRICTLY ADHERED TO THE TENURES OF THE OHIO STATE UNIVERSITY’S ACADEMIC INTEGRITY POLICY.

Name: Henry Manning
CSE 2421
Spring, 2024

Bitwise Homework – 31 points; grade reported in Carmen as points out of 31.

Due Date: Friday, January 26, 2024 by 11:30PM. Only submissions via Carmen will be accepted without prior approval. To receive credit, solutions must be clearly written or typed and appear in the same order as the questions below. If you choose not to break up your binary values into 4-bit nibbles, making it harder to read your work, the graders are authorized to lower your grade by 20%.  (e.g.  if you would have received 80% on your homework, you will receive a grade of (80%*.8) or 64%)

Early submissions are allowable although no bonus awarded for early homework.  Late submissions accepted for up to 24 hours after due date with 25% penalty (%correct *.75).                                       

[16 points] Complete the table below showing the effect of the different shift operations.  Use 8 bits for the binary representations.  Use logical left/right shifting rather than arithmetic.

x | Binary x | y | Binary y | x & y | (logical) x >>1 | (x & y )<<7 | (x>>1)&#124;((x & y)<<7)
--- | --- | --- | --- | --- | --- | --- | --- 
0xB1 | 1011 0001 | 0x01 | 0000 0001 | 0000 0001 | 0101 1000 | 1000 0000 | 1101 1000
0x72 | 0111 0010 | 0x01 | 0000 0001 | 0000 0000 | 0011 1001 | 0000 0000 | 0011 1001
0x33 | 0011 0011 | 0x01 | 0000 0001 | 0000 0001 | 0001 1001 | 1000 0000 | 1001 1001
0xA6 | 1010 0110 | 0x01 | 0000 0001 | 0000 0000 | 0101 0011 | 0000 0000 | 0101 0011

[5 points] After computing the values in the table above, look closely at the values in the Binary x column and the rightmost column of the chart. Can you describe the relationship between the two binary values?   

The right most column of the chart has all the same bits of the `binary x` but rotated 1 bit to the right, meaning that they were shifted 1 bit to the right and the most significant bit is replaced by old least significan bit.

[5 points] Given the relationship you described in Question 2, how would you get an analogous result when shifting x one position to the left rather than to the right? What value would you use for y?

For `y` I would use 0x80. You could use the exact same process for this as we traced in the table for the first question.

[5 points] If you wanted to shift 2 positions left or right, how could you change y to easily do this?

Just add another bit to the left or right side of y. Changing it either to 0x03 or 0xC0.