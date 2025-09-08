```rust
// This is a comment
/*
 * this
 * is a
 * multi-line
 * comment
 */
 
fn main() {
    let toprint = "Hello, world!";
    let age = 69;
    let name = "John Doe";

    let mut mutable_int = 42;

    println!("{}", toprint);

    println!("{} is {} years old", name, age);

    println!("I'm mutable: {}", mutable_int);
    mutable_int = 100;
    println!("See?: {}", mutable_int);

    const MY_NUM: i32 = 42;
    const MY_DOUBLE: f64 = 64.0;
    const MY_LETTER: char = 'D';
    const MY_BOOL: bool = true;
    const MY_TEXT: &str = "Hello";

    let my_tuple = (MY_NUM, MY_DOUBLE, MY_LETTER, MY_BOOL, MY_TEXT);

    println!("{:?} we are ALL CONSTANTS", my_tuple);
}


```
