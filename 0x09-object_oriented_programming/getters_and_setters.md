# Getters and Setters

Getters and setters are two important concepts in object-oriented programming that allow you to control access to the private variables of a class. They are used to protect the data of a class and ensure that it is not modified directly.

## Getter

Getter is a method that allows you to access the value of a private variable. It is used to retrieve the value of a private variable and return it to the user. It is also known as accessor method.

## Setter

Setter is a method that allows you to modify the value of a private variable. It is used to set the value of a private variable and store it in the object. It is also known as mutator method.

example

```js
class User {
  constructor(name) {
    this._name = name; // Private property convention (_name)
  }

  // Getter (retrieves the value)
  get name() {
    return this._name;
  }

  // Setter (validates and updates the value)
  set name(newName) {
    if (typeof newName !== "string") {
      console.error("Name must be a string!");
      return;
    }
    this._name = newName;
  }
}

const user = new User("Dennis");

// Using the getter
console.log(user.name); // "Dennis"

// Using the setter
user.name = "John"; // Updates successfully
console.log(user.name); // "John"

user.name = 42; // Error: Name must be a string!
```
