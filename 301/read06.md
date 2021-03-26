# NODE.JS
### **_NODE.JS_** is an event-based, JavaScript runtime that was built on Chrome’s V8 JavaScript engine. it has excellent support for modern JavaScript which means the programmer can write JavaScript using the latest and most modern syntax. it is suited to building applications that require some form of real-time interaction or collaboration Apps
### **_Version Manager_** is program that allows you to install multiple versions of Node and switch between them at will it is useful to negates potential permission issues when using Node with npm and lets the user to set a Node version on a per-project basis
### Node comes bundled with a package manager called **_npm_** , it is the largest software registry. it can be installed globally by typing on the terminal `npm install -g jshint` and locally by `npm init -y` . `node_modules` is where npm has saved lodash and any libraries that lodash depends on. for `package.json` file the lodash listed under the `dependencies` field.
### Node.js is used for bundling the JavaScript files and dependencies into static assets, running tests or automatic code linting and style checking. it is  back end to run (React and Angular) frameworks which are used for developing apps with any modern JavaScript. Node.js also run JavaScript on the server. it provides some unique benefits, compared to traditional languages
### For Execution Model Node.js designed to be as a single-threaded. It’s also event-driven, which means that everything that happens in Node is in reaction to an event so when a new request comes in the server will start processing it. which causes the server very little overhead.

![ex](https://i.ibb.co/KXhmM63/2.jpg)

### However, the errors should always be handled correctly for fear of crashing the entire process.
### To create a server then:
  - it will starting by requiring Node’s native HTTP module. then use its `createServer` method to create a new web server object, to which pass an anonymous function. This function will be invoked for every new connection that’s made to the server.
  - The anonymous function is called with two arguments `request` and `response` . These contain the request from the user and the response which we use to send back a 200 HTTP status code
### One of the big advantages for the Node.js is speaking to JSON which is probably the most important data exchange format on the Web. In addition to it can be used as a scripting language to automate repetitive or error prone tasks to PC. It can also be used to write a command line tool.
### Finally Node.js can be interduced as an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library


