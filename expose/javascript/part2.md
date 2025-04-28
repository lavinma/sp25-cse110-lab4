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