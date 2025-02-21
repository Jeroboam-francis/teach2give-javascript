# WHATS ES6

ES6 is a new version of JavaScript. It is a superset of JavaScript and adds new features to the language.

## LETS AND CONST FOR BLOCK SCOPED VARIABLES









# Destructuring
Last modified: 19 February 2025
Destructuring is a convenient way to extract values from arrays or objects and assign them to variables in a single line.

## Destructuring arrays
```js

const numbers = [1, 2, 3];
const [first, second, third] = numbers;

console.log(first); // 1
console.log(second); // 2
console.log(third); // 3
```

We can also skip values when destructuring:
```js

const numbers = [1, 2, 3];
const [, , third] = numbers;

console.log(third); // 3
We can use the rest operator to collect remaining elements into an array during destructuring:

const numbers = [1, 2, 3, 4, 5, 6, 7];
const [first, second, ...others] = numbers;
console.log(others); // [ 3, 4, 5, 6, 7 ]
We can also use destructuring to swap variables:

let a = 1, b = 2;

[a, b] = [b, a];

console.log(a); // 2
console.log(b); // 1
```



