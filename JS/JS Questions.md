## JS Questions
1. [Explain event delegation](#explain-event-delegation)
2. [Explain how `this` works in JavaScript](#explain-how-this-works-in-javascript)
3. [Explain how prototypal inheritance works](#explain-how-prototypal-inheritance-works)
4. [What do you think of AMD vs CommonJS?](#what-do-you-think-of-amd-vs-commonjs)
5. [Explain why the following doesn't work as an IIFE: `function foo(){ }();`. What needs to be changed to properly make it an IIFE?](#explain-why-the-following-doesnt-work-as-an-iife-function-foo--what-needs-to-be-changed-to-properly-make-it-an-iife)
6. [What's the difference between a variable that is: `null`, `undefined` or undeclared? How would you go about checking for any of these states?](#whats-the-difference-between-a-variable-that-is-null-undefined-or-undeclared-how-would-you-go-about-checking-for-any-of-these-states)
7. [What is a closure, and how/why would you use one?](#what-is-a-closure-and-howwhy-would-you-use-one)
8. [Can you describe the main difference between a `.forEach` loop and a `.map()` loop and why you would pick one versus the other?](#can-you-describe-the-main-difference-between-a-foreach-loop-and-a-map-loop-and-why-you-would-pick-one-versus-the-other)
9. [What's a typical use case for anonymous functions?](#whats-a-typical-use-case-for-anonymous-functions)
11. [What's the difference between host objects and native ob.jects?](#whats-the-difference-between-host-objects-and-native-objects)
12. [Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Pe.rson()`?](#difference-between-function-person-var-person--person-and-var-person--new-person)
13. [What's the difference between `.call` and `.apply`?](#whats-the-difference-between-call-and-apply)
14. [Explain `Function.prototype.bind`.](#explain-functionprototypebind)
17. [Explain Ajax in as much detail as possible.](#explain-ajax-in-as-much-detail-as-possible)
18. [What are the advantages and disadvantages of using Ajax?](#what-are-the-advantages-and-disadvantages-of-using-ajax)
19. [Explain how JSONP works (and how it's not really Ajax).](#explain-how-jsonp-works-and-how-its-not-really-ajax)
20. [Have you ever used JavaScript templating? If so, what libraries have you used?](#have-you-ever-used-javascript-templating-if-so-what-libraries-have-you-used)
21. [Explain "hoisting".](#explain-hoisting)
22. [Describe event bubbling abd capture.](#describe-event-bubbling-and-capture)
24. [Why is extending built-in JavaScript objects not a good idea?](#why-is-extending-built-in-javascript-objects-not-a-good-idea)
25. [Difference between document `load` event and document `DOMContentLoaded` event?](#difference-between-document-load-event-and-document-domcontentloaded-event)
26. [What is the difference between `==` and `===`?](#what-is-the-difference-between--and-)
27. [Explain the same-origin policy with regards to JavaScript.](#explain-the-same-origin-policy-with-regards-to-javascript)
28. [Make this work: `duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]`](#make-this-work)
29. [Why is it called a Ternary expression(三元表达式), what does the word "Ternary" indicate?](#why-is-it-called-a-ternary-expression-what-does-the-word-ternary-indicate)
30. [What is "use strict";? what are the advantages and disadvantages to using it?](#what-is-use-strict-what-are-the-advantages-and-disadvantages-to-using-it)
31. [Create a for loop that iterates up to 100 while outputting "fizz" at multiples of 3, "buzz" at multiples of 5 and "fizzbuzz" at multiples of 3 and 5](#create-a-for-loop-that-iterates-up-to-100-while-outputting-fizz-at-multiples-of-3-buzz-at-multiples-of-5-and-fizzbuzz-at-multiples-of-3-and-5)
32. [Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?](#why-is-it-in-general-a-good-idea-to-leave-the-global-scope-of-a-website-as-is-and-never-touch-it)
33. [Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?](#why-would-you-use-something-like-the-load-event-does-this-event-have-disadvantages-do-you-know-any-alternatives-and-why-would-you-use-those)
34. [Explain what a single page app is and how to make one SEO-friendly.](#explain-what-a-single-page-app-is-and-how-to-make-one-seo-friendly)
35. [What is the extent of your experience with Promises and/or their polyfills?](#what-is-the-extent-of-your-experience-with-promises-andor-their-polyfills)
36. [What are the pros and cons of using Promises instead of callbacks?](#what-are-the-pros-and-cons-of-using-promises-instead-of-callbacks)
37. [What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?](#what-are-some-of-the-advantagesdisadvantages-of-writing-javascript-code-in-a-language-that-compiles-to-javascript)
38. [What tools and techniques do you use debugging JavaScript code?](#what-tools-and-techniques-do-you-use-for-debugging-javascript-code)
39. [What language constructions do you use for iterating over object properties and array items?](#what-language-constructions-do-you-use-for-iterating-over-object-properties-and-array-items)
40. [Explain the difference between mutable and immutable objects.](#explain-the-difference-between-mutable-and-immutable-objects)
41. [Explain the difference between synchronous and asynchronous functions.](#explain-the-difference-between-synchronous-and-asynchronous-functions)
42. [What is event loop? What is the difference between call stack and task queue?](#what-is-event-loop-what-is-the-difference-between-call-stack-and-task-queue)
43. [Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`](#explain-the-differences-on-the-usage-of-foo-between-function-foo--and-var-foo--function-)
44. [What are the differences between variables created using `let`, `var` or `const`?](#what-are-the-differences-between-variables-created-using-let-var-or-const)
45. [What are the differences between ES6 class and ES5 function constructors?](#what-are-the-differences-between-es6-class-and-es5-function-constructors)
46. [Can you offer a use case for the new arrow => function syntax? How does this new syntax differ from other functions?](#can-you-offer-a-use-case-for-the-new-arrow--function-syntax-how-does-this-new-syntax-differ-from-other-functions)
47. [What advantage is there for using the arrow syntax for a method in a constructor?](#what-advantage-is-there-for-using-the-arrow-syntax-for-a-method-in-a-constructor)
48. [What is the definition of a higher-order function?](#what-is-the-definition-of-a-higher-order-function)
49. [Can you give an example for destructuring an object or an array?](#can-you-give-an-example-for-destructuring-an-object-or-an-array)
50. [ES6 Template Literals offer a lot of flexibility in generating strings, can you give an example?](#es6-template-literals-offer-a-lot-of-flexibility-in-generating-strings-can-you-give-an-example)
51. [Can you give an example of a curry function and why this syntax offers an advantage?](#can-you-give-an-example-of-a-curry-function-and-why-this-syntax-offers-an-advantage)
52. [What are the benefits of using spread syntax and how is it different from rest syntax?](#what-are-the-benefits-of-using-spread-syntax-and-how-is-it-different-from-rest-syntax)
53. [How can you share code between files?](#how-can-you-share-code-between-files)
54. [Why you might want to create static class members?](#why-you-might-want-to-create-static-class-members)


### Explain event delegation
Event delegation is a techinique involving adding event listeners to a parement element instead of addding them to themself. The listener will fire whenever the event is triggereddue to event bubbling up the DOM. 
Advantages: 
 - Low memory usage becuae only one single handler is needed on the parent element, rather than having no attach even handlers on each element.
 - There is no need to unbind the handler from elements that are removed and to bind the event for new elements.
 
### Explain how this works in JavaScript
The value of this depends on how the function is called. 
1. if the new keyword is used when calling the function, this inside the function is a brand new object.
2. if apply, call or bind are used to call/create a function, this inside the function is the object that is passed in as the argument
3. if a function is called as a method, such as obj.method() - this is the object that the function is a propery of (当函数作为对象里的方法被调用时，函数内的this是调用该函数的对象。比如当obj.method()被调用时，函数内的 this 将绑定到obj对象。)
4. if a function is called as a free function, meaning it was called without any of conditions present above, this is the global object. In browser, it is the window object. if in strict mode, this will be undefined instead of the global object
5. if multiple of the above rules apply, the rule that is higher wins and will set the this value (from 1 to 4)
6. if the function is an arrow function, it ignores all the rules above and receives the this value of its surrounding scope at the time it is created

### Explain how prototypal inheritance works
All JavaScript objects have a prototype property, that is a reference to another object. When a property is accessed on an object and if the property is not found on that object, the JavaScript engine looks at the object's prototype, and the prototype's prototype and so on, until it finds the property defined on one of the prototypes or until it reaches the end of the prototype chain.

### What do you think of AMD vs CommonJS?
Both are ways to implement a module system, which was not natively present in JavaScript until ES6 came along. CommonJS is synchronous while AMD (Asynchronous Module Definition) is asynchronous. CommonJS is desgined with server-side develpoment, AMD is support for asynchronous loading of modules, is more inteded for browsers.

I find AMD syntax is too verbose and CommonJS is closer to the style you would write import statements in other languages. Most of time, I find AMD unnecesary, because if you severed all your JavaScript into one bundle file, you would not benefit from the async loading properties. Also, CommonJS syntax is closer to Node style of writing modules.

I am happy that with ES6 modules, that has support for both synchronous and asynchronous loading, we can just stick to one approach.  We can use tools like Babel to convert the code if browser is not support ES6.

### Explain why the following doesn't work as an IIFE: function foo(){ }();. What needs to be changed to properly make it an IIFE?
IIFE stands for Immediately Invoked Function Expressions. The function foo(){ }(); will be parsed to function foo(){ } and (). where the former is a function declaration and the latter (a pair of brackets) is an attempt at calling a function but there is no name specified, hence it throws Uncaught SyntaxError: Unexpected token )

to make it work: 
- (function foo(){ })()
- (function foo(){ }())

### What's the difference between a variable that is: null, undefined or undeclared? How would you go about checking for any of these states?
- A variable that is undefined is a variable that has been declared, but not assigned a value. use strict equality `(====) or typeof foo === 'undefined'` to check undefined
- Undeclared variables are created when you assign a value to a variable that is not created using var, let or const before.
- Null variable will have been assigned to the null value. use `foo === null` to check null variable

### What is a closure, and how/why would you use one?
.Closures are functions that have access to the outer (enclosing) function's variables—scope chain even after the outer function has returned.

Benefit: 
- Data privacy / emulating private methods with closures
- Partail applications or currying

### Can you describe the main difference between a .forEach loop and a .map() loop and why you would pick one versus the other?
forEach:
- Iterates through the element in an array
- Executes a callback for each element
- Does not return a value

map: 
- Iterates through the elements in an array.
- "Maps" each element to a new element by calling the function on each element, creating a new array as a result.

forin: 
- Iterates the property as well.
- can used to iterates the keys of object

The main difference between .forEach and .map is that .map returns a new array. If you need the result, but do not wish to mutate the original array use map. if you simply need to iterate over an array, use forEach

### What's a typical use case for anonymous functions?
They can be used in IIFEs so that variables declared in it do not leak to the global scope

As a callback that is used once and does not need to be used anywhere else. The code will seem more self-contained and readable when handlers are defined right inside the code calling them, rather than having to search elsewhere to find the function body.
```
setTimeout(function() {
  console.log('Hello world!');
}, 1000);
```

### What’s the difference between host objects and native ob.jects?
Native objects are objects that are part of the JavaScript language defined by the ECMAScript specification, such as String, Math, RegExp, Object, Function, etc.

Host objects are provided by the runtime enviornment(browser or Node), such as window, XMLHTTPRequest.

### Difference between: function Person(){}, var person = Person(), and var person = new Person()?

var person = Person() invokes the Person as a function, and not as a constructor. Invoking as such is a common mistake if the function is intended to be used as a constructor.

var person = new Person() creates an instance of the Person object using the new keyword, which inherits from Person.prototype. Or you can use Object.create(Person.prototype)
```
function Person(name) {
	this.name = name;
}

var person = Person('John');
console.log(person) // undefined

var person = new Person('John')
console.log(person) // Person { name: "John"}
```

### What's the difference between .call and .apply?
Both .call and .apply are used to invoke functions and the first parameter will be used as the value of this within the function. However, .call takes in comma-separated arguments, and .apply takes in an array of arguments as the next argument.
```
function add(a, b) {
	return a + b;
}

console.log(add.call(null, 1, 2)) // 3
console.log(add.apply(null, [1,2])) // 3
```

### Explain Function.prototype.bind
The bind() method creates a new function that, when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.

It is most useful for binding the value of this in methods class that you want to pass into other function.

### Explain Ajax in as much detail as possible.
Advantages: 
- Reduce connections to the server since scripts and stylesheets only have to be requested once.
- State can be maintained on a page. JavaScript variables and DOM state will persist because the main container page was not reloaded.

Disadvantages:
- Dynamic webpages are harder to bookmark
- Does not work if JavaScript has been disabled in the browser.
- Basically most of the disadvantages of a SPA

### Explain how JSONP works (and how it's not really Ajax).
JSONP (JSON with Padding) is a method commonly used to bypass the cross-domain policies in web browsers because Ajax requests from the current page to a cross-origin domain is not allowed

JSONP works by making a request to cross-origin domain via a `<script>` tag and usually with a callback query parameter, for example: https://example.com?callback=printData. The server will then wrap the data within a function called prinData and return it to the client
```
<!-- https://mydomain.com -->
<script>
function printData(data) {
  console.log(`My name is ${data.name}!`);
}
</script>

<script src="https://example.com?callback=printData"></script>
```
The client has to have the printData function in its global scope and the function will be executed by the client when the response from the cross-origin domain is received.

JSONP can be unsafe and has some security implications. As JSONP is really JavaScript, it can do everything else JavaScript can do, so you need to trust the provider of the JSONP data.

CORS is the recommended approach instead of JSONP

### Have you ever used JavaScript templating? If so, what libraries have you used?
Yes. Lodash, JSX and Vue. JSX  is my new favorite as it's close to JavaScript and there is barely any syntax to learn. Nowadays, you can even use ES6 template string literals as a quick way for creating templates without relying on third-part code.
```
const template = `<div>My name is ${name}</div>`
```

### Explain "hoisting"
Variables declared or initialized with the var keyword will have their declaration "move" up to the top of the current scope is Hoisting.

Only the declaration is hoisted, the assignment, will stay where it is.
```
// var declarations are hoisted.
console.log(foo); // undefined
var foo = 1;
console.log(foo); // 1

// let/const declarations are NOT hoisted.
console.log(bar); // ReferenceError: bar is not defined
let bar = 2;
console.log(bar); // 2
```
Function declarations have the body hoisted while the function expressions (written in the form of variable declarations) only has the variable declaration hoisted
```
// Function Declaration
console.log(foo); // [Function: foo]
foo(); // 'FOOOOO'
function foo() {
  console.log('FOOOOO');
}
console.log(foo); // [Function: foo]

// Function Expression
console.log(bar); // undefined
bar(); // Uncaught TypeError: bar is not a function
var bar = function() {
  console.log('BARRRR');
};
console.log(bar); // [Function: bar]
```

### Describe event bubbling.
When an event triggers on a DOM element, then the event is bubbled up to its parent and the same thing happen. This bubbling occurs up the element's root all the way to the document. 

### Why is extending built-in JavaScript objects not a good idea?
Extending a built-in JavaScript object means adding properties/functions to its prototype. While this may seem like a good idea at first, it is dangerous in practice. Imagine your code uses a few libraries that both extend the Array.prototype by adding the same contains method, the implementations will overwrite each other and your code will break if the behavior of these two methods is not the same.

### Difference between document load event and document DOMContentLoaded event?
The DOMContentLoaded event is fired when the initial HTML document has been completely loaded and parsed, without waiting for styleshees, images, and subframes to finish loading.

window's load event is only fired after the DOM and all dependent resources and assets have loaded

### What is difference between == and ===?
`==` is the abstract equality operator while `===` is the strict equality operator. The `==` operator will compare for equality after doing any necessary type conversions. The `===` operator will not do type conversion, so if two values are not same type `===` will simply return false.

### Explain the same-origin policy with regards to JavaScript.
The same-origin policy prevents JavaScript from making requests across domain boundaries. An origin is defined as a combination of URL scheme, hostname, and port number. This policy prevents a malicious script on one page from obtaining access to sensitive data on another web page through that page's Document Object Model.

### Make this work:
```
duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]

function duplicate(arr) {
  return arr.concat(arr);
}

duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]
```

### Why is it called a Ternary expression, what does the word "Ternary" indicate.
"Ternary" indicates three, and a ternary expression accepts three operands, the test condition, the "then" expression and the "else" expression.

### Create a for loop that iterates up to 100 while outputting "fizz" at multiples of 3, "buzz" at multiples of 5 and "fizzbuzz" at multiples of 3 and 5.
```
for (let i = 1; i <= 100; i++) {
	let a  = i % 3  === 0;
	let b = i % 5 === 0;
	console.log(`${a} ? (${b} ? 'FizzBuzz' : 'Fizz') : ${b} : 'Buzz' : ''`)
}
```

### Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
Every script has access to the global scope, and if everyone uses the global namespece to define their variables, conflicts will occur. Use the module pattern (IIFEs) to keep your variables within a local namespece.

### Explain what a single page app is and how to make one SEO-friendly.
Web apps tend to be highly interactive and dynamic, allowing the user to perform actions and receive a response to their action. Traditionally, the browser receives HTML from the server and renders it. When the user navigates to another URL, a full-page refresh is required and the server sends fresh new HTML to the new page. This is server-side rendering.

However, in modern SPAs, client-side rendering is used instead. The browser loads the initial page from the server, along with the scripts (frameworks, libraries, app code) and stylesheets required for the whole app. When the user navigates to other page, a pagre refresh is not triggered. The URL of the page is updated via the HTML History API. New data requiredfor the new page, usually in JSON format, is retrieved by the browser via AJAX requests to the server. The SPA then dynamically updates the page with the data via JavaScript, which it has already downloaded in the initial page load. This model is similar to how native mobile apps work.

The benefit:
 - The app feels more responsive and users do not see the flash between page navigations due to full-page refreshes.
 - Fewer HTTP requests are made to the server, as the same assets do not have to be downloaded again for each page load.
 - Clear separation of the concerns between the client and the server; you can easily build new clients for different platform without having to modify the server code. You can also modify the technology stack on the client and server independently, as long as the API contract is not broken.

The disadvantages:
- HEavier initial page load due to the loading of framework, app code, and assets required for multiple pages.
- There is an additional step to be done on your server which is to configure it to route all requests to a single entry point and allow client-side routing to take over from there.
- SPAs are reliant on JS to render content, but not all search engines execute JavaScript during crawling, and they may see empty content on my page. This hurts the Search Engine Optimization of your app. However, most of the time, when you are building apps, SEO is not the most important factor, as not all the content needs to be indexable by search engines. To overcome this, you can either server-side render your app or use services such as Prerender to "render your javascript in a browser", save the static HTML.

### What are the pros and cons of using Promises instead of callbacks?
Benefits:
 - Avoid callback hell
 - make it easy to write asynchhronous code that is readable with .then()
 - make it easy to write parallel asynchronous code with Promise.all()
 
 Disadvantages:
 - slightly more complex code
 - ES6 is not supported in older browsers

### What tools and techniques do you use for debugging JavaScript code?
- React and Redux
  - React Devtools
  - Redux Devtools
 
- Vue
  - Vue Devtools
  
- JavaScript
 - Chrome Devtools
 - debugger statemenet
 - console.log() debugging

### Explain the difference between mutable and immutable objects.
mutable object can be changed after created. Immutable object is not allow to be changed, it will make test, development easier and reduce side effect.

### Explain the difference between synchronous and asynchronous functions.
Synchronous functions are blocking while asynchrounous function are not. In synchronous functions, statements complete before the next statement is run. In this case, the program is evaluated exactly in order of the statements and execution of the program is paused if one of the statements take a very long time.

Asynchronous functions usually accept a callbakc as a parameter and execution continue on the next line immediately after the asynchronous function is invoked. The callback is only invoked when the asynchronous operation is complete and the call stack is empty. Heavy duty operations such as loading data from a web server or querying a database should be done asynchronously so that the main thread can continue executing other operations instead of blocking until that long operation to complete (in the case of browsers, the UI will freeze).

### What is event loop? What is the difference between call stack and task queue?
The event loop is a single-threaded loop that monitors the call stack and checks if there is any work to be done in the task queue. If the call stack is empty and there are callback functions in the task queue, a function is dequeued and pushed onto the call stack to be executed.

Event loop will push the first event on the task queue to stack.

### Explain the differences on the usage of foo between function foo() {} and var foo = function() {}
The former is a function declaration while the latter is a function expression. They key difference is that function declarations have its body hoisted but the bodies of function expression are not.

Function Declaration
```
foo(); // 'FOOOOO'
function foo() {
  console.log('FOOOOO');
}
```
function expression
```
foo() // Uncaught TypeError: foo is not a function
var foo = function () {
	console.log('Foo')
}
```

### What are the differences between variables created using let, var or const?
Variables declared using the var keyword are scoped to the function in which they are created, or if created outside of any function, to the global object. let and const are block scoped, meaning they are only accessible within the nearest set of curly braces (function, if-else block, or for-loop).

var allows variables to be hoisted, meaning they can be referenced in code before they are declared. let and const will not allow this, instead throwing an error.

Redeclaring a variable with var will not throw an error, but 'let' and 'const' will.

let allows reassigning the variable's value while const does not.


### What are the differences between ES6 class and ES5 function constructors?
```
// ES5 Function Constructor
function Student(name, studentId) {
  // Call constructor of superclass to initialize superclass-derived members.
  Person.call(this, name);

  // Initialize subclass's own members.
  this.studentId = studentId;
}

Student.prototype = Object.create(Person.prototype);
Student.prototype.constructor = Student;

// ES6 Class
class Student extends Person {
  constructor(name, studentId) {
    super(name);
    this.studentId = studentId;
  }
}
```

### Can you offer a use case for the new arrow => function syntax? How does this new syntax differ from other functions?
One obvious benefit of arrow functions is to simplify the syntax to create function s, without a need for the function keyword. The this within arrow functions is also bound to the enclosing scope. 

### What is the definition of a higher-order function?
A higher-order function is any function that takes one or more functions as arguments, which it uses to operate on some data, and/or returns a function as a result. Higher-order functions are meant to abstract some operation that is performed repeatedly. The classic example of this is map, which takes an array and a function as arguments. map then uses this function to transform each item in the array, returning a new array with the transformed data. Other popular examples in JavaScript are forEach, filter, and reduce. A higher-order function doesn't just need to be manipulating arrays as there are many use cases for returning a function from another function. Function.prototype.bind is one such example in JavaScript.

### Can you give an example for destructuring an object or an array?
Destructing is enables a succinct and convenient way to extract values of Objects or Arrays and play them into distinct variables.
Array Destruction
```
// Variable assignment.
const foo = ['one', 'two', 'three'];

const [one, two, three] = foo;
console.log(one); // "one"
console.log(two); // "two"
console.log(three); // "three"
```
Object destructuring
```
// Variable assignment.
const o = { p: 42, q: true };
const { p, q } = o;

console.log(p); // 42
console.log(q); // true
```
