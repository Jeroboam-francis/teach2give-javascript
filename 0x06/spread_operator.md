# SPREAD OPERATOR

The spread operator (...) allows you to expand elements of an iterable (like arrays, objects, or strings) into individual elements.

## Use Cases of The Spread Operator

1. Copying Arrays

The spread operator can be used to copy array elements, which helps avoid mutate the original array.

```js

 const original = [1, 2, 3];
const copy = original;

copy.push(55);
```

```js
const original = [1, 2, 3];
const copy = [...original];
```

2. Merging Arrays

```js

const obj1 = { name: "John" };
const obj2 = { age: 25 };
const merged = { ...obj1, ...obj2 };

console.log(merged); //  { name: "John", age: 25 }
```

3. Overwriting Properties

```js
const user = { name: "John", role: "User" };
const updatedUser = { ...user, role: "Admin" };

console.log(updatedUser); // { name: "John", role: "Admin" }
```