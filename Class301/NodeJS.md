## My summary of reading the NodeJS article.
# **What is NodeJS:**

![NodeJS](/images/node.jpg)

1- From the perspective of "Project's homepage": Node.js is a JavaScript runtime built on Chrome’s V8 JavaScript engine.

2-From the perspective of the one and only "Stack overflow": Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library..

3-From my personal perspective after much researching: It's an open source development platform that executes the JavaScript code on the serverside whivh mosty useful for run-time web applications and any other appilications that requires persistant connection to the server.

# **Node Is Built on Google Chrome’s V8 JavaScript Engine:**

Basically what does that mean is when we say the "v8 engine" that it's a JS runtime compiler that runs on chromium based web browsers such as(Brave, Opera, and Vivaldi).
 However this doesn't mean that it's executed on the browser but rather that it has been inhanced by its creator to include various features such as(file system API, an HTTP library, and numourus operating system–related utility methods).

 It's literally a JavaScript run-time .

# **Node Binaries vs Version Manager & how you can install it:**

1- head to the official Node download page and grab the Node binaries for your system. or you use a version manager instead.
2- You can check that Node is installed on your system by opening a terminal and typing node -v

# **Why does Node.js Has Excellent Support for Modern JavaScript?:**

Because it only targets the JS runtime & since it's only fir JS meaning you can run and write the js code using latest and modern syntax then it would totally run it and has no issues doing so. it also means that you don't need to worry about compatibilty issues.

# **Introducing npm, the JavaScript Package Manager:**

NodeJS is bundled with a package manager called ***npm***, it is also known as the worlds largest software regiestry as it contains over 1 million JS code that is ready to download and is actually downloaded by billions.

# **You can download JS in two different ways:**

1- **Globally**: In terminal by running the following command (npm install -g jshint).
2- **Locally**:  In terminal by running the following command (npm init -y).

# **What Is Node.js Used For?:**
NodeJS has built in tools.
 These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them.
 Such tools are:
1- A Beginner’s Guide to Webpack

2- Up and Running with ESLint — the Pluggable JavaScript Linter

3- An Introduction to Gulp.js

4- Unit Test Your JavaScript Using Mocha and Chai

# **Node.js Lets Us Run JavaScript on the Server:**
 It is single-threaded. It’s also event-driven, which means that everything that happens in Node is in reaction to an event. For example, when a new request comes in (one kind of event) the server will start processing it. If it then encounters a blocking I/O operation, instead of waiting for this to complete, it will register a callback before continuing to process the next event. When the I/O operation has finished (another kind of event), the server will execute the callback and continue working on the original request. Under the hood, Node uses the libuv library to implement this asynchronous (that is, non-blocking) behavior.


# **The downsides of using NodeJS:**
1- It slows the performance as it blocks (I/O) calls.

2-Node.js invites a lot of code changes due to Unstable API as CPU-intensive operations should be handed off to a worker thread

3-Node.js Asynchronous Programming Model makes it difficult to maintain code as errors should always be handled correctly for fear of crashing the entire process. Which makes some developers not liking it as much.

# ** The advantages of using NodeJS:**
1- High-performance for Real-time Applications.

2- Easy Scalability for Modern Applications.

3- Cost-effective with Fullstack JS.

4- Community Support to Simplify Development.

5- Easy to Learn and Quick to Adapt.

6- Helps in building Cross-functional Teams.

7- Improves App Response Time and Boosts Performance.

![NodeJS](https://strongloop.com/blog-assets/2014/01/threading_java.png)
# And that was it for this summary.