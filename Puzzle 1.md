# Puzzle 1 - The Golfy Array

A *golfy array* is an array of positive integers, where each element is higher than or equal to the arithmetic mean of all the previous terms. 

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
