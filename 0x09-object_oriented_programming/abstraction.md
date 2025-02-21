# Abstraction

Abstraction is a process of hiding the complex details and showing only the necessary features of an object. It helps in reducing the complexity of the system and makes it easier to understand and use.

example

```js
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

  withdraw(amount) {
    if (amount > this.#balance) {
      console.log(`Please enter an amount that matches your balance`);
    } else {
      this.#balance -= amount;
      console.log(
        `Successful withdrawal of ${amount}. New balance: ${this.#balance}`,
      );
    }
  }
}

const account = new BankAccount("John");
account.deposit(500);
account.withdraw(900); // Please enter an amount that matches your balance
account.withdraw(200); // Successful withdrawal of 200. New balance: 300
```

In this example, `withdraw()` method is abstracted away from the user, and the user only needs to know that they can call `withdraw()` with an amount to withdraw money from their account. The user does not need to know how the withdrawal is actually implemented, which makes the system easier to understand and use.
