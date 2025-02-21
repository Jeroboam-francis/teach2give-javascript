# OBJECTS

Arrays is a collection of elements

## Creating Objects

1. Object literal
2. new object constructor
3. array constructor

### 1. Object literal

use of curly braces

```js
const students = {
  firstName: "jeroboam",
  lastName: "james",
  age: 25,
  location: "lagos",
  greet: function () {
    console.log("Hello " + this.firstName);
  },
  // output: Hello jeroboam
};
```

### 2. new object constructor

creates an empty object and returns the reference to it

```js
const students = new Object();
student.firstName = "jeroboam";
student.lastName = "francis";
student.age = 25;
student.location = "lagos";
student.greet = function () {
  console.log("Hello " + this.firstName);
  //output: Hello jeroboam
};
```

### 3. array constructor

creates multiple objects with shared properties and methods

```js
function Student(firstName, lastName, age, location) {
  this.firstName = firstName;
  this.lastName = lastName;
  this.age = age;
  this.location = location;
  this.greet = function () {
    console.log("Hello " + this.firstName);
  };
}

const student1 = new Student("jeroboam", "francis", 25, "lagos");
```

## Accessing Object Properties

i. dot
ii. bracket

i. dot

allows access to an object property using the dot followed by the property name

```js
const student1 = {
  firstName: "jeroboam",
  lastName: "francis",
  age: 25,
  location: "lagos",
  greet: function () {
    console.log("Hello " + this.firstName);
  },
};
console.log(student1.firstName);
//output: jeroboam
console.log(student1.lastName);
//output: francis"];
```

ii. bracket

allows access to an object property using the bracket followed by the property name

```js
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

console.log(student["firstName"]); // John
console.log(student["lastName"]); // Doe
console.log(student["age"]); // 25
console.log(student["isStillStudying"]); // true
```

## Modifying Object Properties

Adding new properties
You can use the dot or bracket notation to add new properties to an object.

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

student.major = "Computer Science";
student["graduationYear"] = 2026;
```

## Updating a property

You can also use dot or bracket notation to update object's properties.

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

student.age = 37;
student["isStillStudying"] = false;
```

## Deleting a property

Use the delete keyword to delete a property.

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

delete student.age;
delete student.isStillStudying;
```

## Checking properties in an object

To check if a certain property is available in an object, you can use:

The in keyword.

The hasOwnProperty() method.

### The `in` keyword

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

console.log("firstName" in student); // true
console.log("middleName" in student); // false
```

### The hasOwnProperty() method

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

console.log(student.hasOwnProperty("firstName")); // true
console.log(student.hasOwnProperty("middleName")); // false
```

### Object Methods

`Object.keys(objectName)`

Returns an array containing all the keys of an object.

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

console.log(Object.keys(student));
// [ 'firstName', 'lastName', 'age', 'isStillStudying', 'greet' ]
```

`Object.values(objectName)`

Returns an array containing all the values of an object.

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

console.log(Object.values(student));
// [ 'John', 'Doe', 25, true, [Function: greet] ]
```

`Object.entries(objectName)`

Object.entries() returns an array of key-value pairs from an object, making it useful for iteration.

```javascript
const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

console.log(Object.entries(student));
// [
//     [ 'firstName', 'John' ],
//     [ 'lastName', 'Doe' ],
//     [ 'age', 25 ],
//     [ 'isStillStudying', true ],
//     [ 'greet', [Function: greet] ]
// ]
```

`Object.freeze(objectName)`

Freezes an object, preventing new properties from being added to it and existing ones from being removed, it also prevents an object from modification.

```javascript

const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

Object.freeze(student);
student.middleName = "Smith"; // won't work
Iterating over an object using the for..in loop﻿
You can use the for..in loop to iterate over an object as shown:

const student = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  isStillStudying: true,
  greet: function () {
    console.log("Hello, World!");
  },
};

for (let key in student) {
  console.log(key)
}
```

The for..in loop can also be used to loop over arrays.
