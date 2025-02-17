# LOOPS

Loopes are used to repeat a block of code multiple times.
## Basic loops in Java  Script

- for loop
- while loop
- do while loop

### for loop

Used when number of times the block of code to be excuted is known.

The syntax is as follows:

```javascript
for (initialization; condition; increment) {
    // block of code to be executed
}
```

Example in code

```javascript   
for (let i = 0; i < 10; i++) {
    console.log("Value of i is", i);

}
```

### while loop
Runs as long as long as the speicified condition remains true

The syntax is as follows:

```javascript

while (condition) {
    // block of code to be executed
}
```

Example in code
```javascript

let num = 1;

while (num <= 10) {
    console.log ( "number" , num);
    num++;

}
```

### do while loop
Runs the loop at least once even if the condition is false it starts from the start.

The syntax is as follows:

```javascript

do {
    // block of code to be executed
} while (condition);
```

Example in code

```javascript

let num = 1;

do {
    
    console.log ( "number" , num);
    num++;

} while (num <= 10);

```
### Break and continue statement

The break statement terminates the loop completely and the continue statement skips the current iteration of the loop.

```javascript

for (let i = 0; i < 10; i++) {
    if (i == 5) {
        break;
    }
    console.log(i);

}

```

```javascript

for (let i = 0; i < 10; i++) {
    if (i == 5) {
        continue;
    }
    console.log(i);
}
