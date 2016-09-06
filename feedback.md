# Feedback

## Two Sum 

> Monday, September 5th, 2016

### Mistakes (in JavaScript)

`for (int i=0; i<(len(nums)-1); i++)`

#### Mistake 1: Using Java types!

We should never have *any* 'int' or other types in JavaScript! 

#### Mistake 2: Array.length

len(arr) is Python! For JavaScript, you call .length on your array.

### Big O

Time Complexity for brute force (double for loop) solution:

let n = length of nums
Draw a n x n triangle thing --> n^2 / 2 = O(n^2)

Space Complexity: iterating through arrays, O(1)

### Cool Stuff

If you don't have anything to return (and you're supposed to) at least throw an exception or print something.

In Java: `throw new IllegalArgumentException("No two sum solution");`

In JavaScript: `print("No two sum solution")`
