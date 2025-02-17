# SCOPE

Scope is the context in which a variable is defined.

## Types of scoopes in Javascript

1. Global Scope
2. Local Scope( functional scope)
3. Block Scope (introduced in ES6)
4. lexical scope

### 1. Global Scope
A variable defined outside of a function is known as a global variable and can be accessed anywhere in the program.

Example
```javascript
let marks = 90;

function printMarks(){
    console.log(marks);// accessible inside function
   
}
printMarks();// accessible outside function
console.log(marks);// accessible outside function
```

### 2. Local Scope

A variable defined inside a function is known as a local variable and can only be accessed within that function.

Example
```javascript
function printMarks(){
    let marks = 90;
    console.log(marks);// accessible inside function
}
printMarks();// printmark is not defined

```

### 3. Block Scope

A variable defined inside a block is known as a block variable and can only be accessed within that block if we use let, if we use var its accessible outside the block

Example
```javascript
if(true){
    let age = 25;
    console.log(age);// accessible inside block
}
console.log(age);// age is not defined
```

### 4. Lexical Scope

A variable defined in the scope of another variable is known as lexical variable and can only be accessed within that scope.

Example
```javascript

function printMarks(){
    let marks = 90;
    function printAge(){
        console.log(marks);// accessible inside function
    }
    printAge();
    }

printMarks();

``` 

