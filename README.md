# Haskell Sort Function Bug

This repository demonstrates a common misunderstanding with Haskell's `sort` function.  Many programmers new to Haskell expect `sort` to behave like in-place sorting functions in imperative languages. However, Haskell's `sort` is a pure function; it returns a *new* sorted list, leaving the original list unchanged.  This example highlights this behavior and provides a solution.

## Bug
The original code attempts to sort a list using `sort` and then print the result.  The issue lies in the assumption that the original list is modified.  Haskell's immutability means that the original list remains unchanged.