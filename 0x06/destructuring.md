# Destructuring objects 

```js

const person = {
  name: "Alice",
  age: 25,
};

const { name, age } = person;

console.log(name); // Alice
console.log(age); // 25
```

You can also rename variables when destructuring objects:

```js

const person = {
  name: "Alice",
  age: 25,
};

const { name: firstName, age: yearsSinceBirth } = person;

console.log(firstName); // Alice
console.log(yearsSinceBirth); // 25

```

You can assign default value if the variable doesn't exist in an object:

```js

const person = {
  name: "Alice",
  age: 25,
};

const {
  name: firstName,
  age: yearsSinceBirth,
  major = "Computer Science",
} = person;

console.log(firstName); // Alice
console.log(yearsSinceBirth); // 25
console.log(major); // Computer Science

```
We can use the rest operator to gather the remaining properties of an object during destructuring:

```javascript
const person = {
  firstName: "Alice",
  lastName: "Doe",
  dateOfBirth: 2000,
  major: "Computer Science",
  profession: "Web Developer",
};

const { firstName, lastName, ...otherDetails } = person;
console.log(otherDetails);
// {
//   dateOfBirth: 2000,
//   major: 'Computer Science',
//   profession: 'Web Developer'
// }
```

