# DATA STRUCTURES

This is a way of organizing data so that it can be accessed and used efficiently.

## Basic Data Structures

1. Array
2. Object
3. Map
4. Sets

### 1. arrays

Collection of elements at contiguous memory location

#### Creating Arrays

There are two types

##### an array literal

example

```javascript
const students = ["jeroboam", "james", "john"];

```

##### new array  constructor

```javascript
const students = new Array("jeroboam", "james", "john");

```

multidimensional arrays

```javascript
const students = [
    ["jeroboam", "james", "john"],
    ["james", "john", "jeroboam"],
    ["john", "jeroboam", "james"],
]
```

#### Accessing Array Elements

we access using index numbers

```javascript
const students = ["jeroboam", "james", "john"];
console.log(students[0]);

// output : jeroboam 

```

#### Basic Array methods

1. length

Length is the number of elements in an array.

```javascript
const students = ["jeroboam", "james", "john"];
console.log(students.length);
// output : 3

2.pop()

Removes the last element from an array and returns that element.

```javascript
const students = ["jeroboam", "james", "john"];
console.log(students.pop());
// output : john

```

3.push()

Adds one or more elements to the end of an array and returns the new length.

```javascript
const students = ["jeroboam", "james", "john"];
students.push("james");
console.log(students);

// output : ["jeroboam", "james", "john", "james"]
```

4.shift()

Removes the first element from an array and returns that element.

```javascript
const students = ["jeroboam", "james", "john", "jack"];
students.shift();
console.log(students);
// output: ["james", "john", "jack"]

```

5.unshift()

Adds one or more elements to the beginning of an array and returns the new length.

```javascript
const students = ["james", "john", "jack"];
students.unshift("jeroboam", "Francis");
console.log(students);
// output: ["jeroboam", "francis", "james", "john", "jack"]

```

6.at()

Returns the element at the specified index in an array.

```javascript
const students = ["jeroboam", "james", "john", "jack"];
console.log(students.at(2));
// output: "john"
```

7.toLocaleString()

Returns a string representation of an array.

```javascript
const students = ["jeroboam", "james", "john", "jack"];
console.log(students.toLocaleString());
// output: "jeroboam,james,john,jack"
```

8.join ()

Returns a string representation of an array and you can specify the separator.

```javascript
const students = ["jeroboam", "james", "john", "jack"];
console.log(students.join("+++ "));
// output: "jeroboam+++ james+++ john+++ jack"

```

9 concat()

Returns a new array containing the elements of the first array followed by the elements of the second array.

```javascript
const students = ["jeroboam", "james", "john", "jack"];
const newStudents = ["james", "john", "jack"];
console.log(students.concat(newStudents));
// output: ["jeroboam", "james", "john", "jack", "james", "john", "jack"]
```

10 flat()

converts a multidimensional array into a one-dimensional array.

```javascript
const students = [
    ["jeroboam", "james", "john", "jack"];
    ["Amos", "john", "jack"];
]
console.log(students.flat());
//output: []
```

11 reverse
Reverses the elements of an array.

```javascript

const students = ["John", "Ken", "June", "Jack"];
console.log(students.reverse());
```
