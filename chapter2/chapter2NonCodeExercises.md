# Chapter 2 Non-Code exercises
1. Add "let" to the front of each of these. REPL requires that declaration.

2. let circleArea r = 3.14 * (r\*r)

3. let circleArea r = pi * (r\*r) 

# Chapter 2.6 Exercises

1. (B) Changes the value of the function. Goes from 71 to 225

2. (A) does not change the value of the function. Both return 4 with values of 1 for both variables

3. (B) changes the value of the function. Using 1 as an input, A returns 9.5, B returns 0.090909r

# Chapter 2.7 REPL exercises

1. 

    Prelude> let area x = 3. 14 * (x * x)
    <interactive>:14:5: error:
        Non type-variable argument in the constraint: Num (a -> b)
        (Use FlexibleContexts to permit this)
        When checking the inferred type
        area :: forall b c a.
        (Num (a -> b), Num (a -> c), Num (b -> c))      =>  (a -> c) -> a -> c
    Prelude> let area x = 3.14 * (x * x)
    Prelude> area 2
    12.56

2. 

     Prelude> let double x = b * 2
        <interactive>:17:16: error: Variable not in scope: b
    Prelude> let double x = x * 2
    Prelude> double 2
    4

