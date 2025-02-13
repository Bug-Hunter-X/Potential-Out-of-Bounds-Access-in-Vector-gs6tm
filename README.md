# Rust Vector Out-of-Bounds Access Bug
This repository demonstrates a common error in Rust: accessing a vector element using an index without checking for bounds.

## Bug Description
The `bug.rs` file contains code that attempts to access a vector element at a given index.  However, it fails to check if the index is within the valid range of the vector. If the index is out of bounds, the program will panic.

## Solution
The `bugSolution.rs` file provides a corrected version of the code. It uses the `get()` method to safely access the element, returning an `Option` that handles the case where the index is out of bounds.

## How to Reproduce the Bug
1. Clone this repository.
2. Navigate to the directory in your terminal.
3. Run the code using `rustc bug.rs && ./bug`.