## Functional Programming Tasks

You can use language of your choice to solve these tasks, but solve the 
problems using functional programming approach. Try to use best programming practices 
when writing solutions. Focus more on code readability and coding 
conventions, not trying to create the most efficient and compact 
solution (which are often really hard to read/understand).

### Problem 1

Create a function multiplyAll/multiply_all which takes an array of integers as an argument.
This function must return another function, which takes an integer as an argument and 
returns a new array. The returned array should consist of each of the elements 
from the first array multiplied by the integer.

For example:

```
multiplyAll([1, 2, 3])(2) // -> [2, 4, 6]
multiplyAll([1, 2, 3])(3) // -> [3, 6, 9]
```


### Problem 2

Create a function flattenArray/flatten_array which takes a list as a parameter. That list can 
contain multiple nested lists and returns a single list containing all the
element expect nil/null values.

For example:

```
const arr = [[1, 2, 3, [4, 5, [6]]], [null], [7, 8], [9, [10, null]]]
flattenArray(arr) // -> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```
