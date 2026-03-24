# E++ Compiler

## Overview
This project implements a simplified compiler for a custom language (**E++**) with support for **arbitrary-precision arithmetic** and **expression evaluation**.

The system parses mathematical expressions, constructs structured representations using trees, and compiles them into a **stack-based target machine language**.

---

## Key Features

- **Arbitrary Precision Arithmetic**
  - Implemented custom data types:
    - `UnlimitedInt`
    - `UnlimitedRational`
  - Enables handling of large integers and rational numbers beyond standard limits

- **Expression Parsing**
  - Parses infix expressions containing:
    - variables
    - constants
    - operators
  - Converts expressions into a **unified AVL tree structure** for efficient evaluation

- **Compiler Pipeline**
  - Builds **symbol tables** for variable management
  - Translates parsed expressions into a **stack-based target language (Targ)**

- **Tree-Based Representation**
  - Uses **AVL trees** to maintain balanced expression structures
  - Ensures efficient operations and evaluation

```
├── UnlimitedInt / UnlimitedRational # Arbitrary precision number implementation
├── Parser # Infix expression parsing logic
├── AVL Tree # Expression representation
├── Symbol Table # Variable storage and lookup
├── Compiler # Translation to target machine code
├── Targ Machine # Stack-based execution model
```
