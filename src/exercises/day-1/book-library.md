# Designing a Library

We will learn much more about structs and the `Vec<T>` type tomorrow. For now,
you just need to know part of its API:

```rust,editable
fn main() {
    let mut vec = vec![10, 20];
    vec.push(30);
    println!("middle value: {}", vec[vec.len() / 2]);
    for item in vec.iter() {
        println!("item: {item}");
    }
}
```

Use this to create a library application. Update the types to make the code
below compile:

```rust,should_panic
// TODO: remove this when you're done with your implementation.
#![allow(unused_variables, dead_code)]

{{#include book-library.rs:setup}}

{{#include book-library.rs:Library_new}}
        unimplemented!()
    }

{{#include book-library.rs:Library_len}}

{{#include book-library.rs:Library_is_empty}}

{{#include book-library.rs:Library_add_book}}

{{#include book-library.rs:Library_print_books}}

{{#include book-library.rs:Library_oldest_book}}
}

{{#include book-library.rs:main}}
```
