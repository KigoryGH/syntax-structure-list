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

## Data types by example

| Data types | use                                                |
| ---------- | -------------------------------------------------- |
| String     | `console.log("quotes make a string")`              |
| Number     | `console.log(10) // as the name says a number`     |
| Null       | `let something = null // now something is nothing` |

---

## Operators

| Operator | Name                         |
| -------- | ---------------------------- |
| `+`      | Addition                     |
| `-`      | Subtraction                  |
| `*`      | Multiplication               |
| `**`     | Exponentiation               |
| `/`      | Division                     |
| `%`      | Modulus (division remainder) |
| `++`     | Increment                    |
| `--`     | Decrement                    |

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

```text
13
7
30
1000
3.3333333333333335
1
5
6
6
5
4
4
```

---

## Libraries

_You can install libraries using the Node package manager, which is `npm`. Once a library is installed, you import it into your file. To import with ES modules, type this at the top of your file:_

```js
import { functionName } from "library-name";
```

### Here's an example of using a library

I'm going to use `chalk`.

First, set up a project and download the library:

```bash
npm init -y
npm install chalk
```

Then open the `package.json` file that `npm init` created and add `"type": "module"` to it, so Node understands the `import` syntax.

Now make a file called `fileName.js` and paste the code below to print hello world in blue:

```js
import chalk from "chalk";

console.log(chalk.blue("Hello world!"));
```

`chalk` is a default export, which is why there are no curly braces around it.

Run it with:

```bash
node fileName.js
```

Now go to <https://www.npmjs.com/package/chalk>, look at the documentation, and try to mess around with it so you can get the feel of JavaScript a little.

---

# Statements and Declarations

| control flow | description                                                                                                                       |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------- |
| return       | returns a value from the function (basically `yeild` in python)                                                                   |
| break        | stops the current loop, switch, or label statement and transfers program control to the statement following the stopped statement |
| if...else    | an `if` statment but with another condition                                                                                       |
| switch       | Evaluates an expression, matching the expression's value to a case clause, and executes statements associated with that case.     |

There are a lot of those but these are just the most used (personally)

## _Iterations_

now these are ones that are mandatory the ones that you will use 100% in any project.

| iterations       | description                                                                                                                      |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `do...while`     | Runs a statement until the condition is false. The condition is checked after each run, so the statement executes at least once. |
| `for`            | Loop with three optional expressions in parentheses, separated by semicolons, followed by the statement to run.                  |
| `for...in`       | Iterates over an object's enumerable properties in arbitrary order, running the statement for each one.                          |
| `for...of`       | Iterates over iterable objects (arrays, array-like objects, iterators and generators), running the statement for each value.     |
| `for await...of` | Iterates over async iterable objects, array-like objects, iterators and generators, running the statement for each value.        |
| `while`          | Runs a statement as long as the condition is true. The condition is checked before each run.                                     |
