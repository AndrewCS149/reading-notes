# Node || Express || APIs

---

### Google Chrome's V8 Engine

Chrome's V8 engine is an open source engine that runs JavaScript within the browser.Node.js takes these features and enables a user to create and run JavaScript code on our local machines.

### Run node in the command line

Steps:

1. Create a new app.js file in a directory.
2. Create a `console.log("Hello World!")` in that app.js.
3. Navigate to that file within the command  line.
4. Run `node app.js` in the command line and there ya go!

--- 

### Installing packages locally vs globally

Globally: 

`$ npm install -g [package-name]`

Locally:

`$ npm install -y [package-name]`

Installing a package locally means it will exist within whatever project you download it to.

---

### Running JavaScript on a server with Node.js

```js
const http = require('http');

http.createServer((request, response) => {
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);

console.log('Server running on http://localhost:3000');
// code block retrieved from - https://www.sitepoint.com/an-introduction-to-node-js/
```

---

### Advantages of Node.js

* It can read JSON
* You do not need to switch languages to do everything you need
* Transitioning to Node development is very seamless

