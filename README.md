# Javascript functions
a collaboration project of Danny, Gert & Wendy
## About functions
The first thing we need to know is that in Javascript, functions are first-class objects.
### Types of functions
* **built-in functions** = functions that already excist in javascript libraries.
* **custom functions** = a function that you wrote yourself.
* **anomymous functions** = a function without a name
* **callback** = a function that accepts a function as a paramenter.
* **methods** = how a function in an object is called.

### Why do we use functions
* reuse returning blocks of code (define once, reuse many times, use different arguments)
* to simplify your code (write it shorter)

### How to use functions
To execute a function we call or invoke a function.
```
function(arguments);
```

* stand alone
* in loops, events, conditional statements, ....
* nested in another function
* callback

### Naming conventions
* Name is usually a verb (function = action)
* Brief, accurate, describe what the function does
* Good practice to start with a verbal prefix

**examples**
* **"get"** - return a value
* **"calc"** - calculate something
* **"show"** - shows something
* **"create"** - create something
* **"check"** - check something and return a boolean

### Scope
scope = order in which the code is executed
  ! important to access functions and variables !

### Did you know...
* A function can have up to 255 parameters!
<hr>
## SYNTAX

### Anonymous function
```javascript
function(parameters){
  statements;
}
```

### Function declaration
```javascript
function name(parameters){
  statements;
}
```

### Function expression
```javascript
let name = function(parameters){
  statements;
}
```
```javascript
let name = function(para1, para2, ...){
  statements;
}
```

### Arrow function (ES6)
Shorthand writing method for a function.

**Standard arrow function accepts multiple parameters and statements.**
```javascript
let name = (parameters) => {
  statements;
}
```

**Curly brackets are optional if you have only 1 statement.**
```javascript
let name = (parameters) => statement;
```

**Parentheses are necessary when your function has no parameters.**
```javascript
let name = () => statement;
```

**Parentheses and curly brackets are optional if your function has no parameters and only 1 statement.**
```javascript
let name = parameter => statement;
```
<hr>
## Built-in functions
Javascript has already some built-in functions that you can use. Here's some examples. If you want to know more, please visit   [MDN resource](https://developer.mozilla.org/nl/docs/Web/JavaScript/Reference/Global_Objects).
* Number functions
* Boolean functions
* String functions
* Array functions
* Date functions
* Math methods

You can find a list with all built-in functions [here](https://www.tutorialspoint.com/javascript/javascript_builtin_functions).

**eval()**
Rhymes with evil! Don't use this!
[More info...](https://developer.mozilla.org/nl/docs/Web/JavaScript/Reference/Global_Objects/eval#Do_not_ever_use_eval!)

**Math.floor()**
**length()**
**slice()**
**toUpperCase()**
**join()**
**Date()**
**...**
<hr>
## Callback functions
A callback function is a function that is passed as an argument to another function, to be “called back” at a later time. A function that accepts other functions as arguments is called a **higher-order function**, which contains the logic for when the callback function gets executed.
[More info...](https://guide.freecodecamp.org/javascript/callback-functions/)

```JavaScript
function myCallbackFunction(parameter, callback){
  let cookies = "I want a cookie, " + parameter;
  callback(cookies); // 2
}

function myFunction(string){
  console.log(string);
}

createQuote("give me the cookie!", logQuote); // 1

// Result in console:
// I want a cookie, give me the cookie!
```

<hr>
## Interesting links
* [MDN documentation on functions](https://developer.mozilla.org/nl/docs/Web/JavaScript/Reference/Functions)
* [Function basics](http://javascript.info/function-basics)
* [Javascript for cats](http://jsforcats.com/)
* [5 dogs that represent Javascript](https://medium.com/@sporks/5-dogs-that-represent-javascript-ee3d42798c3c)
<hr>
## Online tutorials
* **YouTube** - [LearnWebCode - 10 days of Javascript](https://www.youtube.com/watch?v=dc-2t26Vuhs) - free
* **Udemy** - [The complete javascript course](https://www.udemy.com/the-complete-javascript-course/) - paid
