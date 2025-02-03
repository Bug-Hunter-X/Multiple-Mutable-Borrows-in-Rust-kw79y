# Multiple Mutable Borrows in Rust

This repository demonstrates a common error in Rust: attempting to create multiple mutable borrows to the same variable.  Rust's borrow checker prevents this to ensure memory safety and data consistency. The `bug.rs` file contains the erroneous code, while `bugSolution.rs` shows how to correctly handle this scenario.

The error arises because Rust's ownership system doesn't allow simultaneous mutable access to a single variable from multiple locations. Doing so could lead to unpredictable behavior and data corruption. 