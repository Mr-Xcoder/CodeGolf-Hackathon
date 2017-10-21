# [Jelly](https://github.com/DennisMitchell/jelly), 10 bytes

    ²D€ẎṁR€ṪIS

[Test suite.](https://tio.run/##y0rNyan8///QJpdHTWse7up7uLMxCMTaucoz@P/RPYfbgRz3//@jDXUUjHQUjHUUTHQUTHUUzHQUzHUULHQULHUUDA1iAQ)

Author: [GolfingSuccess](https://github.com/GolfingSuccess) - [Erik the Outgolfer](https://chat.stackexchange.com/users/80316/erik-the-outgolfer)

# Explanation

    ²D€ẎṁR€ṪIS
    ²D€        Return list of lists of digits of numbers [1..z²]
       Ẏ       Concatenate
        ṁR€    Reshape like list of [1..n] ranges of numbers [1..z] (truncates)
           Ṫ   Pop last element
            I  Get deltas
             S Sum
