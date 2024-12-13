# Unexpected Null Behavior in JavaScript

This repository demonstrates a common error in JavaScript related to how null values are handled, especially when using loose comparison.  The `foo` function shows how explicitly checking for null can prevent unexpected results.

## The Problem

JavaScript's loose comparison (`==`) can lead to unexpected results when comparing values to `null` or `undefined`.  This is because the loose comparison does type coercion. 

## The Solution

Always explicitly check for null using the strict equality operator (`===`) to avoid unexpected coercion and maintain predictable behavior. This ensures that only values that are strictly equal to null are treated as null.

## How to Run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` to view the problematic and corrected code.
3. Run `node bug.js` and `node bugSolution.js` to see the output.