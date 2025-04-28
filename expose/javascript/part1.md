# Part 1 Answers

## `var` Declaration
1. What is printed by line 9? If the code returns an error, explain why. 
    No error was returned. This was what was printed: values added: 20
2. What is printed by line 13? If the code returns an error, explain why. 
    No error was returned. This was what was printed: final result: 20
3. Why should you not use var? Explain why. 
    `Var` should not be used because it does not observe block scoping rules. It can be accessed anywere in the code (even if it was declared inside a if/for loop) and that can lead to unexpected results and bugs.
4. What is printed by line 9? If the code returns an error, explain why. 
    No error was returned. This was what was printed: values added: 20
5. What is printed by line 13? If the code returns an error, explain why. 
    A reference error was returned because the `result` variable was not found. This is because `result` was declared the previous `if` loop and `let` variables are block scoped so it cannot be accessed outside of that function.

## `const` Declaration
6. What is printed by line 9? If the code returns an error, explain why.
    The code returns an error at line 7 before line 9 is even reached. There is a reassignment error because `result` was declared as a `const` variable and `const` variables cannot be reassigned new values.
7. What is printed by line 13? If the code returns an error, explain why. 
    The code returns an error at line 7 before line 13 is even reached. There is a reassignment error because `result` was 
    declared as a `const` variable and `const` variables cannot be reassigned new values, so the functions stops running immediately.
