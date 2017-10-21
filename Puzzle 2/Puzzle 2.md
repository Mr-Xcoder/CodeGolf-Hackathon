# Puzzle 2 - Alternested numbers

### Definition

Consider the array of positive integers:

    1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, ...
    
Then, concatenate them:

    1234567891011121314151617181920212223242526...
    
And then try spliting them into chuncks of variable length, each length being equal to the **N**th positive integer:

    [1][23][456][7891][01112][131415][1617181][92021222][324252627][2829303132] ...
    ---------------------------------------------------------------------------
     1  2    3     4     5       6       7        8          9          10      ...
     
### Task
 
Given an integer **N** (positive for 1-indexing or non-negative for 0-indexing), your task is to output the sum of deltas bewteen the digits in that chunck (the differences between consecutive digits).

### Examples & Test cases

|**N**|Chunck|Deltas|Sum|
|-----|------|------|---|
|1|`1`|`[]`|`0`|
|2|`23`|`[1]`|`1`|
|3|`456`|`[1, 1, 1]`|`3`|
|4|`7891`|`[1, 1, -8]`|`-6`|
|5|`01112`|`[1,0,0,1]`|`2`|
|6|`131415`|`[2, -2, 3, -3, 4]`|`4`|
|7|`1617181`|`[5, -5, 6, -6, 7, -7]`|`0`|
|8|`92021222`|`[-7, -2, 2, -1, 1, 0, 0]`|`-7`|
|9|`324252627`|`[-1, 2, -2, 3, -3, 4, -4, 5]`|`4`|
|10|`2829303132`|`[6, -6, 7, -6, -3, 3, -2, 2, -1]`|`0`|

