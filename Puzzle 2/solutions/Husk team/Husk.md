# [Husk](https://github.com/barbuz/Husk), 9 bytes

    ΣẊ-!SCṁdN

[Test suite.](https://tio.run/##yygtzv6vkPuoqfH/ucUPd3XpKgY7P9zZmOL3////aEMdIx1jHRMdUx0zHXMdCx1LHUODWAA)

Author: [GolfingSuccess](https://github.com/GolfingSuccess) - [Erik the Outgolfer](https://chat.stackexchange.com/users/80316/erik-the-outgolfer)

# Explanation

    ΣẊ-!SCṁdN⁰
        S      (x -> y -> z):f -> (x -> y):g -> x:x :: return f(x, g(x))
         C      f= [num]:x -> [x]:y -> [x] :: cut y in pieces where each piece has its respective length in x
          ṁ     g= (x -> [y]):f -> ([x]:x -> [y]) :: maps f over x then concatenate
           d     f= num:x -> [num] :: return decimal digits of x
            N   x= sequence of natural numbers [1..]
       !     ⁰ [x]:x -> num:y -> x :: get yth (impl. input) element of x (above result)
     Ẋ         (x -> x -> y):f -> [x]:x -> [y] :: map f over overlapping pairs of x (above result)
      -         f= num:x -> num:y -> num :: return y - x
    Σ          [num]:x -> num :: return sum of x (above result)
