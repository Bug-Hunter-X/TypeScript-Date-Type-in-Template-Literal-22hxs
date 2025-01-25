# TypeScript Date Type in Template Literal Bug

This repository demonstrates a common, subtle bug in TypeScript related to using Date objects directly within template literals. The issue arises from the implicit type coercion that can lead to unexpected results or runtime errors.

## Bug Description

The provided TypeScript code defines a function 'greet' that takes a person's name and a Date object as parameters. Inside the function, it attempts to directly embed the Date object within a template literal to format a greeting.  However, this doesn't implicitly convert the Date object to a user-friendly string. Instead, it includes the object's internal representation, leading to an unusual output.

## Solution

The solution involves explicitly converting the Date object to a string using methods like `toDateString()` or `toLocaleDateString()` before incorporating it into the template literal. This ensures the expected string representation is used.

## How to Run

1. Clone the repository.
2. Compile the TypeScript code using a compiler like the TypeScript compiler (tsc).  
3. Run the compiled Javascript code