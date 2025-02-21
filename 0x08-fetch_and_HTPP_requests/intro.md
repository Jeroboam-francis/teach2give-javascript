# INTRODUCTION TO `FETCH` AND `HTTP` REQUESTS

`fetch` is a modern way to make HTTP requests in the browser.

`http` is a protocol that defines how information is transmitted over the internet, including how to make requests, handle responses, and manage errors.

## HTTP REQUESTS

There are different types of HTTP requests:

- GET : a client computer asks for data

- POST : a client computer sends data to be created on the server

- PUT : a client computer sends data to be updated on the server

- DELETE : a client computer sends data to be deleted on the server

### Making a simple fetch request

```js
fetch('https://jsonplaceholder.typicode.com/todos/1')
    .then(response => response.json())
    .then(json => console.log(json));
```