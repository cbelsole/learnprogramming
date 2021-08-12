# Lesson 1 - Variables and operators

## Variables hold information

In JavaScript we use variables to hold onto information. Previously we learned about `console.log()` which outputs information to the terminal. If I wanted to tell you how old I am I could say:

```js
console.log("I am 34")
```

This works perfectly fine now, but this does not work for me next year. Let's say we extracted out the age to a variable.

```js
var age = 34

console.log("I am", age)
```

Now we have the age extracted out into a variable (`var`) called `age` that holds an `integer` (whole number) with my current age. Let's make that dynamic.

```js
var birthYear = 1987
var currentYear = new Date().getFullYear()
var age = currentYear - birthYear

console.log("I am", age)
```

The above program now ticks away every year telling me I am one year older. There are a few new things going on here.

1. `new Date()` is the JS way to create a date/time object. Here we are pulling the year out of it with `getFullYear()`.
2.  `currentYear - birthYear` introduces our first operator; the `-` sign representing subtraction. There are many more [operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators) in JS which do everything from math (`-`, `+`, `/`, `*`) to comparisons (`>`, `<`, `===`) and beyond.
3.  With the `age` variable we can see that variables can be used to set other variables. There is an order of operations when the computer reads a line of code. on line 3 we are asking the computer to compute the value of `currentYear - birthYear` and then store that value in `age`. This logic will get more complex in the future. So knowing how the computer reads your code will help you sidestep bugs later.

## Resources about variables:
* 📖 [MDN: Grammar and Types - variables](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_Types#variables)
* 🎮 [FCC: Declare Javascript Variables](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/declare-javascript-variables)
* 🎥 [FCC: Declare JavaScript Variables](https://www.youtube.com/watch?v=5mFKY3AhYPo)

## Resources about operators:

* 📖 [MDN: Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
* 🎮 [W3S: JavaScript Operators](https://www.w3schools.com/js/js_operators.asp)
* 🎥 [Different Types of Operators in JavaScript](https://www.youtube.com/watch?v=FZzyij43A54)
