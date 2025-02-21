# OPERATORS

Operators are symbols that are used to perform operations on variables and values.
In JavaScript, there are several types of operators, including arithmetic operators, comparison operators, logical operators, assignment operators, and more.

## 1. ARITHMETIC OPERATORS

Used to perform mathemetic operations such as addition, subtraction, multiplication, and division.

 A. Addition (+)

Adds two or more numbers

```javascript
// Adding two numbers
let x = 10;
let z = 20;
console.log( a+b ):
// output 30

// Addition can e used to add two strings as well

// Adding two strings
let firtsName= "Jeroboam";
let secondName= "Francis";
console.log( firtsName+secondName ):
//Output JeroboamFrancis 
```

B. Subtraction(-)

This subtracts operands and returns the difference between them ie right operand from the left operand

```javascript

//Subracting 

let x = 10;
let y = 5;
console.log( x-y ):
//Output 5

```

C. Multiplication(*)

This multiplies operands and returns the product of them

```javascript

//Multiplying 

let x = 10 ; 
let y = 5;
console.log( x*y ):
//Output 50

```

D. Division(/)

This divides operands and returns the quotient of them

```javascript

//Dividing

let x = 10;
let y = 5;
console.log( x/y ):
//Output 2

```

E. Modulus(%)

This divides operands and returns the remainder of them

```javascript

//Modulus

let x = 10;
let y = 5;
console.log( x%y ):
//Output 0

```

F. Exponentiation(**)

This raises the left operand to the power of the right operand and returns the result

```javascript

//Exponentiation

let x = 10;
let y = 5;
console.log( x**y ):
//Output 100000

```

### 2.  INCREMENT AND DECREMENT OPERATORS

#### Increment operator(++)

This increments the value of a variable by 1

```javascript

//Increment operator 

let x = 10;
console.log( x++ ): // returns 10 then  increments the value of x by 1
console.log ( x ): // returns 11

let y = 5;
console.log( ++Y ): // returns  6 then increments the value of y by 1

```

##### Decrement operator(--)

This decrements the value of a variable by 1

```javascript

//Decrement operator
//Post-decrement

let x = 10; console.log( x-- ): // returns 10 then decrements the value of x by 1
console.log ( x ): // returns 9

// Pre-decrement

let y = 5; console.log( --Y ): // returns  4 then decrements the value of y by 1

```

### 3.  ASSIGNMENT OPERATORS (=' +=, -=, *=, /=, %=, **=')

This is used to assign a value to a variable

#### A. Simple assignment operator(=)

Used to assign a value to a variable

```javascript

//Assignment operator   

let x = 10;
console.log( x ): // returns 10

```

##### B. Additiional assignment operator(+=)

Used to add a value to a variable

```javascript

//Additional assignment operator

let x = 10;
x += 5;
console.log( x ): // returns 15

```

###### C. Subtraction assignment operator(-=)

Used to subtract a value from a variable

```javascript

//Subtraction assignment operator

let x = 10;
x -= 5;
console.log( x ): // returns 5

```

###### D. Multiplication assignment operator(*=)

Used to multiply a value to a variable

```javascript

//Multiplication assignment operator

let x = 10;
x *= 5;
console.log( x ): // returns 50

```

###### E. Division assignment operator(/=)

Used to divide a value to a variable

```javascript

//Division assignment operator

let x = 10;
x /= 5;
console.log( x ): // returns 2

```

### 4. COMPARISON OPERATORS

Used to compare values and return true or false

#### A. Equality operator(==) and strict equality operator(===)

Equality operator(==)

Returns true if the operands are equal to each other and false otherwise and also ignores datatypes  and does only comparison

```javascript

//Equality operator

let x = 10;
let y = 10;
console.log( x==y ): // returns true
console.log( x==5 ): // returns false

```

Strict Equality operator(===)

Returns true if the operands are equal to each other and false otherwise and also checks the datatypes

```javascript

//Strict equality operator

let x = 10;
let y = "10";
console.log( x===y ): // returns false
console.log( x===10 ): // returns true

```

##### B. Inequality operator(!=) and Strict inequality operator(!==)

Inequality operator(!=)

Returns true if the operand left is not equal to the operand right and false otherwise and also ignores datatypes

```javascript

// Inequality operator

let x = 10;
let y = 5;
console.log( x!=y ): // returns true
console.log( x!=10 ): // returns false

console.log( 10 != "10" ): // returns false
console.log( 10 != 10 ): // returns false

```

Strict Inequality operator(!==)

Returns true if the operand left is not equal to the operand right and false otherwise
and checks datatypes and compares them

```javascript

// Strict Inequality operator

let x = 10;
let y = 5;
console.log( x ! ==y ): // returns true
console.log( x!==10 ): // returns false

console.log( 10 !== "10" ): // returns true

```

###### C. Greater than operator(>) and less than operator(<)

i. Greater than operator(>)

Returns true if the operand left is greater than the operand right and false otherwise

```javascript

// Greater than operator

let x = 10;
let y = 5;
console.log( x>y ): // returns true
console.log( y>x): // returns false

```

ii. Less than operator(>)

Return true if the operands on left is less than the operand on the right and false otherwise

```javascript

//Less than operator

let x = 10;
let y = 5;
console.log( x<y ): // returns false
console.log( y<x): // returns true

```

iii. Greater than or equal to operator(>=)

Returns true if the operand left is greater than or equal to the operand right and false otherwise

```javascript

//Greater than or equal to operator 

let x = 10;
let y = 5;
console.log( x>=y ): // returns true
console.log( y>=x): // returns false
console.log( x>=x): // returns true

```

iv. Less than or equal to operator(<=)

Returns true if the operand left is less than or equal to the operand right and false otherwise

```javascript

//Less than or equal to operator    

let x = 10; 
let y = 5;  
console.log( x<=y ): // returns false   
console.log( y<=x): // returns true   
console.log( x<=x): // returns true 

```

### 5. LOGICAL OPERATORS

Used for boolean logic.

i. logical AND Operator (&&)

Returns true if both operands are true and false otherwise returns false

```javascript

//Logical AND operator
console.log( true && true ): // returns true
console.log( true && false ): // returns false

```

Truth table for the AND operator

| a | b | a && b |
|---|---|---|
| true | true | true |
| true | false | false |
| false | true | false |
| false | false | false |

ii. logical OR Operator (||)

Returns true if either operand is true and false otherwise returns false

```javascript

//Logical OR operator
console.log( true || true ): // returns true
console.log( true || false ): // returns true
console.log( false || true ): // returns true
console.log( false || false ): // returns false

```

Truth table for the OR operator

| a | b | a OR b |
|---|---|---|
| true | true | true |
| true | false | true |
| false | true | true |
| false | false | false |

iii. logical NOT Operator (!)

Used to negate boolean values i.e. true becomes false and false becomes true

```javascript

//Logical NOT operator
console.log( !true ): // returns false
console.log( !false ): // returns true
```
