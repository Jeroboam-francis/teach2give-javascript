# FUNCTIONS

A Function is a block of code that performs a specific task. They are first-class citizens meaning they can be passed as arguments to other functions and can be returned from other functions.

Basic syntax

```javascript
function functionName(parameters) {
  // code to be executed
}
```

Example

```javascript
function sayHello(name) {
  console.log("Hello " + name);
}
// calling a function
sayHello("John");
```

## Parameters and Arguments

Parameters are the variables listed inside the parentheses in the function definition and act as placeholders for the values that are passed into the function when it is called.

Arguments are the values that are passed into the function when it is called.

example

```javascript
function sayHello(name) {
  // name is a parameter
  console.log("Hello " + name);
}
// calling a function
sayHello("Jeroboam"); // jeroboam is an argument
```

## Function Return Values

A function can return a value using the return keyword.

```javascript
function add(a, b) {
  return a + b;
}
let sum = add(5, 10);
console.log(sum);
// output
15;
```

## Categories of Functions

1. Functions that don't take parameter(S) and don't return a value
2. Functions that don't take parameter(S) but return a value
3. Functions that take parameter(S) and return a value
4. Functions that take parameter(S) but don't return a value

### 1. Functions that don't take parameter(S) and don't return a value

This functions don't take parameter(S) and don't return a value

```javascript
function add() {
  let x = 10;
  let y = 20;
  console.log(x + y);
}
add();
```

#### 2. Functions that don't take parameter(S) but return a value

This functions don't take parameter(S) but return a value

```javascript
function add() {
  let x = 10;
  let y = 20;
  return x + y;
}
console.log(add());
```

#### 3. Functions that take parameter(S) and return a value

This functions take parameter(S) and return a value

```javascript
function add(a, b) {
  return a + b;
}
console.log(add(10, 20));
```

#### 4. Functions that take parameter(S) but don't return a value

This functions take parameter(S) but don't return a value

```javascript
function add(a, b) {
  console.log(a + b);
}
add(10, 20);
```

## Types of functions in JavaScript

1. Function declaration
2. Function expression/ anonymous functions
3. Arrow functions
4. Immediately Invoked Function Expression (IIFE)
5. Callback functions

### 1. Function declaration

```javascript
function add(a, b) {
  console.log(a + b);
}
add(10, 20);
```

#### 2. Function expression/ anonymous functions

```javascript
let add = function (a, b) {
  console.log(a + b);
};
add(10, 20);
// involves saving a function to a variable
```

#### 3. Arrow functions

Used to simplify functions and the way they are written

```javascript
let add = (a, b) => {
  return a + b;
};

console.log(add(10, 20));
```

i. If the function has only one parameter, the parentheses can be omitted

```javascript
let add = (a) => {
  return a + b;
};
```

ii. If an arrow function has only one line of code, the curly braces can be omitted

```javascript
let add = (a, b) => {
  console.log(a + b);
};
add(10, 20);
```

this can be written as

```javascript
let add = (a, b) => console.log(a + b);
```

iii. If an arrow function has only one line of code in the body and that line happens to be a return statement, we can get rid of the return keyword

```javascript
let add = (a, b) => a + b;
console.log(add(10, 20));
```

#### 4. Immediately Invoked Function Expression (IIFE)

Invoked immediately means that the function is executed as soon as it is defined.

```javascript
(function (a, b) {});
```

They can also take parameters

```javascript
(function (a, b) {
  let sum = a + b;
  let product = a * b;
  console.log("the sum of ${a} and ${b} is ${sum}");
  console.log("the product of ${a} and ${b} is ${product}");
})(10, 20);
```

#### 5. Callback functions

A function that is passed as an argument to another function is known as a callback function.

```javascript

function greet (name) {
    console.log("Hello " + name);
    callback();
}
greet ("Jeroboam". function callback () {
    console.log("Goodbye");
});

```
