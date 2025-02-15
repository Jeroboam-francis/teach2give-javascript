# DATA TYPES
Datatypes are a way of classifying data. There are different types of datatypes.
1. String
2. Number
3. Boolean
4. BigInt
5. Null
6. Undefined

### STRING

It is a data type that is used to represent text or a sequence of characters.

```javascript   
// string

let firtsName = "Jeroboam";
let lastName = "Francis;
```

### NUMBER

It is a data type that is used to represent numbers thats stores integers and decimals.

```javascript
// number

let age = 25;
let height = 5.8;

```

### BOOLEAN

It is a data type that is used to represent true or false values.

```javascript   
// boolean
let isMarried = true;
let isSingle = false;       
```

### BIGINT

It is a data type that is used to represent large integers that cannot be represented by a normal number in javascript.

```javascript  
// bignit 
let numberOfCows = 12838373672829282737292927n;

```

### NULL
Used as an intentional absence of a value unlike `undefined` which represents the absence of a value  ie "NOT ASSIGNED "`null` means `empty on purpose`

```javascript
// null
let cow = null; 
// no cow yet

```
## CHECKING THE TYPES OF VARIABLES USING THE `typoof` OPERATOR

```javascript

// check the type of a variable

let age = 25;
console.log(typeof age); // number

let firstName = "Jeroboam"; 
console.log(typeof firstName); // string

let isMarried = true;
console.log(typeof isMarried); // boolean


```


