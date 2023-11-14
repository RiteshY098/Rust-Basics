# Rust-Basics
  Rust Programming Language Basics  .container { max-width: 800px; margin: 0 auto; } h1 { text-align: center; }

Rust Programming Language Basics
================================

Rust is a systems programming language sponsored by Mozilla Research. It is designed to be safe, concurrent, and fast. Rust is a relatively new language, but it has quickly gained popularity among programmers due to its unique features.

Getting Started with Rust
-------------------------

Before you can start writing Rust code, you need to install the Rust compiler and tooling. The easiest way to do this is to use the Rust installer, which is available for Windows, macOS, and Linux. Once you have installed Rust, you can open a terminal window and type \`rustc\` to check that it is installed correctly.

First Rust Program
------------------

The traditional first program in any language is "Hello, World!", and Rust is no exception. Here is a simple Rust program that prints "Hello, World!" to the console:

    fn main() {
        println!("Hello, World!");
    }
        

Data Types
----------

Rust is a statically typed language, which means that the type of each variable must be declared before it is used. There are many different data types in Rust, including integers, floats, strings, and booleans. Here are some examples of how to declare variables of different data types:

    let x: i32 = 10; // An integer variable
    let y: f64 = 3.14; // A floating-point variable
    let z: &str = "Hello, World!"; // A string variable
    let is\_true: bool = true; // A boolean variable
        

Variables and Mutability
------------------------

Variables in Rust can be either mutable or immutable. Mutable variables can be changed after they are declared, while immutable variables cannot. By default, variables in Rust are immutable. Here is an example of how to declare a mutable variable:

    let mut x = 10;
    x = 20;
        

Control Flow
------------

Rust has several control flow statements, including \`if\`, \`else\`, \`for\`, and \`while\` loops. Here is an example of how to use an \`if\` statement:

    if x > 10 {
        println!("x is greater than 10");
    }

Here is an example of how to use a \`for\` loop:

    for i in 1..11 {
        println!("i is {}", i);
    }
            

Functions
---------

Functions are blocks of code that can be reused. Here is an example of how to define a function in Rust:

    fn greet(name: &str) {
        println!("Hello, {}!", name);
    }
            

This function takes a string as an argument and prints a greeting to the console.

Modules
-------

Modules are used to organize code into reusable units. Here is an example of how to define a module in Rust:

    mod myModule {
        pub fn greet(name: &str) {
            println!("Hello, {}!", name);
        }
    }

This module defines a function called \`greet()\`. The \`pub\` keyword makes the function available to other modules.

Error Handling
--------------

Errors are an inevitable part of programming.

    fn main() {
        let result = divide(10, 0);
        match result {
            Ok(result) => println!("The result is {}", result),
            Err(error) => println!("Error: {}", error),
        }
    }
    fn divide(x: i32, y: i32) -> Result {
        if y == 0 {
            return Err("Cannot divide by zero".to\_string());
        }
        Ok(x / y)
    }
    

The output of this code is:

Error: Cannot divide by zero
