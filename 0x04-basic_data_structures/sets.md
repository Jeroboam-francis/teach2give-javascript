# SETS

Data structure that represents a collection of unique values

## Properties of a set

- uniques elements
- no indexing
- no order

## creating a set

we use `new set ()`

```js
const mySet = new Set(1, 2, "a", "jeroboam", "james");
console.log(mySet);
```

## Set methods

- add(value)

Adds new element with the specified value to the set

```js
const mySet = new Set();
mySet.add(1);
mySet.add(2);
mySet.add("a");
mySet.add("jeroboam");
mySet.add(true);
console.log(mySet);
// output: {1, 2, "a", "jeroboam", true}
```

- delete(value)

Removes a specified element from the set.

```js
const mySet = new Set(["John", 44, "Doe", true, false]);
mySet.delete("John");
mySet.delete(true);
mySet.delete(44);
console.log(mySet); // Set(2) { 'Doe', false }
```

- has(value)

Returns true if a specified value exists in a set, false otherwise.

```js
const mySet = new Set(["John", 44, "Doe", true, false]);
console.log(mySet.has("John")); // true
console.log(mySet.has("June")); // false
```

- size

Returns the number of elements in a set.

```js
const mySet = new Set(["John", 44, "Doe", true, false]);
console.log(mySet.size); // 5
```
