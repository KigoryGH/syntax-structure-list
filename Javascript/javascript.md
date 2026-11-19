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

## Statements and declarations

### Control flow

| Control flow | Description                                                                                 |
| ------------ | ------------------------------------------------------------------------------------------- |
| `return`     | sends a value back out of a function (same idea as `return` in Python)                      |
| `break`      | stops the current loop or `switch` and jumps to the code right after it                     |
| `if...else`  | runs one block of code if a condition is true, and another block if it isn't                |
| `switch`     | compares a value against a list of `case` options and runs the code of the one that matches |

There are a lot more of those, but these are just the most used ones (personally).

### Iterations

Now these are the loops you'll see in almost every project.

| Iterations       | Description                                                                                                                  |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `do...while`     | runs the code, then checks the condition and repeats while it's true, so it always runs at least once                        |
| `for`            | the classic loop: three optional parts in parentheses separated by semicolons (setup, condition, step), then the code to run |
| `for...in`       | loops over the keys (property names) of an object, in no guaranteed order                                                    |
| `for...of`       | loops over the values of something iterable, like an array or a string                                                       |
| `for await...of` | like `for...of` but for async iterables (rare, you won't need it until you learn async code)                                 |
| `while`          | checks the condition first and keeps running the code as long as it's true                                                   |

---

Now if you're a little experienced you should be able to read these tables and understand everything you need, but if you want something more in-depth you can visit this great documentation:
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements>

_(I heavily recommend contributors add more to this because I'm just too lazy to do that)_

---

## Arrays

Here is how an array is structured in JavaScript:

```js
const arrayName = [value1, value2, value3, value4];
```

To make an array you usually use `const`, then pick a name for your array, and type your values between the brackets `[]`, separated by commas.

Here is an example:

```js
const myArray = [1, 2, 3, 4]; // This is an array with the numbers from 1 to 4

// Arrays are zero-indexed, so index 0 is the first item.
// Here index 0 holds the value 1
console.log(myArray[0]);
```

Here's a little image I had Gemini make me:

<img width="700" height="350" alt="image" src="github.com/KigoryGH/syntax-structure-list/main/jsArrays.jpg" />

---

Output:

```text
1
```
