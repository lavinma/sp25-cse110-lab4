# Part 2 Answers

1. What will happen at line 12 and why? If the code causes an error, explain why. 
   
    No error occurs. The following is printed: 3

    The variable `i` is declared as a  `var` variable making it function scoped (so it can be accessible anywhere in the function).
2. What will happen at line 13 and why? If the code causes an error, explain why
   
    No error occurs. The following is printed: 150

    The variable `discountedPrice` is declared as a  `var` variable making it function scoped (so it can be accessible anywhere in the function even outside of the for loop where it was initially declared).
3. What will happen at line 14 and why? If the code causes an error, explain why. 
   
    No error occurs. The following is printed: 150
    
    The variable `finalPrice` is declared as a  `var` variable making it function scoped (so it can be accessible anywhere in the 
    function). `finalPrice` is updated at each loop iteration and at the last iteration it holds the final calculated discounted price value and that is ultimately returned. 
4. What will this function return? Give a brief explanation why. If the code causes an error, explain why.
   
    The function returns `[50, 100, 150]`. The `for` loop calculates the discounted price for each item, rounds it, and pushes it into the `discounted` array. Then the `return discounted;` line executes. No errors occur, and the correct array `[50, 100, 150]` is returned.
5. What will happen at line 12 and why?  If the code causes an error, explain why.
   
    A reference error was returned because the `i` variable was not found. This is because `i` was declared in the `for` loop  and `let` variables are block scoped so it cannot be accessed outside of that function.
6. What will happen at line 13 and why?  If the code causes an error, explain why.
   
    A reference error was returned because the `discountedPrice` variable was not found. This is because `discountedPrice` was declared inside the `for` loop and `let` variables are block scoped so it cannot be accessed outside of that function. 
7. What will happen at line 14 and why? If the code causes an error, explain why. 
   
    No error occurs. The following is printed: 150

    The variable `finalPrice` is declared as a `let` variable outside the `for` loop, making it accessible anywhere inside the `discountPrices` function. It holds the final value after the `for` loop completely finishes running and that final computed value is what is printed.
8. What will this function return? Give a brief explanation. If the code causes an error, explain why. 
   
    The function returns `[50, 100, 150]`. The function correctly calculates the discounted prices for each item and pushes them into the `discounted` array which is then returned.
9.  What will happen at line 11 and why? If the code causes an error, explain why.
    
    A reference error occurs because the variable `i` is declared with `let` inside the `for` loop, making it block-scoped. So it cannot be accessed outside of that loop.
10. What will happen at line 12 and why? If the code causes an error, explain why.
    No error occurs. The following is printed: 3

    The variable `length` is declared with `const` at the beginning of the `discountPrices` function so it is in the scope of the entire function and no reference error occurs. 
11. What will this function return? Give a brief explanation. If the code causes an error, explain why.
    
    The function returns `[50, 100, 150]`. The function correctly calculates the discounted prices for each item (doing a 50% discount) and pushes them into the `discounted` array which is then returned. 

## Data Types
A. Accessing the value of the name property in the student object

`student.name`

B. Accessing the value of the Grad Year property in the student object

`student['Grad Year']`

C. Calling the function for the greeting property in the student object

`student.greeting()`

D. Accessing the name property of the object in the Favorite Teacher property in student

`student['Favorite Teacher'].name`

E. Access index zero in the array of the courseLoad property of the student object

`student.courseLoad[0]`

## Basic Operators & Type Conversion 
### Arithmetic 
A. '3' + 2
    
output: 32

why: JS converts the number `2` into a string and concatenates it with `'3'`, resulting in `'32'`.

B. '3' - 2

output: 1

why: The subtraction operator forces the function to convert the input to numbers, so `'3'` becomes `3`, and `3 - 2` equals`1`.

C. 3 + null

output: 3

why: `null` is converted to `0`, so the expression becomes `3 + 0` which equals `3`.

D. '3' + null

output: 3null

why: `null` is converted to string `'null'` and it is concatenated to `'3'`, so the output was `'3null'`

E. true + 3

output: 4

why: The boolean `true` is converted to `1`, and `1 + 3` equals `4`.

F. false + null

output: 0

why: Both `false` and `null` are converted to `0`, and `0 + 0` equals `0`.

G. '3' + undefined

output: 3undefined

why: JS turns `undefined` into the string `'undefined'`. It is then concatenated with `'3'`, resulting in `'3undefined'`.

H. '3' - undefined

output: Nan

why: The subtraction operator tries to convert both `'3'` and `undefined` into numbers, but `undefined` becomes `NaN`, and any arithmetic operation with `NaN` results in `NaN`.

### Comparison
A. '2' > 1

output: true

why: The string `'2'` is converted to the number `2`, and since `2 > 1`, the result is `true`.

B. '2' < '12'

output: false

why: JS compares string alphabetically, so since `'2'` comes after `'1'`, so `'2' < '12'` is `false`.

C. 2 == '2'

output: true

why: The `==` operator allows type coercion, so the string `'2'` is converted to the number `2`, and `2 == 2` is `true`.

D. 2 === '2'

output: false

why: The `===` operator checks both value and type without type conversion, so since `2` is a number and `'2'` is a string, so they are not equal.

E. true == 2

output: false

why: The boolean `true` is converted to `1`, so `1 == 2` is `false`.

F. true === Boolean(2)

output: true

why: `Boolean(2)` evaluates to `true`, and `true === true` is `true`.

Explain the difference between the == and === operators.

The `==` operator checks for equality after performing type conversion (if needed), meaning the operands can be different types and still be the expression would output equality.  
The `===` operator checks for both value and type to be the same without performing any type conversion.


### Functions
17.  The result of calling `modifyArray([1, 2, 3], doSomething)` is `[2, 4, 6]`. The `modifyArray` function takes an array and function`callback`. It loops through each element of the array and calls `callback` on each one. `callback` here is `doSomething`, which doubles the number. So `1` becomes `2`, `2` becomes `4`, and `3` becomes `6`. These values are added to a new array, which gets returned as `[2, 4, 6]`. 
18.  What is the output of the above code?
    output: 
    
    1

    4

    3

    2





