JavaScript is a really important language and has really easy syntax.

You use `console.log()` to log stuff to the console, it's basically the `print()` function but for JavaScript.  
<ins>**console.log() is a function that prints data types to the console**</ins>

---

To make a comment you use `//` for a single line comment, and `/* ... */` for a multi-line comment, like `/* start` on one line and `stop */` on another.

---

Now the data types in JavaScript are:
Number, String, Boolean, Undefined and Null. The rest are used less often, but it's good to know they exist: BigInt and Symbol. There's also Object, which you'll actually use all the time (arrays and functions are objects too).

---

## Variables: there are actually 3 ways to declare a variable

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

# Operators in javascript are

`+` Addition

`-` Subtraction

`*` Multiplication

`**` Exponentiation

`/` Division

`%` Modulus (Division Remainder)

`++` Increment

`--` Decrement

### Here's a quick example

```js
// Arithmetic operators
console.log(10 + 3); // 13
console.log(10 - 3); // 7
console.log(10 * 3); // 30
console.log(10 ** 3); // 1000 (exponent)
console.log(10 / 3); // 3.3333333333333335
console.log(10 % 3); // 1 (remainder)

// Increment: x++ returns the old value, then adds 1
let x = 5;
console.log(x++); // 5
console.log(x); // 6

// ++y adds 1 first, then returns the new value
let y = 5;
console.log(++y); // 6

// Decrement: z-- returns the old value, then subtracts 1
let z = 5;
console.log(z--); // 5
console.log(z); // 4

// --w subtracts 1 first, then returns the new value
let w = 5;
console.log(--w); // 4
```

### This will be the output

```js
13;
7;
30;
1000;
3.3333333333333335;
1;
5;
6;
6;
5;
4;
4;
```

---

# Libraries

_you can install libraries using the node package manager which is `npm` now that you installed a library you want to import it to you're file to import in ES6 you can type this at the top of your file like this:_

```js
import { functionName } from "library-name";
```
