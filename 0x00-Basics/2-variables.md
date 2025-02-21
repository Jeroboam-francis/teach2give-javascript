# VARIABLES

In programming, a variable is a named container that can hold data of different types. It allows you to store and manipulate values at different points in your code.

## DECLARING VARIABLES AND INIZIALIZING VARIABLES

### 1.DECLARING VARIABLES

To declare a variable in JavaScript, you can use the `var`, `let`, or `const` keywords. For example:

```javascript

// Declare a variable
var x = 5; // not recommended for modern coding
let y = 10; // Holds a changing variable
const z = 15; // holds a constant
```

In the above example, `x`, `y`, and `z` are variables that hold the values `5`, `10`, and `15`, respectively.

### UPDATING VARIABLES

The values of `let` can be updated while `const` cannot be updated

```javascript
// Update a variable
let y = 10
y = 20
```

the value of y now is 20

A variable can be created without assigning a value  to it which communicates that a variable exists but doesnt have a value yet and you can update it later

```javascript
// Create a variable without assigning a value

let z;
console.log(z); 

// the output is going to be undefined
```

updating it later

```javascript
// Update a variable
let cows;
cows = 10;
console.log(cows); 

// the output is going to be 10
```

### 2.INITIALIZING VARIABLES

Refer to the previous section for declaring variables. To initialize a variable, you can assign a value to it. For example:

```javascript
// Initialize a variable       

let cows = 10;
console.log(cows);

// the output is going to be 10    

```

## RULES FOR NAMING VARIABLES

1. Variable names should be descriptive and meaningful
and when one uses multiple words they should use this cases below

### a. Camel convention

```javascript
// Camel convention
let numberOfCows = 10;
let numberOfBoys = 10;

```

#### b. Pascal convention

```javascript
// Pascal convention
let NumberOfCows = 10;
let NumberOfBoys = 10;

```

#### c. Snake convention

```javascript
// Snake convention

let number_of_cows = 10;
let number_of_boys = 10;

```

Most commonly used is `camel case` thus a recommended one

2.Variables names can only start with a letter, underscore, or dollar sign.

EXAMPLE

```javascript
// underscore, dollar sign and letter
// valid example
let _cows = 10;
let $cows = 10;
let cows = 10;
```

```javascript
// invalid example
let 1cows = 10;
let #cows = 10;
let @cows = 10;

```

3.Variables names are case-sensitive

```javascript
// case-sensitive example 

let cows = 10;
console.log(cows);

// the output is going to be 10

let Cows = 200;
console.log(Cows);

// the output is going to be 200

```

4.Variables names should not be reserved words

```javascript
//wrong use of reserved words
let var = 10;
let let = 10;
// this is wrong 
```
