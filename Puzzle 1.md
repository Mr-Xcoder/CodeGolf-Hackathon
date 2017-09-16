# Puzzle 1 - The Golfy Array

### Definition

A *golfy array* is an array of positive integers, where each element is higher than or equal to the arithmetic mean of all the previous terms. 

### Exmple

For example, the following array:

    [1, 4, 3, 8, 6]
    
Is a golfy array, because each term is higher than the arithmetic mean of those preceding it. Let's work it out step-by-step:

|Current Number|Elements preceding it|Average|Follows the rule?|
|--------------|---------------------|-------|-----------------|
|`1`|`[]`|`0.0`|`1 ≥ 0.0`, True|
|`4`|`[1]`|`1.0`|`4 ≥ 1.0`, True|
|`3`|`[1, 4]`|`2.5`|`3 ≥ 2.5`, True|
|`8`|`[1, 4, 3]`|`2.(6)`|`8 ≥ 2.(6)`, True|
|`6`|`[1, 4, 3, 8]`|`4.0`|`6 ≥ 4.0`, True|

All the elements respect the condition, thus this is a golfy array.

### Test Cases

|Input|Output|
|-----|------|
|`[]`|True|
|`[3]`|True|
|`[2, 12]`|True|
|`[1, 4, 3, 8, 6]`|True|
|`[1, 2, 3, 4, 5]`|True|
|`[6, 6, 6, 6, 6]`|True|
|`[3, 2]`|False|
|`[4, 5, 6, 4]`|False|
|`[4, 2, 1, 5, 7]`|False|
|`[45, 45, 46, 43]`|False|
|`[32, 9, 15, 19, 10]`|False|

### References 

- [Arithmetic mean](https://en.wikipedia.org/wiki/Arithmetic_mean).

### Tags

[Array Manipulation](https://codegolf.stackexchange.com/questions/tagged/array-manipulation), [Integer](https://codegolf.stackexchange.com/questions/tagged/integer), [Arithmetic](https://codegolf.stackexchange.com/questions/tagged/arithmetic)