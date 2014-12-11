# Intro to Rust

## Ownership

Ownership is a property of a type

## Borrowing

Represented by the `&` sigil

Only valid for a particular lifetime (similar to scope)

## Memory Management

you can say when memory is allocated and deallocated. You don't _NEED_ to
dealloc

Rust will dealloc when something goes out of scope

    fn main() {
      let myvar = box 3i;
    }
    // myvar is deallocated because it's out of scope

Also uses reference counting to do this

## Mutability

property of a type

    let mute a = A

## Concurency

Because of ownership and borrowing, concurrency is safe

## Traits

Similar to types in Haskell

## Unsafe blocks

Turns off some compile time checks. Can't do everything you want within Rust,
but they account for that with unsafe blocks

## What rust is good at

- large scale maintainable systems
- embedded in other languages
- fast, correct code
