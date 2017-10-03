# Puzzle 1 - The Golfy Array

### Definition

A *golfy array* is an array of positive integers, where each element is higher than or equal to the arithmetic mean of all the previous terms. 

### Task

Your task is to determine whether a given array is golfy or not.

### Example

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

All the elements respect the condition, thus this is a golfy array. Note that for the purpose of this challenge, we will assume that the average of `[]` is `0`.

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

### Rules

- [PPCG loopholes apply](https://codegolf.meta.stackexchange.com/questions/1061/loopholes-that-are-forbidden-by-default).

- [PPCG Standard Input and Output methods apply](https://codegolf.meta.stackexchange.com/questions/2447/default-for-code-golf-input-output-methods).

- You can choose any two distinct non-empty values. They **must** be consistent.

### References 

- [Arithmetic mean](https://en.wikipedia.org/wiki/Arithmetic_mean).

- **Labels (from PPCG Tags):** [Array Manipulation](https://codegolf.stackexchange.com/questions/tagged/array-manipulation), [Integer](https://codegolf.stackexchange.com/questions/tagged/integer), [Arithmetic](https://codegolf.stackexchange.com/questions/tagged/arithmetic), [Decision Problem](https://codegolf.stackexchange.com/questions/tagged/decision-problem).

- **Difficulty:** 4/10

### Scoreboard

|Position|Team|Current lowest byte count|Author|Current Status|
|--------|----|-------------------------|------|------|
|**#1**|Jelly|[6 bytes](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%201/solutions/Jelly%20team/Jelly.md)|[SatansSon](https://github.com/SatansSon)|**Golden golf**|
|**#1**|05AB1E|[6 bytes](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%201/solutions/05AB1E%20team/05AB1E.md)|[Adriandmen](https://github.com/Adriandmen)|**Golden golf**|
|**#2**|Pyth|[7 bytes](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%201/solutions/Pyth%20team/Pyth2.md)|[GolfingSuccess](https://github.com/GolfingSuccess)|**Silver golf**|
|**#3**|Husk|[8 bytes](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%201/solutions/Husk%20Team/Husk.md)|[H.PWiz](https://codegolf.stackexchange.com/users/71256/h-pwiz)|**Bronze Golf**|
|**#4**|Pyth|[10 bytes](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%201/solutions/Pyth%20team/Pyth.md)|[Mr-Xcoder](https://github.com/Mr-Xcoder)|**Competitor**|
