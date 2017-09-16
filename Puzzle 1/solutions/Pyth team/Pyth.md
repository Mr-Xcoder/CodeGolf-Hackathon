# [Pyth](https://github.com/isaacg1/pyth), 10 bytes

    .A.egb.O<Q

[Test Suite.](http://pyth.herokuapp.com/?code=.A.egb.O%3CQ&test_suite=1&test_suite_input=%5B%5D%0A%5B3%5D%0A%5B2%2C+12%5D%0A%5B1%2C+4%2C+3%2C+8%2C+6%5D%0A%5B1%2C+2%2C+3%2C+4%2C+5%5D%0A%5B6%2C+6%2C+6%2C+6%2C+6%5D%0A%5B3%2C+2%5D%0A%5B4%2C+5%2C+6%2C+4%5D%0A%5B4%2C+2%2C+1%2C+5%2C+7%5D%0A%5B45%2C+45%2C+46%2C+43%5D%0A%5B32%2C+9%2C+15%2C+19%2C+10%5D&debug=0)

Author: [Mr-Xcoder](https://github.com/Mr-Xcoder) - [Mr. Xcoder](https://chat.stackexchange.com/users/268674)

## Explanation

    .A.egb.O<Q  - Full program.
    
      .e        - Enumerated map over the implicit input, with b as values and k as indices.
          .O    - Arithmetic mean.
            <Q  - The elements before the current index (k).
         b      - The current value.
        g       - Is greater than or equal to?
    .A          - All elements are truthy; All in Python.
                - Implicitly output.
