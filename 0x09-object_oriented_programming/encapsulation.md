# Encapsulation

Encapsulation is a mechanism that wraps data and methods together into a single unit called an object. It is a fundamental concept in object-oriented programming (OOP) that helps to protect the data and ensure that it is accessed and modified only through the defined methods.

example

``` js
class BankAccount {
  #balance = 0;

  constructor(owner) {
    this.owner = owner;
  }

  deposit(amount) {
    this.#balance += amount;
    console.log(`Deposited ${amount}. New balance: ${this.#balance}`);
  }

  checkBalance() {
    console.log(`Current balance is: ${this.#balance}`);
  }
}

const account = new BankAccount("John");
account.deposit(500);
account.checkBalance();
// console.log(account.#balance); // Error: Private field '#balance' must be declared in an enclosing class
```

In the example above, the `#balance` field is declared as private using the `#` symbol. This means that it can only be accessed and modified within the `BankAccount` class. The `deposit` and `checkBalance` methods are public and can be used to interact with the `#balance` field.

By encapsulating the `#balance` field within the `BankAccount` class, we can ensure that it is protected from being accessed or modified directly from outside the class. This helps to maintain the integrity of the data and prevent any unintended modifications.
