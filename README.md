# Uninitialized Property Access in C#

This repository demonstrates a common error in C#: accessing a property that hasn't been explicitly initialized.  Uninitialized properties can lead to unexpected results, especially when the property's type is a value type like `int`. In this case, the property defaults to its type's default value. This example shows how an uninitialized property can cause issues when accessing it in methods.

## How to reproduce

1. Clone this repository.
2. Open the `bug.cs` file.
3. Observe how the `MyProperty` in the `MyMethod` function is accessed without being initialized.
4. Run the code, you might see the default value (0) if the property is an integer, or unexpected behavior if it's a reference type.

## Solution

The `bugSolution.cs` file provides a corrected version.   Proper initialization is essential to prevent unexpected runtime errors or default values from influencing program behavior.