# C# NullReferenceException: Uninitialized Property

This repository demonstrates a common C# error: the `NullReferenceException`.  This exception occurs when you attempt to access a member (property or method) of an object that hasn't been initialized, meaning it's currently `null`.

The `bug.cs` file contains code that will throw a `NullReferenceException`. The `bugSolution.cs` file provides a corrected version.

## How to Reproduce

1. Clone this repository.
2. Compile and run `bug.cs`. You'll encounter a `NullReferenceException`.
3. Examine `bugSolution.cs` to see the fix.

## Solution

The solution involves initializing the `MyProperty` before accessing it.  This ensures that the object isn't null when the `ToString()` method is called.