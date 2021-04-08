## My summary of reading the Call stack article.
# What is call stack:

![Stack JS](https://flaviocopes.com/node-event-loop/call-stack-first-example.png)

A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

1- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.

2- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.

3- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.

4- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

# Temporarily store:

When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.

# Manage function invocation (call):

The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.


# What causes a stack overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

# FThe JavaScript Call Stack - What It Is and Why It’s Necessary:

The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

# JavaScript error messages && debugging:

Types of error messages
The first thing that indicates you that something is wrong with your code is the (in)famous error message that the one we saw just moments ago, it usually appears on your console (being developer tools of the browser, terminal or whatever else you are using).

For those already used to programming, reading an error message is like second nature, for everybody else, is something you learn either you like it or not so might as well talk a bit about each of them.

1- Reference errors

2- Type errors

3- Syntax errors

4- Range errors


# Debugging:
1- The most common way its to simply console.log()

2- Using Node.js with Visual Studio Code you can press the debug tab and add a configuration


# Handling errors:
we usually try to catch the errors so we can fallback to a default state of our application in case of an error (this fallback can be a 404 page which is better than a page to just stop working).
An alternative it’s to encapsulate our problematic function code with a try…catch which would make an error be thrown but this time, not “uncaught” so we can send it to a error logging to be checked later and send a fallback to the function so that our code continues without problems.


# And that was it for this summary.