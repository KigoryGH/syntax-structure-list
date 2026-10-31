JavaScript is a really important language and has really easy syntax.

You use `console.log()` to log stuff to the console, it's basically the `print()` function but for JavaScript.  
<ins>**console.log() is a function that prints data types to the console**</ins>

---

To make a comment you use `//` for a single line comment, and `/* ... */` for a multi-line comment, like `/* start` on one line and `stop */` on another.

---

Now the data types in JavaScript are:
Number, String, Boolean, Undefined and Null. The rest are used less often, but it's good to know they exist: BigInt and Symbol. There's also Object, which you'll actually use all the time (arrays and functions are objects too).

---

Variables: there are actually 3 ways to declare a variable.

| Keywords to declare a variable                                                                         |
| ------------------------------------------------------------------------------------------------------ |
| `var` _it's the old way to declare a variable_                                                         |
| `const` _declares a constant variable that never changes, to protect yourself from your own stupidity_ |
| `let` _declares a variable that "lets" you change it, unlike const_                                    |

note: _you'll never use `var` because it's old and outdated, but you'll be using `const` and `let`, and especially `const` because things can get messy in codebases. If you need to change the variable, use `let`._

---

Here is a table so you can understand better

| Data types | use                                                |
| ---------- | -------------------------------------------------- |
| String     | `console.log("quotes make a string")`              |
| Number     | `console.log(10) // as the name says a number`     |
| Null       | `let something = null // now something is nothing` |

---

Operators in javascript are:

- Addition

- Subtraction

- Multiplication
  ** Exponentiation
  / Division
  % Modulus (Division Remainder)
  ++ Increment
  -- Decrement
