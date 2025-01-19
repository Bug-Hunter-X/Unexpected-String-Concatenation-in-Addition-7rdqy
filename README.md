# Unexpected String Concatenation in JavaScript Addition

This repository demonstrates a common, yet subtle, bug in JavaScript related to the '+' operator and type coercion.  The `bug.js` file contains code that, under certain conditions, will unexpectedly concatenate strings instead of performing numerical addition. The `bugSolution.js` file offers a solution to prevent this issue.

## The Problem

In JavaScript, the '+' operator is overloaded. It performs both numerical addition and string concatenation.  If one or both operands are strings, it performs string concatenation. This can lead to unexpected results when working with numbers that might be inadvertently treated as strings.

## The Solution

The most reliable solution is to explicitly convert the operands to numbers before performing addition.  The `bugSolution.js` file shows how to use `Number()` or `parseInt()` to ensure that the addition operation behaves as expected.

## How to Run the Code

1. Clone the repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment.
3. Execute the code. Observe the different outputs and understand how the solution addresses the potential bug.