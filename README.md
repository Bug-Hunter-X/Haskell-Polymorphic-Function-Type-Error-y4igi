# Haskell Polymorphic Function Type Error

This repository demonstrates a common type error in Haskell involving polymorphic functions.  The `bug.hs` file contains code that attempts to use a polymorphic function with incompatible types, resulting in a compilation error. The `bugSolution.hs` file shows a corrected version.

**Problem:**
The original code attempts to apply a polymorphic function `f` (designed to work with any type) to a String, but due to the later use, it expects an Int instead. This leads to a type mismatch that Haskell's type system catches.

**Solution:**
The solution involves either making the function `f` more specific or ensuring that the input passed to `f` is consistent with the polymorphic function type signature. If the type of `f` is correct, the other parts should be adjusted to match this type.