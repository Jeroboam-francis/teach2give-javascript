# STRING  CONCATENATION

Process of joining tow or more strings together.

There are several ways of concetenation including using the `+` operator, the `concat` method, and the `template literals` (backticks)

## 1. Using the `+` operator

```javascript

let firstName = "Jeroboam";
let lastName = "Francis";

let fullName = firstName + " " + lastName;

console.log(" My full name is " fullName);
// output My full name is Jeroboam Francis

```

## 2. Using the `+='` operator

```javascript
let message = "Hello";
message += " World";

console.log(message);
// output Hello World

```

## 3. Using Template Literals (Backticks(`)  and ($ {} ) placeholder)

```javascript

let firstName = "Jeroboam";
let lastName = "Francis";
console.log(` my name is ${firstNam} ${lastName}`);
// output my name is Jeroboam Francis

```
