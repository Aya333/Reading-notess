## My summary of reading the NodeJS article.
# **What is REST:**

![APIS](https://www.wrike.com/blog/content/uploads/2019/05/Application-Programming-Interface-API-Explained-2-1.jpg)

REST (Representational State Transfer) is an architectural style for designing decentralized systems. It originated from an architectural analysis of the Web and combines a client/server architecture with additional constraints that define a uniform interface.

Since an API (Application Programming Interface) is a set of rules that lets programs converse interact (it defines the rules of communications between applications), REST as a style puts some constraints on what an API will look like.


# **REST basis:**
1- client-server

2- stateless

3- cacheable

4- uniform interface

5- layered system
 
6-  code on demand

# **API VS HTTP:**
API: In basic terms, APIs are a set of functions and procedures that allow for the creation of applications that access data and features of other applications, services, or operating systems.

HTTP: It tells the browser what protocol to use. describing the location of something anywhere in the world from anywhere in the world. It's the foundation of the web.

# **What is super agent:**
SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

For request:
request
   .post('/api/pet')
   .send({ name: 'Manny', species: 'cat' })
   .set('X-API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(res => {
      alert('yay got ' + JSON.stringify(res.body));
   });


# **Super agent part2:**

1-**GET** requests The .query() method accepts objects, which when used with the GET method will form a query-string. The following will produce the path /search?query=Manny&range=1..5&order=desc.

2-**HEAD** requests can also use the .query() method for HEAD requests. The following will produce the path /users?email=joe@smith.com.

3-**Response status** The response status flags help determine if the request was a success, among other useful information, making SuperAgent ideal for interacting with RESTful web services.

4-**CORS** For security reasons, browsers will block cross-origin requests unless the server opts-in using CORS headers. Browsers will also make extra OPTIONS requests to check what HTTP headers and methods are allowed by the serve

***NOTE***: 
Promise and Generator support SuperAgent’s request is a “tunable” object that’s compatible with JavaScript promises and the async/await syntax. If you’re using promises, do not call .end() or .pipe(). Any use of .then() or await disables all other ways of using the request

# **Why do i need API key:**
API keys identify an application’s traffic for the API producer, in case the application developer needs to work with the API producer to debug an issue or show their application’s usage. You want to control the number of calls made to your API. You want to identify usage patterns in your API’s traffic.

# And that was it for this summary.