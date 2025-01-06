# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common JavaScript closure issue that occurs when using `setTimeout` within a loop. The problem arises because the `setTimeout` callback function doesn't capture the value of `i` at the time it's created, but rather captures a reference to the `i` variable itself. By the time the `setTimeout` callbacks finally execute, the loop has already completed, and `i` will have its final value (10). 

The `bug.js` file shows the incorrect implementation, and `bugSolution.js` provides a corrected version using closures to correctly capture the values of `i`.  This is a classic example highlighting the importance of understanding closures in JavaScript.