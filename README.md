# JavaScript Null Behavior with Strict Equality

This repository demonstrates a common error in JavaScript involving strict equality (===) and null comparisons.  The provided code shows a function that attempts to handle null values, but highlights unexpected behavior.

## Bug Description
The `foo` function uses `===` to check for null values before performing addition. While this handles the cases where either `a` or `b` is explicitly null, it might produce unexpected results in other scenarios involving nullish values (e.g., undefined).  The solution demonstrates a more robust approach.

## How to Reproduce
1. Clone the repository.
2. Run `node bug.js` to observe the unexpected behavior.
3. Run `node bugSolution.js` to see the improved handling of nullish values.

## Solution
The solution uses a more comprehensive approach that handles both null and undefined values appropriately.