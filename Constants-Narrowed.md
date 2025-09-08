### **Variables**
- Declared with `let` (immutable by default) or `let mut` (mutable).
- Scoped to a block (e.g., function or `{}`).
- Type can be inferred or explicit (e.g., `let x: i32 = 5` or `let x = 5`).
- Can be reassigned (if `mut`) or shadowed (redeclared with same name, even different type).
- Used for values that may change or are computed at runtime.

**Example**:
```rust
let x = 5; // Immutable
let mut y = 10; // Mutable
y = 20; // OK
let x = "hello"; // Shadowing
```

### **Constants**
- Declared with `const`, always immutable.
- Often global/module-scoped, accessible program-wide.
- Must have explicit type (e.g., `const MAX: i32 = 100`).
- Value must be a constant expression (set at compile time, no runtime computation).
- Use `SCREAMING_SNAKE_CASE`, inlined at compile time.

**Example**:
```rust
const MAX: i32 = 100;
println!("Max: {}", MAX); // Max: 100
```

### **Key Differences**
| **Feature**       | **Variables**                     | **Constants**                    |
|--------------------|-----------------------------------|----------------------------------|
| **Keyword**       | `let` / `let mut`                | `const`                         |
| **Mutability**    | Immutable or mutable (`mut`)      | Always immutable                |
| **Scope**         | Block-scoped                     | Often global                    |
| **Type**          | Inferred or explicit             | Explicit only                   |
| **Value**         | Runtime or compile-time          | Compile-time only               |
| **Reassignment**  | Allowed if `mut`; supports shadowing | Not allowed                  |
| **Naming**        | `camelCase` / `snake_case`       | `SCREAMING_SNAKE_CASE`          |

### **Summary**
- Use **variables** for dynamic, block-scoped data (mutable or immutable).
- Use **constants** for fixed, compile-time values, often global.

[Canvas](Rust.canvas)
[Code Snippet](Code)

