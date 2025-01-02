# Handling Null Values in JavaScript

This repository demonstrates a common error in JavaScript: failing to explicitly handle null values in function arguments.  Improper null handling can lead to unexpected behavior, including runtime exceptions.

## Bug
The `bug.js` file shows a function that doesn't correctly handle cases where the input parameters (`a` and `b`) are null.  This can result in errors if the function attempts to perform operations on null values.

## Solution
The `bugSolution.js` file demonstrates a solution that explicitly checks for null values and handles them gracefully, preventing any errors.

## How to reproduce the bug

1. Run the code in `bug.js`.
2. Call the `foo` function with at least one null argument.
3. Observe the resulting error (or unexpected behavior).

## How to fix the bug

1. Implement checks for null values (as shown in `bugSolution.js`).
2. Decide how your function should behave when null values are encountered (e.g., return null, throw an error, use a default value).
3. Ensure that the rest of your function's logic only operates on valid non-null data.