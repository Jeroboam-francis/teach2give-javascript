# FUNCTIONS
A Fuction is a block of code that performs a specific task. They are first-class citizens meaning they can be passed as arguments to other functions and can be returned from other functions.

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
// calling a fuction
sayHello("John");
```

## Parameters and Arguments

Parameters are the variables listed inside the parentheses in the function definition and act as placeholders for the values that are passed into the function when it is called.

Arguments are the values that are passed into the function when it is called.

example
```javascript
function sayHello(name) {// name is a parameter
    console.log("Hello " + name);
}
// calling a fuction
sayHello("Jeroboam");// jeroboam is an argument

```
## Fuction Return Values
A fuction can return a value using the return keyword.

```javascript
function add (a, b) {
    return a + b;
}
let sum =add (5, 10);
console.log(sum);
// output
15
```
## Categories of Fuctions

1. Fuctions that don't take parameter(S) and dont returm a value
2. Fuctions that don't take parameter(S) but return a value
3. Fuctions that take parameter(S) and return a value
4. Fuctions that take parameter(S) but don't return a value

#### 1. Fuctions that don't take parameter(S) and dont returm a value
This functions don't take parameter(S) and dont returm a value

```javascript
function add () {
    let x = 10;
    let y = 20;
    consolw.log (x+y);
}
add();

```
#### 2. Fuctions that don't take parameter(S) but return a value
This functions don't take parameter(S) but return a value

```javascript
function add () {
    let x = 10;
    let y = 20;
    return x+y;
}
console.log(add());
```
#### 3. Fuctions that take parameter(S) and return a value
This functions take parameter(S) and return a value

```javascript
function add (a, b) {
    return a + b;
}
console.log(add(10, 20));
```
#### 4. Fuctions that take parameter(S) but don't return a value
This functions take parameter(S) but don't return a value

```javascript
function add (a, b) {
    console.log(a + b);
}
add(10, 20);
```

## Types of fuctions in JavaScript

1. Fuction declaration
2. Fuction expression/ anonymous functions
3. Arrow functions
4. Immedietly Invoked Fuction Expression (IIFE)
5. Callback functions

#### 1. Fuction declaration

```javascript
function add (a, b) {
    console.log(a + b);

}
add (10, 20);

```
#### 2. Fuction expression/ anonymous functions

```javascript
let add = function (a, b) {
    console.log(a + b);
}
add (10, 20);
// involves saving a function to a variable
```

#### 3. Arrow functions
Used to simplify fuctions and the way they are written

```javascript

let add = (a, b) => {
    return a + b;
}

console.log(add(10, 20));
```
i. If the function has only one parameter, the parentheses can be omitted

```javascript

let add = a => {
    return a + b;
}
```
ii. If an arrow function has only one line of code, the curly braces can be omitted

```javascript
let add = (a, b) => { 
    console.log(a + b);

}
add (10, 20);
```
this can be written as 

```javascript
let add = (a, b) => console.log(a + b);
```

iii. If an arrow functio has only one line of code in the body and that line happens to be a return statement, we can get rid of the return keyword
```javascript
let add = (a, b) => a + b;
console.log(add(10, 20));

```

#### 4. Immedietly Invoked Fuction Expression (IIFE)

Invoked immedietly means that the function is executed as soon as it is defined.

```javascript

(function (a, b) {
    
})
```

They can also take parameters
```javascript

(function (a, b) {
    let sum = a + b;
    let product = a * b;
    console.log('the sum of ${a} and ${b} is ${sum}');
    console.log('the product of ${a} and ${b} is ${product}');
    
}) (10, 20);

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

