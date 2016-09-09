# Two Sum 

> Monday, September 5th, 2016

### Mistakes (in JavaScript) for Brute Force

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

### HashMap Solution One (Java)

Now O(n) time complexity (2 O(n) passes through the loop) but O(n) space complexity (to house the hash map)

#### Stuff I Learned

* In Java, to get the keyset of a Map, you call the `<Map>.keySet()` method
* To create a new array with some values, you can do `int[] arr = {1,2,3};`
* Don't forget your **return** statements!
* You can directly check if a Map contains key with the `containsKey(Object key)` method
* Double check if you're supposed to return indices or values
