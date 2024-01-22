# Lecture 4
 - `Permutations` - An ordered set of outcomes. The number of possible outcomes in the sample space =
    - (n!)/(n-r)! - Where `r` = number of outcome events, and `n` equals number of elements in the sample
 - `Combinations` - An unordered subset of items from a list of distinct items. The number of possible outcomes = 
    - (n!)/((n-r)!(r)!)

# Multiple Combination
Suppose you have a set of distinct objects, but a subset of those belong to a group you want to limit or guarantee a number of in the result. You use multiple combinations for this.  
**Example:** There are 25 faculty in department A and 6 of them are cross-listed in department B. How many ways can you choose 3 faculty from department A with at most 1 of them cross listed in department B?
<center>
6C0 * 19C3 + 6C1 * 19C2 = 1995
</center>
This equation to solve sums the outcomes of choosing no cross listed faculty in our set of three and choosing 1 cross listed faculty in the set of three, but excludes all combinations with 6 choose 2 and 6 choose 3.