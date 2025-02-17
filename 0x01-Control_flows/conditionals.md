# CONDITIONALS
Conditionals allow one to excute different  blocks of code based on a condition.

They include `if`, `else if`, and `switch` statements and `if else` ladder.

#### if statement 
Used to excute block of code if a specified condition is true.

The syntax is 

```javascript
if (condition) {
    // block of code to be executed if condition is true
}
```
Example in code

```javascript
let books = 10;

if (books > 9) {
    console.log ("there are more than 9 books");
    
}
```

#### if else statement

Used to excute block of code if a specified condition is true and if its false excute another block of code in else block

The syntax is

```javascript
if (condition) {
    // block of code to be executed if condition is true
} else {
    // block of code to be executed if condition is false
}
```

Example in code

```javascript
let books = 10;

if (books > 9) {
    console.log ("there are more than 9 books");
    
} else {
    console.log ("there are less than 9 books");
}
``` 

#### else if statement

Used when multiple conditions need to be evaluated sequentially.

The syntax is

```javascript
if (condition1) {
    // block of code to be executed if condition1 is true
} else if (condition2) {
    // block of code to be executed if condition2 is true
} else {
    // block of code to be executed if none of the above conditions are true
}
``` 

Example in code

```javascript
let marks = 100;

if (marks > 90) {
    console.log ("A");
    
} else if (marks > 80) {
    console.log ("B");
} else if (marks > 70) {
    console.log ("C");
} else {
    console.log ("D");
}
``` 
#### switch statement

Used to excute block of code based on different cases.

The syntax is   

```javascript
switch (expression) {
    case value1:
        // block of code to be executed if expression is equal to value1
        break;
    case value2:
        // block of code to be executed if expression is equal to value2
        break;
    case value3:
        // block of code to be executed if expression is equal to value3
        break;
    default:
        // block of code to be executed if none of the above cases are true
        break;
}
``` 

Example in code

```javascript
let marks = 100;

switch (marks) {
    case 100:
        console.log ("A");
        break;
    case 90:
        console.log ("B");
        break;
    case 80:
        console.log ("C");
        break;
    case 70:
        console.log ("D");
        break;
    default:
        console.log ("F");
        break;
}
```
#### Ternary operator
Provides a shorter way to write if else statements in a single line

The syntax is

```javascript
(condition) ? expression1 : expression2;
```

Example in code

```javascript
let marks = 100;

(marks > 90) ? console.log ("A") : console.log ("B");
```

