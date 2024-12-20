# Unhandled JSON Decoding Exception in Dart

This repository demonstrates a common error in Dart: failing to handle potential exceptions during JSON decoding.  The `bug.dart` file shows the problematic code, while `bugSolution.dart` provides an improved version with robust error handling.

## Problem

The original code lacks proper error handling for the `jsonDecode` function. If the API response isn't valid JSON, a `FormatException` will be thrown, potentially crashing the application.

## Solution

The solution uses a `try-catch` block to gracefully handle the `FormatException`. It also includes more informative error messages for debugging purposes.