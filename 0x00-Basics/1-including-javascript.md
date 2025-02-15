## Including JavaScript

There are two ways of including JavaScript in HTML:

### A. Internally

   Using `<script>` tag

Using this method requires the script to be placed at the end of the other items in the HTML body, i.e., right above the closing `</body>` tag, as shown below:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Including JavaScript in HTML</title>
</head>
<body>
    <h1>Including JavaScript in HTML</h1>
    <script>
        console.log ("Hello World");
    </script>

</body>
</html>
```

### B. Externally

A separate `.js` file is created and linked using `<script>` tag to the HTML file.

```html 
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>inlcuding javascript in html </title>
    <script src="script.js"></script>
  </head>
  <body>
    <h1>JavaScript</h1>
  </body>
</html>
```

``` javascript

console.log("Hello, world!");
console.log("This is an example of a script running in the browser.");  

```

As shown above, the `console.log` function is used to print the message to the console and the `script.js` for optimal performance must come at the end of the other items in the HTML body, i.e., right above the closing `</body>` tag.
 Or use `<script defer src="script.js"></script>` which contains keyword defer which tells the browser to wait for the script to be downloaded before executing it.

 ```html
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Including JavaScript in HTML</title>
</head>
<body>
    <h1>Including JavaScript in HTML</h1>
    <script
        src="app.js" defer>
    </script>

</body>
</html>
```
