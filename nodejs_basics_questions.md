## About Node.JS

### Which of below is correct about Node.JS

	a. Integrates JavaScript with additional libraries to work on Server Side
	b. Is a Java Virtual Machine (JVM) for executing JavaScript on Server Side
	c. Its the Chrome browser but executing headless on server side
	d. Is a Web server replacement for Apache HTTP, NGINX, Tomcat
	e. All of the above

### Which of these below application can be built using Node.js

	a. Desktop application
	b. A scheduler background service
	c. Large scale Web servers
	d. A file based Database server
	e. All of above
	f. None of above

### Which of below scenario makes best or ideal case for using Node.js

	a. I/O Intensive  operations
	b. Data stream processing applications
	c. Concurrent data requests
	d. Non CPU-Intensive applications
	e. All of the above

### Using Node.js which of below can be done

	a. Process data as Streams
	b. Perform Asynchronous operations
	c. Efficient use of CPU time
	d. Apply functional programming paradigm
	e. Interface with other backend services

### Which command starts a REPL session?

	a. node
	b. node -v
	c. node repl
	d. node console

### Which module is required from NODE.js to perform path operations?

	a. os module
	b. fs module
	c. path module
	d. HTTP module

----

## Data Types, String Immutability, Type checking operator

### What will be the output of below

```javascript
let foo = null;
let bar = undefined;
if (foo == bar) {
	console.log("FOO & BAR are same");
} else if (foo === bar) {
	console.log("FOO & BAR are exactly same");
} else {
	console.log("FOO & BAR are different");
}
```

	a. FOO & BAR are same
	b. FOO & BAR are exactly same
	c. FOO & BAR are different
	d. Run time error as `null` values cannot be compared or accessible
	e. None of the above

### What is the correct operator to use to print `You are the one`

```javascript
let one = 1947;
let anotherOne = '1947';

if (anotherOne /* ? which operator */ anotherOne) {
	console.log('You are the one');
}
```

	a. if (anotherOne >= one)
	b. if (anotherOne <= one)
	c. if (anotherOne = one)
	d. if (anotherOne == one)
	e. if (anotherOne === one)

### Which expression should be used apply the discount in below code snippet

```javascript
let exactAmtForDiscount = 9.999;
let cartAmount = 9;

if (exactAmtForDiscount /* operator */ cartAmount) {
	console.log('Apply discount')
} else {
	console.log('Not eligible for discount')
}
```

	a. if (parseInt(exactAmtForDiscount) == cartAmount)
	b. if (exactAmtForDiscount == cartAmount)
	c. if (exactAmtForDiscount === cartAmount)
	d. if (parseInt(exactAmtForDiscount) <= cartAmount)
	e. if (parseFloat(exactAmtForDiscount) <= parseFloat(cartAmount))

### What will be the value printed at the end

```JavaScript
let str = 'The quick brown fox jumps over the lazy dog';
str.toLowerCase();
str.toUpperCase();
console.log("value of str ", str);
```

	a. The Quick Brown Fox Jumps Over The Lazy Dog
	b. The quick brown fox jumps over the lazy dog
	c. THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG
	d. the quick brown fox jumps over the lazy dog

---

## Modules, Package.json

### Which of below is a incorrect expression to expose a function

	a. module.exports = function calculate(operation, lhs, rhs) {}
	b. exports = function calculate(operation, lhs, rhs) {}
	c. module.exports = exports = function calculate(operation, lhs, rhs) {}
	d. export function calculate(operation, lhs, rhs) {}

### Which of down below statements import foo alone in a correct way

```javascript
/* example.js */
module.exports = {
	bar,
	foo
}
```

	a. const foo = require ('./example.js');
	b. const foo = require ('./example');
	c. const { foo } = require ('./example.js');
	d. const { null, foo } = require ('./example.js');
	e. all of the above

### Which of below statement is correct about modules

a. You can have multiple methods, variables exported from a module
b. You can choose not to export and instead hide any method or variable form a module
c. Once you have exported a method, it must refer to valid JavaScript expression
d. If you don't export any thing from the module, it will not be usable by other parts of your code/project
e. All of the above

### A node package has below versions available, What is the correct `semver` symbol to include, if we want to use only version 1.8.9 or its closest stable version

##### `2.0.1`, `1.9.4`, `1.9.3`, `1.9.2`, `1.9.1`, `1.8.9`, `1.8.5`

	a. Symbol `^`
	b. Symbol `#`
	c. Symbol `~`
	d. Symbol `=`
	e. Symbol `>`

### Which of below cannot be used to maintain node.js application dependencies

	a. npm
	b. yarn
	c. npmpm
	d. bower
	e. all of above



