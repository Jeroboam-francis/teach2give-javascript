# High Order Array Methods

## forEach

Executes a function on each array element but does not return anything

```js
const arr = [1, 2, 3, 4, 5];
arr.forEach((item, index, array) => {
  console.log(item, index, array);
});
```

## map

Creates an array populated with the results of calling a provided function on every element in the calling array

```js
const arr = [1, 2, 3, 4, 5];
const newArr = arr.map((item, index, array) => {
  return item * 2;
});
console.log(newArr); // [2, 4, 6, 8, 10]
```

## filter

Creates a new array populated with elements that pass a test provided by a function

```js
const arr = [1, 2, 3, 4, 5];
const newArr = arr.filter((item, index, array) => {
  return item % 2 === 0;
});
console.log(newArr); // [2, 4]
```

## reduce

Executes a reducer function on each element of the array, resulting in a single output value

```js
const arr = [1, 2, 3, 4, 5];
const sum = arr.reduce((accumulator, currentValue, currentIndex, array) => {
  return accumulator + currentValue;
}, 0);
console.log(sum); // 15
```

## find

Returns the value of the first element in the provided array that satisfies the provided testing function

```js
const arr = [1, 2, 3, 4, 5];
const found = arr.find((item, index, array) => {
  return item === 3;
});
console.log(found); // 3
```

## findIndex

Returns the index of the first element in the provided array that satisfies the provided testing function

```js
const arr = [1, 2, 3, 4, 5];
const index = arr.findIndex((item, index, array) => {
  return item === 3;
});
console.log(index); // 2
```

## every

Returns true if all elements in the array pass the test implemented by the provided function

```js
const arr = [1, 2, 3, 4, 5];
const allEven = arr.every((item, index, array) => {
  return item % 2 === 0;
});
console.log(allEven); // false
```

## some

Returns true if at least one element in the array passes the test implemented by the provided function

```js
const arr = [1, 2, 3, 4, 5];
const atLeastOneEven = arr.some((item, index, array) => {
  return item % 2 === 0;
});
console.log(atLeastOneEven); // true
```