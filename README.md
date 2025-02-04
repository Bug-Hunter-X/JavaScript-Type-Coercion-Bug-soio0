# JavaScript Type Coercion Bug

This repository demonstrates a common type coercion bug in JavaScript.  The `foo` function is intended to add two numbers but due to type coercion, it performs string concatenation when one of the inputs is a string.

## Bug Description
The bug lies in the lack of explicit type checking within the `foo` function. JavaScript's loose typing allows for implicit type conversions, leading to unexpected behavior when different data types are mixed. The bug results in unintended string concatenation rather than numerical addition.

## How to reproduce
Clone this repository and run `bug.js`. The output will show the unexpected string concatenation instead of numerical addition.

## Solution
The solution involves implementing explicit type checking to ensure both inputs are numbers before performing the addition.  The corrected code is provided in `bugSolution.js`.