# Javascript Type Coercion Bug
This repository demonstrates a common Javascript bug arising from type coercion with the + operator. The `foo` function intends to add numbers, but due to Javascript's loose typing, it performs string concatenation when given strings, leading to unexpected results.

## Bug Description
The `foo` function adds two numbers. However, if either input is a string, Javascript converts the other to a string and performs string concatenation instead of numerical addition. This results in incorrect output, especially when unexpected string inputs are involved.

## Solution
The solution involves explicit type checking and conversion to ensure both inputs are numbers before performing addition.  This prevents implicit type coercion and ensures the function behaves as intended.