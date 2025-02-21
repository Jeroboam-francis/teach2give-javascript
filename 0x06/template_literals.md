# TEMPLATE LITERALS

makes working with strings easier flexible and readable and they allow

- multi-line strings
- string interpolation
- embedding expressions

## multi-line strings

before

```javascript
const multiLine = "This is line 1\n" + "This is line 2\n" + "This is line 3";

console.log(multiLine);
/*
This is line 1
This is line 2
This is line 3
*/
```

after

```js
const multiLine = `This is line 1
This is line 2
This is line 3`;

console.log(multiLine);
/*
This is line 1
This is line 2
This is line 3
*/
```

### String interpolation: Injecting variables into strings

Before, we had to use the `+` operator for string concatenation (+), which was cumbersome.

before

```js
const username = "Dennis";
const age = 25;

console.log("My name is " + username + " and I am " + age + " years old.");
// My name is Dennis and I am 25 years old.
```

after

```js
const name = "Dennis";
const age = 25;

console.log(`My name is ${name} and I am ${age} years old.`);
// My name is Dennis and I am 25 years old.
```

### Expressions inside template literals

Template literals can evaluate expressions directly inside ${}.
before

```js
let a = 10;
let b = 20;

function product(number1, number2) {
  return number1 * number2;
}

console.log(
  `The sum of ${a} and ${b} is ${a + b} and the product is ${product(a, b)}`
);
```

