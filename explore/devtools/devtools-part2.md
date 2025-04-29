## DevTools - Debugging
1. What was the bug?

The bug was that `num1` and `num2` were taken in as strings from the input fields. When passed into `calculateSum()`, the "+" operator concatenated the two strings instead of performing numeric addition.


2. How would you fix it? Include a screenshot of your fix. Name it fix.png (or whatever image extension you would like to use) and add it to your expand/screenshots directory.

I will fix it by converting `num1` and `num2` to numbers inside the `calculateSum()` function with the `Number()` function.