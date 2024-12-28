# JavaScript Loose Equality with Null and Undefined

This repository demonstrates a common pitfall in JavaScript when using loose equality (`==`) to compare values, specifically with `null` and `undefined`.  The example shows how loose equality can lead to unexpected results and how to fix the problem using strict equality (`===`).

## Bug

The provided code uses loose equality (`==`) to check if a variable is `null`. However, this check will also evaluate to true for `undefined`, leading to unintended behavior when `undefined` is passed as an argument. The function is expected to return 0 for null and for undefined.

## Solution

The solution utilizes strict equality (`===`) to avoid the ambiguity of loose equality. Strict equality will only return true if both operands are of the same type and value.