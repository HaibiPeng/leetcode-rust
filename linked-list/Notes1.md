# keywords

1. [ref](https://doc.rust-lang.org/std/keyword.ref.html#-vs-ref): Bind by reference during pattern matching

2. [match](https://doc.rust-lang.org/std/keyword.match.html): Control flow based on pattern matching.

3. [mut](https://doc.rust-lang.org/std/keyword.mut.html): A mutable variable, reference, or pointer.

4. [unsafe](https://doc.rust-lang.org/std/keyword.unsafe.html): Code or interfaces whose memory safety cannot be verified by the type system.

# type

1. [pointer](https://doc.rust-lang.org/std/primitive.pointer.html#): Raw, unsafe pointers, *const T, and *mut T.

2. [reference](https://doc.rust-lang.org/std/primitive.reference.html): References, &T and &mut T. A reference represents a borrow of some owned value.

Rust Book: 
1. [ownership](https://doc.rust-lang.org/book/ch04-01-what-is-ownership.html)
2. [References and Borrowing](https://doc.rust-lang.org/book/ch04-02-references-and-borrowing.html)

# methods

1. [as_mut](https://doc.rust-lang.org/std/primitive.pointer.html#method.as_mut): Returns None if the pointer is null, or else returns a unique reference to the value wrapped in Some.

2. [as_ref](https://doc.rust-lang.org/std/primitive.pointer.html#method.as_ref): Returns None if the pointer is null, or else returns a shared reference to the value wrapped in Some.

3. [unwrap](https://doc.rust-lang.org/std/option/enum.Option.html#method.unwrap): Returns the contained Some value, consuming the self value.

3. [take](https://doc.rust-lang.org/core/option/enum.Option.html#method.take): Takes the value out of the option, leaving a None in its place.

# module

1. [clone](https://doc.rust-lang.org/std/clone/index.html): when you assign them or pass them as arguments, the receiver will get a copy, leaving the original value in place.

2. [boxed](https://doc.rust-lang.org/std/boxed/index.html):The Box<T> type for heap allocation.

3. [option](https://doc.rust-lang.org/std/option/index.html): represents an optional value: every Option is either Some and contains a value, or None, and does not.

# enum

1. [Option](https://doc.rust-lang.org/std/option/enum.Option.html#)

# Other discussions

https://www.reddit.com/r/rust/comments/g3oqjk/please_help_me_get_rid_of_as_refas_refunwrap/