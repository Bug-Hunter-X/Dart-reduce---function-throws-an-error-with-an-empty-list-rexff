# Dart reduce() function throws an error with an empty list

This repository demonstrates a common error that can occur when using the `reduce()` function in Dart. The `reduce()` function is a powerful tool for processing lists, but it can throw an error if it encounters an empty list.

## Bug
The bug is that the `reduce()` function throws a `StateError` exception when invoked on an empty list.  This is because the `reduce` function needs at least one element to start the reduction process.  Attempting to reduce an empty list has no initial value to operate on.

## Solution
The solution is to check for an empty list before calling the `reduce()` function, and handle the empty case separately.  This prevents the `StateError` and allows your code to handle empty lists gracefully.
