# The Node Core

## Server vs. Client
Node.js is a server technology. A server is a computer that is performing
services. The client asks for those services. The server performs those services
and then gives the response.

DOM Manipulation, XML HTTP Request, and other features that you use
on the browser are not in the ECMA script standards, but they're made
available by the browser. Google chrome is just a C++ app that embeds
the V8 engine. Chrome the browser is the one that's giving more features.

The goal with Node.js is to also use JavaScript on the server side.
This allows you to share libraries of code between server and client side.

## What does JavaSCript need to manage a server?
* JS needs better ways to organize our code into reusable pieces.
* Ways to deal with files
* ways to deal with databases
* The ability to communicate over the Internet
* The ability to accept requests and send repsponses (in the standard format)
* A way to deal with work that takes a long time.

## The JS code
Most of them are wrappers for the C++ code, but there are parts that are
not and simply add more functionality for you.

## Modules
A reusable block of code whose existence does not accidentally impact
other code.

CommonJS Modules: An agreed upon standard for how code modules should be
structured.

The `require` function is made available by Node.

## First-class functions and function expressions
First-class functions: everything you can do with other types, you can
do with functions. In other words, you can use functions like strings,
ints, etc. (ie. pass them around, set variables equal to them, put them
in arrays, and more.)

More specifically, this means that JS supports constructing new functions
during the execution of a program, storing them in data structures,
passing them as arguments to other functions, and returning them as the
values of other functions.


Expression: a block of code that results in a value.
Example of function expression:

```js
var greetMe = function() {
  console.log('Hi Tony');
};
```

The above is different from a named function (ie. `function greetMe {}`).

Personal aside: This is part of the reason I like JS so much. When you
have control over the execution of functions by having first-class
functions, it gives you so much more flexibility with functions.
