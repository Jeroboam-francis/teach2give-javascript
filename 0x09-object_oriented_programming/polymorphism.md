# Polymorphism

In object-oriented programming, polymorphism is a feature that allows objects of different classes to be treated as objects of a common base class.

Polymorphism is a concept in which a parent class reference variable can refer to an object of a child class.

Can be archieved in two ways:

1. Method Overriding
2. Method Overloading

## Method Overriding

Method overriding is a feature in object-oriented programming that allows a subclass to provide a specific implementation of a method that is already defined in its superclass.

When a subclass provides a specific implementation of a method, it is said to override the method in the superclass.

Method overriding is used to achieve polymorphism in object-oriented programming.

## Method Overloading

Method overloading is a feature in object-oriented programming that allows a class to have multiple methods with the same name but different parameters.

When a class has multiple methods with the same name but different parameters, it is said to have method overloading.

Method overloading is used to achieve polymorphism in object-oriented programming.

example

```js
// implementing polymorphism in javascript with overriding

class Math {
  add(number1, number2) {
    return number1 + number2;
  }
}

class Arithmetics extends Math {
  add(number1, number2) {
    if (number1 < 0) {
      console.log("Can only add positive numbers");
    } else if (number2 < 0) {
      console.log("Can only add positive numbers");
    } else {
      console.log(number1 + number2);
    }
  }
}

const arithmetic = new Arithmetics();
arithmetic.add(-5, 5);
arithmetic.add(5, -5);
arithmetic.add(5, 5);

```

