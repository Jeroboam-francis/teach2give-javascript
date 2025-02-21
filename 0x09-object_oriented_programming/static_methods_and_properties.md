# Static Methods and Properties

Static methods and properties are methods and properties that are associated with a class rather than an instance of a class. They are defined using the `static` keyword in the class definition.

## static methods

Method defined with the `static` keyword are called static methods. They can be called on the class itself, rather than on an instance of the class. Static methods are often used for utility functions that do not depend on the state of an instance.

example

```js
class MathUtils {
  static add(a, b) {
    return a + b;
  }

  static subtract(a, b) {
    return a - b;
  }
}

// Calling static methods directly from the class
console.log(MathUtils.add(10, 5)); // 15
console.log(MathUtils.subtract(10, 5)); // 5

// Trying to call a static method on an instance
const math = new MathUtils();
// console.log(math.add(10, 5)); Error: math.add is not a function
```

## static properties

A variable  that belongs to the class itself, rather than to any instance of the class. Static properties are often used to store constants or configuration settings that are shared across all instances of the class.

example.

```js
class Counter {
  static count = 0; // Static property

  static increment() {
    Counter.count++; // Accessing the static property
  }

  static getCount() {
    return Counter.count;
  }
}

// Accessing static property without an instance
console.log(Counter.getCount()); // 0

Counter.increment();
Counter.increment();

console.log(Counter.getCount()); // 2

```
