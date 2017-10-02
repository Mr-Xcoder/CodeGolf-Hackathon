# [Pyth](https://github.com/isaacg1/pyth), 7 bytes

    SI.OM._

[Test suite.](http://pyth.herokuapp.com/?code=SI.OM._&test_suite=1&test_suite_input=%5B%5D%0A%5B3%5D%0A%5B2%2C+12%5D%0A%5B1%2C+4%2C+3%2C+8%2C+6%5D%0A%5B1%2C+2%2C+3%2C+4%2C+5%5D%0A%5B6%2C+6%2C+6%2C+6%2C+6%5D%0A%5B3%2C+2%5D%0A%5B4%2C+5%2C+6%2C+4%5D%0A%5B4%2C+2%2C+1%2C+5%2C+7%5D%0A%5B45%2C+45%2C+46%2C+43%5D%0A%5B32%2C+9%2C+15%2C+19%2C+10%5D&debug=0)

Author: [GolfingSuccess](https://github.com/GolfingSuccess) - [Erik the Outgolfer](https://chat.stackexchange.com/users/80316/erik-the-outgolfer)

## Explanation

    SI.OM._
         ._ Get prefixes
      .OM   Map average
    SI      Check if sorted
