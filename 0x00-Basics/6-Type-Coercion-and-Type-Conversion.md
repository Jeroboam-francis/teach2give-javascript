# TYPES OF COERCION AND TYPE CONVERSION

Involves changing values of datatypes to another datatype.

## TYPES  COERCION - Implicit coercion

Happens automatically when javascript tries to perfromm operations between different data types and is commonly in comparison ( == ), string concatenation ( + ) and arithmetic operations  and may sometimes lead to unexcpected error.

examples

```javascript
console.log( 10 + "10" ): // returns 1010
console.log( "10" + 10 ): // returns 1010       

```

## TYPE CONVERSION - Explicit coercion

Happens when we explicitly convert one datatype into another.

methods of type conversion

### 1. Convert to string  using toString() or string ()

example

```javascript

console.log( 10.toString() ): 
console.log(String( 10 )): 

```

### 2. Convert to number using Number() , parseInt() or parseFloat()

example

```javascript
console.log (Number("10")); 
console.log (parseInt ("10") )
```

### 3. Boolean ()

- faisy values: 0, "", null, undefined, NaN, false.
- Truthy values: everything else

```javascript
console.log( boolean(0))// false
console.log ( "hello world")
```
