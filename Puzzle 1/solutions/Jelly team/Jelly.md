# [Jelly], 6 bytes

    ÆmƤµ⁼Ṣ

[Try it online!][TIO-j7nb0xzm]

[Jelly]: https://github.com/DennisMitchell/jelly
[TIO-j7nb0xzm]: https://tio.run/##y0rNyan8//9wW@6xJYe2Pmrc83Dnov@H2x81rXH//z86OlYn2hiIjXQUDI2AtKGOgomOgrGOgoWOghmEbwTmA0VNgXwzoDAcgfQC5YEUSBYsZgLhgIwDC5mD@EAajEHyIMuMgdKWQBVAMUMQbRAbCwA "Jelly – Try It Online"

Author: [SatansSon](https://github.com/SatansSon) - [caird coniheringaahing](https://codegolf.stackexchange.com/users/66833/caird-coinheringaahing).

## Explanation

    ÆmƤµ⁼Ṣ - Main link; argument z (array)                [1, 4, 3, 8, 6]

      Ƥ    - Generate the prefixes                        [[1], [1, 4], [1, 4, 3], [1, 4, 3, 8], [1, 4, 3, 8, 6]]
    Æm     - Get the mean of each                         [1, 2.5, 2.6666666666666665, 4, 4.4] 
       µ   - Start a new moadic chain with x as argument
         Ṣ - Sort x (call this y)                         [1, 2.5, 2.6666666666666665, 4, 4.4]
        ⁼  - Is y equal to x?                             1
