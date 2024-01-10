# Lecture 2

There are two kinds of variables:
 - `Quantitative Variables`
    - `Discrete Variables` - There are distinct, separate steps without space in between. Like a grade (A, A-, B+, B, B-, etc.)
    - `Continuous Variables` - A continous range in which the variable can exist. Like GPA (4.0, 3.5, 3.75, 3.8, 3.9, etc.)
 - Qualitative Variables

## Sample Spaces and Events
In an ecperimental study, we investigate the **effects of** treatments on individuals in the sample.  
`Experiment` - Activity or process whose outcome is subject to uncertainty
 - Experiments that may be of interest include
    - Tossing a coin several times
    - Selecting a card or cards from a deck
    - Weighing a loaf of bread
    - etc.

`Sample Space (S)` - the set of all possible outcomes of an experiment
    - ie. S = {Outcome1, Outcome2}  
Examples:
1. A fair coin flipped once
    - S = {H, T}
2. A fair coin flipped three consecutive times
    - S = {HHH, HHT, HTH, HTT, THH, THT, TTH, TTT}
3. Record the wait time when calling customer service
    - S = {(0, infinity)}

`Event` - A colletion of outcomes of interest, or a subset of *S*  
Examples:
1. A = [H],  B = [T]
2. A = at least two heads (ie [HHH], [HHT], [HTH], or [THH])
3. A = {[0,10]},  B = {[0, 20]}

A pictorial representation of the sample space and events can be created with a venn diagram. First draw a rectangular background encompassing the sample space *S*, and then draw a diagram within the rectangle for each separate event, including overlap where there is overlap.  

## Set Relations
`Event Complement` - Suppose that A is an event. The complement of A, denoted by A^C or A', is another event that consists of all possible outcomes that are in S but not contained in A.
    - ie. If *S* = {1, 2, 3, 4, 5} and A = {1, 2} then A^C = A' = {3, 4, 5}
Because either A or A' must occur:
    - P(A) + P(A') = 1
    - P(A) = 1 - P(A')

`Intersection of Events` - Denoted by A intersection B, is the event containing all outcomes that belong to both A and B.  
`Union of Events` - Denoted by A union B, is the event containing all outcomes that belong to A or B inclusive.
`Empty/Null Set` - The set that contains no elements. It is denoted by phi.
`Disjoint` - Two events are disjoint if their intersection is the null set.

## Probability
The objective of probability is to assign a number P(A) to each event A representing the proportion of times that the event would occur under the same conditions.

`Long-run Relative Frequency` - The proportion of times an event occurs if you repeated the experiment occurs if you repeated the experiment an infinite number of times.  

Probability assignments must follow some axioms.
 - For any event A, 0 <= P(A) <= 1
 - P(*S*) = 1
    - conversely, P(null set/phi) = 0
 - For infinite disjoint events A_1, A_2, A_3, etc. P(A_1 or A_2 or A_3 or ...) = sum from i=n to infinity of A_i

### Example
Color | Brown | Red | Yellow | Green | Orange | Tan
--- | --- | --- | --- | --- | --- | ---
Probability | 0.3 | 0.2 | 0.2| 0.1 | 0.1 | ?
What is the probability that the outcome is Tan?
```
S = {B, R, Y, G, O, T}
A = {B, R, Y, G, O}
A' = {T}
P(A) = P(B) + P(R) + P(Y) + P(G) + P(O) = 0.3 + 0.2 + 0.2 + 0.1 + 0.1 = 0.9
P(A') = 1 - P(A) = 1 - 0.9 = 0.1 = P(T)
ANSWER : 0.1
```
---
### Equally Likely Outcomes
In an experiment where all of the outcomes have the same chance to occur, these are called `equally likely outcomes`.

### More Probability Rules
 - `Complement Rule` - For any event A, P(A) + P(A') = 1
 - ``