# JS Questions

#### Explain event delegation.

Event delegation allows developers to avoid adding event listeners to specific
nodes. Instead, event listeners are attached to a parent, which analyzes bubbled
events to find a match on child elements. This allows developers to avoid
manually placing event listeners on groups of similar elements with similar
functionality, abstracting functionality and "delegating" it to a parent.

#### Explain how `this` works in JavaScript.

`this` refers to the current execution context of a function. If it's called
outside of a function, it refers to the global object (window) in a browser.
`this` causes a lot of headache for new JavaScript developers because of the
fact that it refers to the execution context of a function and not the
invoking function, and returns as `undefined` when used in strict mode.

#### Explain how prototypal inheritance works.

Prototypal languages only have objects, not classes. A developer creates a new
object either from nothing or by cloning existing objects, which are extended
with new properties -- there's a kind of chain that goes all the way up to a
global object, which inherits from `null`.

#### What do you think of AMD vs CommonJS?

At this point, I try to avoid both. I prefer CommonJS for ease of use with
simple client-side rendered applications, but I prefer to use ES2015 modules on
both the client and the server. AMD is better on certain points than CommonJS because of its
asynchronous nature, but ES2015 modules are easier and better than either, in my
opinion.

#### Explain why the following doesn't work as an IIFE: `function foo(){ }();`.


#### What needs to be changed to properly make it an IIFE?

#### What's the difference between a variable that is: `null`, `undefined` or `undeclared`?

#### What is a closure, and how/why would you use one?

#### What's a typical use case for anonymous functions?

#### How do you organize your code? (module pattern, classical inheritance?)

#### What's the difference between host objects and native objects?

#### Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?

#### What's the difference between `.call` and `.apply`?

#### Explain `Function.prototype.bind`.

#### When would you use `document.write()`?

#### What's the difference between feature detection, feature inference, and using the UA string?

#### Explain AJAX in as much detail as possible.

#### Explain how JSONP works (and how it's not really AJAX).

#### Have you ever used JavaScript templating?

Yes.

###### If so, what libraries have you used?

Handlebars, Mustache, EJS, Pug, etc.

#### Explain "hoisting".


#### Describe event bubbling.


#### What's the difference between an "attribute" and a "property"?


#### Why is extending built-in JavaScript objects not a good idea?

#### What is the difference between `==` and `===`?

#### Explain the same-origin policy with regards to JavaScript.

#### Make this work:

#### Why is it called a Ternary expression, what does the word "Ternary" indicate?

#### What is `"use strict";`? what are the advantages and disadvantages to using it?

#### Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?

#### Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?

#### Explain what a single page app is and how to make one SEO-friendly.

#### What is the extent of your experience with Promises and/or their polyfills?

#### What are the pros and cons of using Promises instead of callbacks?

#### What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?

#### What tools and techniques do you use debugging JavaScript code?


#### What language constructions do you use for iterating over object properties and array items?


#### Explain the difference between mutable and immutable objects.

###### What is an example of an immutable object in JavaScript?
###### What are the pros and cons of immutability?
###### How can you achieve immutability in your own code?


#### Explain the difference between synchronous and asynchronous functions.


#### What is event loop?
###### What is the difference between call stack and task queue?


