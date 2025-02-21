# Inheritance

Inheritance is the process of creating a new class from an existing class. The new class is called a subclass or derived class, and the existing class is called a superclass or base class.

Inheritance allows a subclass to inherit the properties and methods of its superclass, and also to add its own properties and methods. This allows for code reuse and the creation of more specialized classes.

example:

```js
class Animal {
  constructor(numLegs, numEyes) {
    this.numLegs = numLegs;
    this.numEyes = numEyes;
  }

  move() {
    console.log(`Animal looking at the road with ${this.numEyes} eyes`);
    console.log(`Animal moving with ${this.numLegs} legs`);
  }

  eat() {
    console.log(`Animal eating for survival`);
  }
}

class Cow extends Animal {
  constructor(numLegs, numEyes, breed, gender) {
    super(numLegs, numEyes); // calls the parent constructor
    this.breed = breed;
    this.gender = gender;
  }

  sound() {
    console.log(`The ${this.gender} ${this.breed} cow is mooing`);
  }
}

const myCow = new Cow(4, 2, "Guernsey", "Male");
myCow.move();
myCow.eat();
myCow.sound();#
```

In this example, the Cow class extends the Animal class, inheriting its properties and methods. The Cow class also has its own properties and methods, such as breed and gender, and the sound method.
