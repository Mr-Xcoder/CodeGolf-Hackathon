# Puzzle 2 - Alternested numbers

### Definition

Consider the array of positive integers:

    1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, ...
    
Then, concatenate them:

    1234567891011121314151617181920212223242526...
    
And then try spliting them into chunks of variable length, each length being equal to the **N**th positive integer:

    [1][23][456][7891][01112][131415][1617181][92021222][324252627][2829303132] ...
    ---------------------------------------------------------------------------
     1  2    3     4     5       6       7        8          9          10      ...
     
### Task
 
Given an integer **N** (positive for 1-indexing or non-negative for 0-indexing), your task is to output the sum of deltas between the digits in that chunk (the differences between consecutive digits).

### Examples & Test cases

|**N**|Chunck|Deltas|Sum|
|-----|------|------|---|
|1|`1`|`[]`|`0`|
|2|`23`|`[1]`|`1`|
|3|`456`|`[1, 1]`|`2`|
|4|`7891`|`[1, 1, -8]`|`-6`|
|5|`01112`|`[1, 0, 0,1]`|`2`|
|6|`131415`|`[2, -2, 3, -3, 4]`|`4`|
|7|`1617181`|`[5, -5, 6, -6, 7, -7]`|`0`|
|8|`92021222`|`[-7, -2, 2, -1, 1, 0, 0]`|`-7`|
|9|`324252627`|`[-1, 2, -2, 3, -3, 4, -4, 5]`|`4`|
|10|`2829303132`|`[6, -6, 7, -6, -3, 3, -2, 2, -1]`|`0`|

### Rules

- [PPCG loopholes apply](https://codegolf.meta.stackexchange.com/questions/1061/loopholes-that-are-forbidden-by-default).

- [PPCG Standard Input and Output methods apply](https://codegolf.meta.stackexchange.com/questions/2447/default-for-code-golf-input-output-methods).

- You may choose either 0 or 1-indexing for **N**.

- You may **not** include **0** in the sequence though, so it must start with `1234...`.

### References 

- **Labels (from PPCG Tags):** [Sequence](https://codegolf.stackexchange.com/questions/tagged/sequence), [Array Manipulation](https://codegolf.stackexchange.com/questions/tagged/array-manipulation).

- **Difficulty:** 6/10

### Scoreboard

|Position|Team|Current lowest byte count|Author|Current Status|
|--------|----|-------------------------|------|--------------|
|**#1**|Husk|[9 bytes](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%202/solutions/Husk%20team/Husk.md)|[GolfingSuccess](https://github.com/GolfingSuccess)|**Golden golf**|
|**#2**|Jelly|[10 bytes](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%202/solutions/Jelly%20team/Jelly2.md)|[GolfingSuccess](https://github.com/GolfingSuccess)|**Silver golf**|
|**#3**|Jelly|<!--[-->13 bytes<!--](https://github.com/Mr-Xcoder/CodeGolf-Hackathon/blob/master/Puzzle%202/solutions/Jelly%20team/Jelly.md)--> (no explanation)|[kckennylau](https://github.com/kckennylau)|**Bronze golf**|
