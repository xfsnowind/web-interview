# Frontend Interview Guide - Comprehensive Summary

This document provides a comprehensive summary of frontend interview topics based on Chinese frontend interview materials, translated and organized for English-speaking developers.

## Table of Contents

1. [JavaScript](#javascript)
   - [Data Types and Storage](#data-types-and-storage)
   - [Equality Operators (== vs ===)](#equality-operators--vs-)
   - [Type Conversion](#type-conversion)
   - [typeof vs instanceof](#typeof-vs-instanceof)
   - [Scope and Context](#scope-and-context)
   - [this Keyword](#this-keyword)
   - [Execution Context and Call Stack](#execution-context-and-call-stack)
   - [Closures](#closures)
   - [Prototypes and Inheritance](#prototypes-and-inheritance)
   - [new Operator](#new-operator)
   - [Function Context (bind, call, apply)](#function-context-bind-call-apply)
   - [Event Loop](#event-loop)
   - [Debounce and Throttle](#debounce-and-throttle)
   - [Deep vs Shallow Copy](#deep-vs-shallow-copy)
   - [Memory Leaks](#memory-leaks)
   - [Array APIs](#array-apis)
   - [String APIs](#string-apis)
   - [Regular Expressions](#regular-expressions)
   - [AJAX and HTTP Requests](#ajax-and-http-requests)
   - [DOM Manipulation](#dom-manipulation)
   - [BOM (Browser Object Model)](#bom-browser-object-model)
   - [Event Model and Event Delegation](#event-model-and-event-delegation)
   - [Functional Programming](#functional-programming)
   - [Function Caching](#function-caching)
   - [Tail Recursion](#tail-recursion)
   - [JavaScript Data Structures](#javascript-data-structures)
   - [Floating Point Precision](#floating-point-precision)
   - [Security Considerations](#security-considerations)
   - [Single Sign-On (SSO)](#single-sign-on-sso)
   - [File Upload Techniques](#file-upload-techniques)
   - [Pull-to-Refresh and Infinite Scroll](#pull-to-refresh-and-infinite-scroll)
   - [Page Visibility API](#page-visibility-api)
   - [Caching Strategies](#caching-strategies)

2. [React](#react)
   - [React Fundamentals](#react-fundamentals)
   - [JSX to DOM](#jsx-to-dom)
   - [Virtual DOM vs Real DOM](#virtual-dom-vs-real-dom)
   - [Component Types (Class vs Function)](#component-types-class-vs-function)
   - [React Hooks](#react-hooks)
   - [Component Lifecycle](#component-lifecycle)
   - [State vs Props](#state-vs-props)
   - [setState Mechanism](#setstate-mechanism)
   - [Component Communication](#component-communication)
   - [Controlled vs Uncontrolled Components](#controlled-vs-uncontrolled-components)
   - [React Keys](#react-keys)
   - [React Refs](#react-refs)
   - [Event Binding](#event-binding)
   - [SyntheticEvent](#syntheticevent)
   - [Higher Order Components (HOC)](#higher-order-components-hoc)
   - [Render Props](#render-props)
   - [React Fiber](#react-fiber)
   - [Diff Algorithm](#diff-algorithm)
   - [Performance Optimization](#performance-optimization)
   - [Error Boundaries](#error-boundaries)
   - [React Router](#react-router)
   - [Redux State Management](#redux-state-management)
   - [Redux Middleware](#redux-middleware)
   - [Immutable Data](#immutable-data)
   - [CSS in React](#css-in-react)
   - [Animations](#animations)
   - [Server-Side Rendering (SSR)](#server-side-rendering-ssr)
   - [Building Components](#building-components)
   - [super() vs super(props)](#super-vs-superprops)

3. [CSS](#css)
   - [CSS Selectors](#css-selectors)
   - [Box Model](#box-model)
   - [BFC (Block Formatting Context)](#bfc-block-formatting-context)
   - [Flexbox Layout](#flexbox-layout)
   - [CSS Grid](#css-grid)
   - [Positioning and Layout](#positioning-and-layout)
   - [Centering Techniques](#centering-techniques)
   - [Column Layouts](#column-layouts)
   - [Responsive Design](#responsive-design)
   - [CSS Units (px, em, rem, vh, vw)](#css-units-px-em-rem-vh-vw)
   - [Device Pixels and DPR](#device-pixels-and-dpr)
   - [CSS3 Features](#css3-features)
   - [CSS Animations](#css-animations)
   - [CSS Performance](#css-performance)
   - [Layout and Painting](#layout-and-painting)
   - [Visual Scrolling](#visual-scrolling)
   - [Hide Elements](#hide-elements)
   - [Text Handling](#text-handling)
   - [CSS Shapes (Triangles)](#css-shapes-triangles)
   - [Font Size Limitations](#font-size-limitations)
   - [CSS Preprocessors](#css-preprocessors)

4. [ES6](#es6)
   - [Variable Declarations (var, let, const)](#variable-declarations-var-let-const)
   - [Arrow Functions](#arrow-functions)
   - [Template Literals](#template-literals)
   - [Destructuring](#destructuring)
   - [Promises](#promises)
   - [Async/Await](#asyncawait)
   - [Modules](#modules)
   - [Classes](#classes)
   - [Generators](#generators)
   - [Iterators](#iterators)
   - [Set and Map](#set-and-map)
   - [Proxy](#proxy)
   - [Reflect](#reflect)
   - [Symbols](#symbols)
   - [Array Methods](#array-methods)
   - [Object Enhancements](#object-enhancements)
   - [Decorators](#decorators)

5. [HTTP](#http)
   - [HTTP vs HTTPS](#http-vs-https)
   - [HTTP Versions (1.0, 1.1, 2.0)](#http-versions-10-11-20)
   - [HTTPS Security](#https-security)
   - [HTTP Status Codes](#http-status-codes)
   - [HTTP Headers](#http-headers)
   - [GET vs POST](#get-vs-post)
   - [TCP vs UDP](#tcp-vs-udp)
   - [TCP/IP Protocol](#tcpip-protocol)
   - [OSI Model](#osi-model)
   - [DNS Resolution](#dns-resolution)
   - [CDN (Content Delivery Network)](#cdn-content-delivery-network)
   - [TCP Handshakes and Termination](#tcp-handshakes-and-termination)
   - [URL to Page Load Process](#url-to-page-load-process)
   - [WebSocket](#websocket)

6. [TypeScript](#typescript)
   - [TypeScript vs JavaScript](#typescript-vs-javascript)
   - [Data Types](#data-types)
   - [Interfaces](#interfaces)
   - [Classes](#classes-1)
   - [Functions](#functions)
   - [Generics](#generics)
   - [Advanced Types](#advanced-types)
   - [Enums](#enums)
   - [Decorators](#decorators-1)
   - [Namespaces and Modules](#namespaces-and-modules)
   - [TypeScript with React](#typescript-with-react)

7. [Webpack](#webpack)
   - [Webpack Fundamentals](#webpack-fundamentals)
   - [Build Process](#build-process)
   - [Loaders](#loaders)
   - [Plugins](#plugins)
   - [Loaders vs Plugins](#loaders-vs-plugins)
   - [Hot Module Replacement (HMR)](#hot-module-replacement-hmr)
   - [Performance Optimization](#performance-optimization-1)
   - [Build Optimization](#build-optimization)
   - [Development Proxy](#development-proxy)
   - [Alternative Bundlers](#alternative-bundlers)

---

## JavaScript

### Data Types and Storage

**Primitive Types:**
- Number, String, Boolean, Undefined, null, Symbol
- Stored in **stack memory**
- Assignment creates independent copies

**Reference Types:**
- Object, Array, Function
- Stored in **heap memory** with references in stack
- Assignment copies references, not values

**Key Differences:**
```js
// Primitive - independent copies
let a = 10;
let b = a;
b = 20;
console.log(a); // 10

// Reference - shared reference
let obj1 = {};
let obj2 = obj1;
obj2.name = "test";
console.log(obj1.name); // "test"
```

### Debounce and Throttle

**Critical performance optimization techniques for high-frequency events.**

**Debounce Implementation:**
```js
function debounce(func, wait, immediate) {
    let timeout;
    return function () {
        let context = this;
        let args = arguments;
        
        if (timeout) clearTimeout(timeout);
        if (immediate) {
            let callNow = !timeout;
            timeout = setTimeout(function () {
                timeout = null;
            }, wait)
            if (callNow) func.apply(context, args)
        } else {
            timeout = setTimeout(function () {
                func.apply(context, args)
            }, wait);
        }
    }
}
```

**Throttle Implementation:**

```js
function throttled(fn, delay) {
    let timer = null;
    let starttime = Date.now();
    return function () {
        let curTime = Date.now();
        let remaining = delay - (curTime - starttime);
        let context = this;
        let args = arguments;
        clearTimeout(timer);
        if (remaining <= 0) {
            fn.apply(context, args);
            starttime = Date.now();
        } else {
            timer = setTimeout(fn, remaining);
        }
    }
}
```

**Use Cases:**
- **Debounce:** Search input, form validation, window resize
- **Throttle:** Scroll events, mouse movement, API calls

### Function Context (bind, call, apply)

**All three methods change function execution context (`this` binding).**

**Key Differences:**
- `call(thisArg, arg1, arg2, ...)` - immediate execution, individual arguments
- `apply(thisArg, [argsArray])` - immediate execution, array of arguments  
- `bind(thisArg, arg1, arg2, ...)` - returns new function, partial application

**Custom bind Implementation:**

```js
Function.prototype.myBind = function (context) {
    if (typeof this !== "function") {
        throw new TypeError("Error");
    }
    
    const args = [...arguments].slice(1);
    const fn = this;
    
    return function Fn() {
        return fn.apply(
            this instanceof Fn ? new fn(...arguments) : context, 
            args.concat(...arguments)
        ); 
    }
}
```

### Closures

**Definition:** A function combined with references to its surrounding state (lexical environment).

**Core Use Cases:**
1. **Creating private variables**
2. **Extending variable lifetime**

**Practical Examples:**

**Module Pattern:**
```js
var Counter = (function() {
    var privateCounter = 0;
    function changeBy(val) {
        privateCounter += val;
    }
    return {
        increment: function() { changeBy(1); },
        decrement: function() { changeBy(-1); },
        value: function() { return privateCounter; }
    }
})();
```

**Currying:**
```js
function getArea(width) {
    return height => width * height;
}
const getTenWidthArea = getArea(10);
const area1 = getTenWidthArea(20); // 200
```

### Event Loop

**JavaScript is single-threaded but achieves non-blocking behavior through the event loop.**

**Task Categories:**
- **Macrotasks:** setTimeout, setInterval, I/O, UI rendering
- **Microtasks:** Promise.then, MutationObserver, process.nextTick

**Execution Order:**
1. Execute current macrotask
2. Execute all microtasks in queue
3. Repeat with next macrotask

**Example Analysis:**

```js
console.log('script start');
settimeout(() => console.log('settimeout'), 0);
promise.resolve().then(() => console.log('promise'));
console.log('script end');

// Output: script start → script end → promise → setTimeout
```

### Prototypes and Prototype Chain

**Every object has a prototype chain that enables inheritance.**

**Key Concepts:**
- `__proto__` links objects to their constructor's prototype
- `prototype` property exists on constructor functions
- Chain traversal continues until `null` is reached

**Prototype Relationships:**
```js
function Person(name) {
    this.name = name;
}
const person = new Person('John');

person.__proto__ === Person.prototype; // true
Person.prototype.__proto__ === Object.prototype; // true
Object.prototype.__proto__ === null; // true
```

### Equality Operators (== vs ===)

**== (Equality) performs type coercion, === (Strict Equality) does not.**

**Type Coercion Rules for ==:**
- Boolean values convert to numbers
- String and number comparison converts string to number
- Object comparison calls `valueOf()` method
- `null == undefined` returns `true`
- `NaN` comparisons always return `false`

**Examples:**
```js
// Type coercion examples
true == 1;           // true (boolean to number)
"55" == 55;          // true (string to number)
null == undefined;   // true (special case)
NaN == NaN;          // false (NaN rule)

// Strict equality
"55" === 55;         // false (different types)
null === undefined;  // false (different types)
```

**Best Practice:** Use `===` except when checking for `null/undefined`:
```js
// Concise null/undefined check
if (obj.x == null) { /* handles both null and undefined */ }

// Equivalent to:
if (obj.x === null || obj.x === undefined) { /* verbose */ }
```

### Type Conversion

**JavaScript performs implicit type conversion in various contexts.**

**Common Conversion Scenarios:**
```js
// String conversion
String(123);        // "123"
123 + "";          // "123"

// Number conversion
Number("123");      // 123
+"123";            // 123
"123" - 0;         // 123

// Boolean conversion
Boolean(0);         // false
!!0;               // false

// Falsy values: false, 0, "", null, undefined, NaN
// Everything else is truthy
```

**Object to Primitive Conversion:**
```js
const obj = {
    valueOf() { return 42; },
    toString() { return "hello"; }
};

obj + 1;    // 43 (valueOf called)
obj + "";   // "42" (valueOf called)
String(obj); // "hello" (toString called)
```

### typeof vs instanceof

**`typeof` returns primitive type strings, `instanceof` checks prototype chain.**

```js
// typeof examples
typeof 42;              // "number"
typeof "hello";         // "string"
typeof true;            // "boolean"
typeof undefined;       // "undefined"
typeof null;            // "object" (historical bug)
typeof {};              // "object"
typeof [];              // "object"
typeof function(){};    // "function"

// instanceof examples
[] instanceof Array;           // true
[] instanceof Object;          // true
function(){} instanceof Function; // true

// Custom constructor
function Person() {}
const p = new Person();
p instanceof Person;           // true
p instanceof Object;           // true
```

**Safe Type Checking:**
```js
// Better array detection
Array.isArray([]);             // true
Array.isArray({});             // false

// Object type detection
Object.prototype.toString.call([]); // "[object Array]"
Object.prototype.toString.call({}); // "[object Object]"
```

### Scope and Context

**Scope determines variable accessibility, context refers to `this` value.**

**Lexical Scope:**
```js
function outer() {
    const x = 1;

    function inner() {
        console.log(x); // 1 (lexical scope)
    }

    return inner;
}

const fn = outer();
fn(); // Still accesses x from outer scope
```

**Block Scope (let/const):**
```js
if (true) {
    let blockScoped = "only here";
    var functionScoped = "everywhere in function";
}

// console.log(blockScoped); // ReferenceError
console.log(functionScoped); // "everywhere in function"
```

**Execution Context:**
- **Global Context:** Default execution environment
- **Function Context:** Created when function is called
- **Eval Context:** Created by eval() function

### this Keyword

**`this` value depends on how function is called, not where it's defined.**

**Binding Rules (in order of precedence):**

1. **new Binding:**
```js
function Constructor() {
    this.value = 42;
}
const obj = new Constructor(); // this = new object
```

2. **Explicit Binding:**
```js
function fn() { return this.value; }
const obj = { value: 42 };
fn.call(obj);  // this = obj
fn.apply(obj); // this = obj
fn.bind(obj)(); // this = obj
```

3. **Implicit Binding:**
```js
const obj = {
    value: 42,
    fn() { return this.value; }
};
obj.fn(); // this = obj
```

4. **Default Binding:**
```js
function fn() { return this; }
fn(); // this = window (or undefined in strict mode)
```

**Arrow Functions:**
```js
const obj = {
    value: 42,
    regular: function() {
        return () => this.value; // Arrow function inherits this
    }
};

const arrow = obj.regular();
arrow(); // 42 (this from regular function)
```

### Execution Context and Call Stack

**Execution context contains variable environment, scope chain, and this binding.**

**Context Creation Phases:**
1. **Creation Phase:**
   - Variable declarations are hoisted
   - Function declarations are hoisted
   - `this` binding is determined

2. **Execution Phase:**
   - Code is executed line by line
   - Variables are assigned values

**Hoisting Examples:**
```js
console.log(x); // undefined (not ReferenceError)
var x = 5;

console.log(fn); // function fn() {...}
function fn() { return "hoisted"; }

// let/const are hoisted but in "temporal dead zone"
console.log(y); // ReferenceError
let y = 10;
```

**Call Stack:**
```js
function first() {
    console.log("First");
    second();
    console.log("First again");
}

function second() {
    console.log("Second");
    third();
    console.log("Second again");
}

function third() {
    console.log("Third");
}

first();
// Output: First → Second → Third → Second again → First again
```

### Prototypes and Inheritance

**JavaScript uses prototype-based inheritance rather than classical inheritance.**

**Prototype Chain:**
```javascript
function Animal(name) {
    this.name = name;
}

Animal.prototype.speak = function() {
    return `${this.name} makes a sound`;
};

function Dog(name, breed) {
    Animal.call(this, name); // Call parent constructor
    this.breed = breed;
}

// Set up inheritance
Dog.prototype = Object.create(Animal.prototype);
Dog.prototype.constructor = Dog;

Dog.prototype.speak = function() {
    return `${this.name} barks`;
};

const dog = new Dog("Rex", "German Shepherd");
dog.speak(); // "Rex barks"
```

**ES6 Class Syntax:**
```javascript
class Animal {
    constructor(name) {
        this.name = name;
    }

    speak() {
        return `${this.name} makes a sound`;
    }
}

class Dog extends Animal {
    constructor(name, breed) {
        super(name);
        this.breed = breed;
    }

    speak() {
        return `${this.name} barks`;
    }
}
```

### new Operator

**The `new` operator creates instances of constructor functions.**

**What `new` does:**
1. Creates a new empty object
2. Sets the object's prototype to constructor's prototype
3. Binds `this` to the new object
4. Executes constructor function
5. Returns the object (or constructor's return value if object)

**Custom `new` Implementation:**
```javascript
function myNew(constructor, ...args) {
    // Create new object with constructor's prototype
    const obj = Object.create(constructor.prototype);

    // Call constructor with new object as this
    const result = constructor.apply(obj, args);

    // Return object or constructor result if it's an object
    return result instanceof Object ? result : obj;
}

// Usage
function Person(name) {
    this.name = name;
}

const person1 = new Person("John");
const person2 = myNew(Person, "Jane");
```

### Deep vs Shallow Copy

**Shallow copy copies only the first level, deep copy copies all nested levels.**

**Shallow Copy Methods:**
```javascript
// Object.assign
const shallow1 = Object.assign({}, original);

// Spread operator
const shallow2 = { ...original };

// Array methods
const arrShallow1 = [...originalArray];
const arrShallow2 = originalArray.slice();
```

**Deep Copy Methods:**
```javascript
// JSON method (limited - no functions, dates, etc.)
const deep1 = JSON.parse(JSON.stringify(original));

// Custom recursive function
function deepClone(obj) {
    if (obj === null || typeof obj !== "object") return obj;
    if (obj instanceof Date) return new Date(obj);
    if (obj instanceof Array) return obj.map(item => deepClone(item));
    if (typeof obj === "object") {
        const cloned = {};
        Object.keys(obj).forEach(key => {
            cloned[key] = deepClone(obj[key]);
        });
        return cloned;
    }
}

// Using Lodash
const deep2 = _.cloneDeep(original);
```

**Demonstration:**
```javascript
const original = {
    name: "John",
    address: { city: "New York", zip: "10001" }
};

const shallow = { ...original };
const deep = deepClone(original);

original.address.city = "Boston";

console.log(shallow.address.city); // "Boston" (reference shared)
console.log(deep.address.city);    // "New York" (independent copy)
```

### Memory Leaks

**Common causes and prevention of memory leaks in JavaScript.**

**Common Leak Sources:**

1. **Global Variables:**
```javascript
// Bad - creates global variable
function createLeak() {
    leak = "I'm global!"; // Missing var/let/const
}

// Good - proper scoping
function noLeak() {
    const local = "I'm local!";
}
```

2. **Event Listeners:**
```javascript
// Bad - listener not removed
element.addEventListener('click', handler);

// Good - cleanup
element.addEventListener('click', handler);
// Later...
element.removeEventListener('click', handler);

// Or use AbortController
const controller = new AbortController();
element.addEventListener('click', handler, {
    signal: controller.signal
});
// Later...
controller.abort();
```

3. **Timers:**
```javascript
// Bad - timer keeps running
const timer = setInterval(() => {
    // Some operation
}, 1000);

// Good - clear timer
const timer = setInterval(() => {
    // Some operation
}, 1000);
clearInterval(timer);
```

4. **Closures:**
```javascript
// Bad - unnecessary closure retention
function attachListeners() {
    const largeData = new Array(1000000).fill('data');

    document.getElementById('button').onclick = function() {
        // largeData is retained even if not used
        console.log('clicked');
    };
}

// Good - avoid unnecessary retention
function attachListeners() {
    const largeData = new Array(1000000).fill('data');
    const processedData = largeData.length; // Extract what you need

    document.getElementById('button').onclick = function() {
        console.log('clicked', processedData);
    };
}
```

### Array APIs

**Essential array methods for data manipulation.**

**Mutating Methods:**
```javascript
const arr = [1, 2, 3];

// Add/remove elements
arr.push(4);           // [1, 2, 3, 4]
arr.pop();             // [1, 2, 3]
arr.unshift(0);        // [0, 1, 2, 3]
arr.shift();           // [1, 2, 3]

// Modify elements
arr.splice(1, 1, 'new'); // [1, 'new', 3]
arr.sort();            // Sorts in place
arr.reverse();         // Reverses in place
```

**Non-mutating Methods:**
```javascript
const arr = [1, 2, 3, 4, 5];

// Transform
const doubled = arr.map(x => x * 2);        // [2, 4, 6, 8, 10]
const filtered = arr.filter(x => x > 2);    // [3, 4, 5]
const sum = arr.reduce((acc, x) => acc + x, 0); // 15

// Search
const found = arr.find(x => x > 3);         // 4
const index = arr.findIndex(x => x > 3);    // 3
const includes = arr.includes(3);           // true

// Test
const allPositive = arr.every(x => x > 0);  // true
const hasEven = arr.some(x => x % 2 === 0); // true

// Combine
const combined = arr.concat([6, 7]);        // [1, 2, 3, 4, 5, 6, 7]
const sliced = arr.slice(1, 3);            // [2, 3]
```

**Advanced Patterns:**
```javascript
// Chaining
const result = [1, 2, 3, 4, 5]
    .filter(x => x % 2 === 0)
    .map(x => x * 2)
    .reduce((acc, x) => acc + x, 0); // 12

// Flattening
const nested = [[1, 2], [3, 4], [5]];
const flat = nested.flat();              // [1, 2, 3, 4, 5]
const flatMapped = nested.flatMap(arr => arr.map(x => x * 2)); // [2, 4, 6, 8, 10]

// Grouping (ES2021)
const people = [
    { name: 'John', age: 25 },
    { name: 'Jane', age: 30 },
    { name: 'Bob', age: 25 }
];
const grouped = people.reduce((acc, person) => {
    const age = person.age;
    if (!acc[age]) acc[age] = [];
    acc[age].push(person);
    return acc;
}, {});
```

### String APIs

**Essential string methods for text manipulation.**

**Basic Operations:**
```javascript
const str = "Hello World";

// Length and access
str.length;                    // 11
str[0];                       // "H"
str.charAt(0);                // "H"
str.charCodeAt(0);            // 72

// Search
str.indexOf("World");         // 6
str.lastIndexOf("l");         // 9
str.includes("World");        // true
str.startsWith("Hello");      // true
str.endsWith("World");        // true
```

**Transformation:**
```javascript
const str = "  Hello World  ";

// Case
str.toLowerCase();            // "  hello world  "
str.toUpperCase();            // "  HELLO WORLD  "

// Trimming
str.trim();                   // "Hello World"
str.trimStart();              // "Hello World  "
str.trimEnd();                // "  Hello World"

// Replacement
str.replace("World", "JS");   // "  Hello JS  "
str.replaceAll("l", "L");     // "  HeLLo WorLd  "

// Splitting and joining
str.split(" ");               // ["", "", "Hello", "World", "", ""]
str.split(" ").filter(Boolean); // ["Hello", "World"]
```

**Advanced Methods:**
```javascript
// Padding
"5".padStart(3, "0");         // "005"
"5".padEnd(3, "0");           // "500"

// Repetition
"abc".repeat(3);              // "abcabcabc"

// Slicing
"Hello World".slice(0, 5);    // "Hello"
"Hello World".substring(0, 5); // "Hello"
"Hello World".substr(0, 5);   // "Hello" (deprecated)

// Template literals
const name = "John";
const age = 30;
const message = `Hello ${name}, you are ${age} years old`;
```

### Regular Expressions

**Pattern matching and text processing with regex.**

**Basic Patterns:**
```javascript
// Literal notation
const regex1 = /pattern/flags;

// Constructor notation
const regex2 = new RegExp('pattern', 'flags');

// Common flags
// g - global (find all matches)
// i - case insensitive
// m - multiline
// s - dotall (. matches newlines)
```

**Common Methods:**
```javascript
const text = "The quick brown fox jumps over the lazy dog";
const pattern = /quick|lazy/gi;

// Test for match
pattern.test(text);           // true

// Find matches
text.match(pattern);          // ["quick", "lazy"]
text.search(pattern);         // 4 (index of first match)

// Replace with regex
text.replace(/quick/gi, "slow"); // "The slow brown fox..."

// Split with regex
"a,b;c:d".split(/[,;:]/);     // ["a", "b", "c", "d"]
```

**Practical Examples:**
```javascript
// Email validation
const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
emailRegex.test("user@example.com"); // true

// Phone number extraction
const phoneRegex = /\(?\d{3}\)?[-.\s]?\d{3}[-.\s]?\d{4}/g;
"Call (555) 123-4567 or 555.987.6543".match(phoneRegex);

// URL validation
const urlRegex = /^https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)$/;

// Password strength (8+ chars, uppercase, lowercase, number, special)
const passwordRegex = /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$/;
```

### AJAX and HTTP Requests

**Making asynchronous HTTP requests in JavaScript.**

**XMLHttpRequest (Legacy):**
```javascript
function makeRequest(url, method = 'GET', data = null) {
    return new Promise((resolve, reject) => {
        const xhr = new XMLHttpRequest();

        xhr.open(method, url);
        xhr.setRequestHeader('Content-Type', 'application/json');

        xhr.onload = function() {
            if (xhr.status >= 200 && xhr.status < 300) {
                resolve(JSON.parse(xhr.responseText));
            } else {
                reject(new Error(`HTTP ${xhr.status}: ${xhr.statusText}`));
            }
        };

        xhr.onerror = () => reject(new Error('Network error'));

        xhr.send(data ? JSON.stringify(data) : null);
    });
}
```

**Fetch API (Modern):**
```javascript
// Basic GET request
async function fetchData(url) {
    try {
        const response = await fetch(url);

        if (!response.ok) {
            throw new Error(`HTTP ${response.status}: ${response.statusText}`);
        }

        const data = await response.json();
        return data;
    } catch (error) {
        console.error('Fetch error:', error);
        throw error;
    }
}

// POST request with data
async function postData(url, data) {
    const response = await fetch(url, {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
            'Authorization': 'Bearer token'
        },
        body: JSON.stringify(data)
    });

    return response.json();
}

// File upload
async function uploadFile(url, file) {
    const formData = new FormData();
    formData.append('file', file);

    const response = await fetch(url, {
        method: 'POST',
        body: formData // Don't set Content-Type for FormData
    });

    return response.json();
}
```

**Request Interceptors and Error Handling:**
```javascript
class ApiClient {
    constructor(baseURL) {
        this.baseURL = baseURL;
        this.defaultHeaders = {
            'Content-Type': 'application/json'
        };
    }

    async request(endpoint, options = {}) {
        const url = `${this.baseURL}${endpoint}`;
        const config = {
            headers: { ...this.defaultHeaders, ...options.headers },
            ...options
        };

        try {
            const response = await fetch(url, config);

            if (!response.ok) {
                throw new Error(`HTTP ${response.status}`);
            }

            return await response.json();
        } catch (error) {
            console.error('API request failed:', error);
            throw error;
        }
    }

    get(endpoint, options) {
        return this.request(endpoint, { method: 'GET', ...options });
    }

    post(endpoint, data, options) {
        return this.request(endpoint, {
            method: 'POST',
            body: JSON.stringify(data),
            ...options
        });
    }
}

// Usage
const api = new ApiClient('https://api.example.com');
const users = await api.get('/users');
const newUser = await api.post('/users', { name: 'John', email: 'john@example.com' });
```

### DOM Manipulation

**Interacting with the Document Object Model.**

**Element Selection:**
```javascript
// Single element
const element = document.getElementById('myId');
const element2 = document.querySelector('.myClass');
const element3 = document.querySelector('[data-id="123"]');

// Multiple elements
const elements = document.getElementsByClassName('myClass');
const elements2 = document.querySelectorAll('.myClass');
const elements3 = document.getElementsByTagName('div');
```

**Element Creation and Modification:**
```javascript
// Create elements
const div = document.createElement('div');
const text = document.createTextNode('Hello World');

// Set attributes and properties
div.id = 'myDiv';
div.className = 'container';
div.setAttribute('data-id', '123');
div.style.backgroundColor = 'blue';

// Modify content
div.textContent = 'Text content';
div.innerHTML = '<span>HTML content</span>';

// Add to DOM
document.body.appendChild(div);
document.body.insertBefore(div, existingElement);
```

**Event Handling:**
```javascript
// Add event listeners
element.addEventListener('click', handleClick);
element.addEventListener('click', handleClick, { once: true });

// Event delegation
document.addEventListener('click', function(event) {
    if (event.target.matches('.button')) {
        handleButtonClick(event);
    }
});

// Remove event listeners
element.removeEventListener('click', handleClick);

// Custom events
const customEvent = new CustomEvent('myEvent', {
    detail: { message: 'Hello' }
});
element.dispatchEvent(customEvent);
```

**DOM Traversal:**
```javascript
const element = document.querySelector('.target');

// Parent/child relationships
const parent = element.parentNode;
const children = element.children;
const firstChild = element.firstElementChild;
const lastChild = element.lastElementChild;

// Siblings
const nextSibling = element.nextElementSibling;
const prevSibling = element.previousElementSibling;

// Searching within element
const descendant = element.querySelector('.descendant');
const descendants = element.querySelectorAll('.descendant');
```

### BOM (Browser Object Model)

**Browser-specific objects and APIs for interacting with the browser environment.**

**Window Object:**
```javascript
// Window properties
window.innerWidth;           // Viewport width
window.innerHeight;          // Viewport height
window.outerWidth;           // Browser window width
window.outerHeight;          // Browser window height

// Window methods
window.open('url', 'name', 'features');
window.close();
window.focus();
window.blur();

// Dialogs
window.alert('Message');
const result = window.confirm('Are you sure?');
const input = window.prompt('Enter value:', 'default');
```

**Location Object:**
```javascript
// Current URL information
location.href;               // Full URL
location.protocol;           // "https:"
location.host;               // "example.com:8080"
location.hostname;           // "example.com"
location.port;               // "8080"
location.pathname;           // "/path/page"
location.search;             // "?param=value"
location.hash;               // "#section"

// Navigation
location.assign('newURL');   // Navigate to new URL
location.replace('newURL');  // Replace current URL
location.reload();           // Reload page
```

**History Object:**
```javascript
// Navigation history
history.length;              // Number of entries
history.back();              // Go back
history.forward();           // Go forward
history.go(-2);              // Go back 2 pages

// HTML5 History API
history.pushState(state, title, url);
history.replaceState(state, title, url);

// Listen for history changes
window.addEventListener('popstate', function(event) {
    console.log('History changed:', event.state);
});
```

**Navigator Object:**
```javascript
// Browser information
navigator.userAgent;         // Browser string
navigator.platform;         // Operating system
navigator.language;          // Browser language
navigator.languages;         // Preferred languages
navigator.cookieEnabled;     // Cookie support
navigator.onLine;            // Online status

// Geolocation
navigator.geolocation.getCurrentPosition(
    position => {
        console.log(position.coords.latitude, position.coords.longitude);
    },
    error => console.error(error)
);
```

### Event Model and Event Delegation

**Understanding JavaScript event system and efficient event handling.**

**Event Flow:**
```javascript
// Event phases:
// 1. Capturing phase (document → target)
// 2. Target phase (at target element)
// 3. Bubbling phase (target → document)

element.addEventListener('click', handler, true);  // Capturing
element.addEventListener('click', handler, false); // Bubbling (default)
```

**Event Object:**
```javascript
function handleEvent(event) {
    // Event properties
    event.type;              // Event type ('click', 'keydown', etc.)
    event.target;            // Element that triggered event
    event.currentTarget;     // Element with event listener
    event.timeStamp;         // When event occurred

    // Event control
    event.preventDefault();  // Prevent default behavior
    event.stopPropagation(); // Stop event bubbling
    event.stopImmediatePropagation(); // Stop other listeners

    // Mouse events
    event.clientX;           // Mouse X relative to viewport
    event.clientY;           // Mouse Y relative to viewport
    event.pageX;             // Mouse X relative to document
    event.pageY;             // Mouse Y relative to document

    // Keyboard events
    event.key;               // Key pressed ('a', 'Enter', etc.)
    event.code;              // Physical key ('KeyA', 'Enter', etc.)
    event.ctrlKey;           // Ctrl key pressed
    event.shiftKey;          // Shift key pressed
    event.altKey;            // Alt key pressed
}
```

**Event Delegation:**
```javascript
// Instead of adding listeners to many elements
document.querySelectorAll('.button').forEach(button => {
    button.addEventListener('click', handleClick);
});

// Use delegation on parent element
document.addEventListener('click', function(event) {
    // Check if clicked element matches selector
    if (event.target.matches('.button')) {
        handleClick(event);
    }

    // Or use closest for nested elements
    const button = event.target.closest('.button');
    if (button) {
        handleClick(event);
    }
});

// Benefits:
// - Better performance with many elements
// - Automatically handles dynamically added elements
// - Less memory usage
```

**Custom Events:**
```javascript
// Create custom event
const customEvent = new CustomEvent('userLogin', {
    detail: {
        userId: 123,
        username: 'john_doe'
    },
    bubbles: true,
    cancelable: true
});

// Dispatch event
element.dispatchEvent(customEvent);

// Listen for custom event
document.addEventListener('userLogin', function(event) {
    console.log('User logged in:', event.detail);
});

// Event emitter pattern
class EventEmitter {
    constructor() {
        this.events = {};
    }

    on(event, callback) {
        if (!this.events[event]) {
            this.events[event] = [];
        }
        this.events[event].push(callback);
    }

    emit(event, data) {
        if (this.events[event]) {
            this.events[event].forEach(callback => callback(data));
        }
    }

    off(event, callback) {
        if (this.events[event]) {
            this.events[event] = this.events[event].filter(cb => cb !== callback);
        }
    }
}
```

### Functional Programming

**Applying functional programming concepts in JavaScript.**

**Pure Functions:**
```javascript
// Pure function - same input always produces same output, no side effects
function add(a, b) {
    return a + b;
}

// Impure function - depends on external state
let counter = 0;
function impureIncrement() {
    return ++counter; // Side effect: modifies external variable
}

// Pure version
function pureIncrement(value) {
    return value + 1;
}
```

**Higher-Order Functions:**
```javascript
// Function that takes other functions as arguments
function withLogging(fn) {
    return function(...args) {
        console.log('Calling function with args:', args);
        const result = fn(...args);
        console.log('Function returned:', result);
        return result;
    };
}

const loggedAdd = withLogging(add);
loggedAdd(2, 3); // Logs input and output

// Function that returns other functions
function createMultiplier(factor) {
    return function(number) {
        return number * factor;
    };
}

const double = createMultiplier(2);
const triple = createMultiplier(3);
```

**Immutability:**
```javascript
// Avoid mutations
const original = [1, 2, 3];

// Bad - mutates original
original.push(4);

// Good - creates new array
const newArray = [...original, 4];
const newArray2 = original.concat(4);

// Object immutability
const originalObj = { name: 'John', age: 30 };

// Bad - mutates original
originalObj.age = 31;

// Good - creates new object
const newObj = { ...originalObj, age: 31 };
const newObj2 = Object.assign({}, originalObj, { age: 31 });
```

**Composition:**
```javascript
// Function composition
const compose = (...fns) => (value) => fns.reduceRight((acc, fn) => fn(acc), value);
const pipe = (...fns) => (value) => fns.reduce((acc, fn) => fn(acc), value);

// Example functions
const addOne = x => x + 1;
const double = x => x * 2;
const square = x => x * x;

// Compose functions
const addOneDoubleSquare = compose(square, double, addOne);
const pipeExample = pipe(addOne, double, square);

addOneDoubleSquare(3); // square(double(addOne(3))) = square(double(4)) = square(8) = 64
pipeExample(3);        // square(double(addOne(3))) = 64
```

**Currying:**
```javascript
// Manual currying
function curry(fn) {
    return function curried(...args) {
        if (args.length >= fn.length) {
            return fn.apply(this, args);
        } else {
            return function(...args2) {
                return curried.apply(this, args.concat(args2));
            };
        }
    };
}

// Example usage
const add3 = (a, b, c) => a + b + c;
const curriedAdd3 = curry(add3);

curriedAdd3(1)(2)(3); // 6
curriedAdd3(1, 2)(3); // 6
curriedAdd3(1)(2, 3); // 6

// Practical example
const filter = curry((predicate, array) => array.filter(predicate));
const map = curry((transform, array) => array.map(transform));

const isEven = x => x % 2 === 0;
const double = x => x * 2;

const filterEven = filter(isEven);
const mapDouble = map(double);

const numbers = [1, 2, 3, 4, 5, 6];
const evenNumbers = filterEven(numbers); // [2, 4, 6]
const doubledNumbers = mapDouble(numbers); // [2, 4, 6, 8, 10, 12]
```

### Function Caching

**Memoization techniques to optimize function performance.**

**Basic Memoization:**
```javascript
function memoize(fn) {
    const cache = new Map();

    return function(...args) {
        const key = JSON.stringify(args);

        if (cache.has(key)) {
            console.log('Cache hit');
            return cache.get(key);
        }

        console.log('Computing result');
        const result = fn.apply(this, args);
        cache.set(key, result);
        return result;
    };
}

// Example: Expensive fibonacci calculation
function fibonacci(n) {
    if (n <= 1) return n;
    return fibonacci(n - 1) + fibonacci(n - 2);
}

const memoizedFib = memoize(fibonacci);
memoizedFib(40); // Computed once
memoizedFib(40); // Retrieved from cache
```

**Advanced Memoization with TTL:**
```javascript
function memoizeWithTTL(fn, ttl = 60000) {
    const cache = new Map();

    return function(...args) {
        const key = JSON.stringify(args);
        const now = Date.now();

        if (cache.has(key)) {
            const { value, timestamp } = cache.get(key);
            if (now - timestamp < ttl) {
                return value;
            } else {
                cache.delete(key);
            }
        }

        const result = fn.apply(this, args);
        cache.set(key, { value: result, timestamp: now });
        return result;
    };
}

// API call caching
const fetchUserData = memoizeWithTTL(async (userId) => {
    const response = await fetch(`/api/users/${userId}`);
    return response.json();
}, 300000); // 5 minutes TTL
```

### Tail Recursion

**Optimizing recursive functions to prevent stack overflow.**

**Regular Recursion (Stack Overflow Risk):**
```javascript
function factorial(n) {
    if (n <= 1) return 1;
    return n * factorial(n - 1); // Not tail recursive
}

// Stack grows: factorial(5) → 5 * factorial(4) → 5 * 4 * factorial(3) → ...
```

**Tail Recursive Version:**
```javascript
function factorialTail(n, accumulator = 1) {
    if (n <= 1) return accumulator;
    return factorialTail(n - 1, n * accumulator); // Tail call
}

// Each call can be optimized away (in supporting environments)
```

**Trampoline Technique (Manual Optimization):**
```javascript
function trampoline(fn) {
    return function(...args) {
        let result = fn(...args);
        while (typeof result === 'function') {
            result = result();
        }
        return result;
    };
}

function factorialTrampoline(n, acc = 1) {
    if (n <= 1) return acc;
    return () => factorialTrampoline(n - 1, n * acc);
}

const factorial = trampoline(factorialTrampoline);
factorial(10000); // Won't cause stack overflow
```

### JavaScript Data Structures

**Implementing common data structures in JavaScript.**

**Stack:**
```javascript
class Stack {
    constructor() {
        this.items = [];
    }

    push(item) {
        this.items.push(item);
    }

    pop() {
        return this.items.pop();
    }

    peek() {
        return this.items[this.items.length - 1];
    }

    isEmpty() {
        return this.items.length === 0;
    }

    size() {
        return this.items.length;
    }
}
```

**Queue:**
```javascript
class Queue {
    constructor() {
        this.items = [];
    }

    enqueue(item) {
        this.items.push(item);
    }

    dequeue() {
        return this.items.shift();
    }

    front() {
        return this.items[0];
    }

    isEmpty() {
        return this.items.length === 0;
    }

    size() {
        return this.items.length;
    }
}
```

**Linked List:**
```javascript
class ListNode {
    constructor(data) {
        this.data = data;
        this.next = null;
    }
}

class LinkedList {
    constructor() {
        this.head = null;
        this.size = 0;
    }

    append(data) {
        const newNode = new ListNode(data);

        if (!this.head) {
            this.head = newNode;
        } else {
            let current = this.head;
            while (current.next) {
                current = current.next;
            }
            current.next = newNode;
        }
        this.size++;
    }

    prepend(data) {
        const newNode = new ListNode(data);
        newNode.next = this.head;
        this.head = newNode;
        this.size++;
    }

    remove(data) {
        if (!this.head) return false;

        if (this.head.data === data) {
            this.head = this.head.next;
            this.size--;
            return true;
        }

        let current = this.head;
        while (current.next && current.next.data !== data) {
            current = current.next;
        }

        if (current.next) {
            current.next = current.next.next;
            this.size--;
            return true;
        }

        return false;
    }

    find(data) {
        let current = this.head;
        while (current) {
            if (current.data === data) return current;
            current = current.next;
        }
        return null;
    }
}
```

**Binary Tree:**
```javascript
class TreeNode {
    constructor(data) {
        this.data = data;
        this.left = null;
        this.right = null;
    }
}

class BinarySearchTree {
    constructor() {
        this.root = null;
    }

    insert(data) {
        const newNode = new TreeNode(data);

        if (!this.root) {
            this.root = newNode;
            return;
        }

        this.insertNode(this.root, newNode);
    }

    insertNode(node, newNode) {
        if (newNode.data < node.data) {
            if (!node.left) {
                node.left = newNode;
            } else {
                this.insertNode(node.left, newNode);
            }
        } else {
            if (!node.right) {
                node.right = newNode;
            } else {
                this.insertNode(node.right, newNode);
            }
        }
    }

    search(data) {
        return this.searchNode(this.root, data);
    }

    searchNode(node, data) {
        if (!node) return false;

        if (data === node.data) return true;

        if (data < node.data) {
            return this.searchNode(node.left, data);
        } else {
            return this.searchNode(node.right, data);
        }
    }

    // Traversal methods
    inOrder(callback) {
        this.inOrderTraversal(this.root, callback);
    }

    inOrderTraversal(node, callback) {
        if (node) {
            this.inOrderTraversal(node.left, callback);
            callback(node.data);
            this.inOrderTraversal(node.right, callback);
        }
    }
}
```

### Floating Point Precision

**Understanding and handling JavaScript number precision issues.**

**The Problem:**
```javascript
// Floating point precision issues
0.1 + 0.2;                    // 0.30000000000000004
0.1 + 0.2 === 0.3;           // false

// Why this happens:
// JavaScript uses IEEE 754 double precision
// Some decimal numbers cannot be represented exactly in binary
```

**Solutions:**

**1. Number.EPSILON for Comparison:**
```javascript
function isEqual(a, b, epsilon = Number.EPSILON) {
    return Math.abs(a - b) < epsilon;
}

isEqual(0.1 + 0.2, 0.3);     // true
```

**2. Fixed Decimal Places:**
```javascript
function addDecimals(a, b, decimals = 2) {
    return parseFloat((a + b).toFixed(decimals));
}

addDecimals(0.1, 0.2);       // 0.3
```

**3. Integer Arithmetic:**
```javascript
function preciseAdd(a, b) {
    const factor = 100; // For 2 decimal places
    return (Math.round(a * factor) + Math.round(b * factor)) / factor;
}

preciseAdd(0.1, 0.2);        // 0.3
```

**4. Decimal.js Library:**
```javascript
// Using external library for precise decimal arithmetic
const Decimal = require('decimal.js');

const a = new Decimal(0.1);
const b = new Decimal(0.2);
const result = a.plus(b);    // 0.3
```

**Safe Integer Range:**
```javascript
// JavaScript can safely represent integers up to:
Number.MAX_SAFE_INTEGER;     // 9007199254740991
Number.MIN_SAFE_INTEGER;     // -9007199254740991

// Check if number is safe integer
Number.isSafeInteger(9007199254740991);  // true
Number.isSafeInteger(9007199254740992);  // false

// For larger integers, use BigInt
const bigInt = 9007199254740992n;
const bigInt2 = BigInt(9007199254740992);
```

### Security Considerations

**Common security vulnerabilities and prevention techniques in JavaScript.**

**Cross-Site Scripting (XSS):**
```javascript
// Dangerous - never do this
function dangerousHTML(userInput) {
    document.innerHTML = userInput; // XSS vulnerability
}

// Safe approaches
function safeTextContent(userInput) {
    element.textContent = userInput; // Automatically escapes
}

function safeHTML(userInput) {
    const div = document.createElement('div');
    div.textContent = userInput;
    return div.innerHTML; // Escaped HTML
}

// Content Security Policy (CSP)
// Add to HTML head:
// <meta http-equiv="Content-Security-Policy" content="default-src 'self'; script-src 'self'">
```

**Input Validation:**
```javascript
// Validate and sanitize user input
function validateEmail(email) {
    const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return emailRegex.test(email) && email.length <= 254;
}

function sanitizeString(input) {
    return input
        .replace(/[<>]/g, '') // Remove potential HTML tags
        .trim()
        .substring(0, 1000); // Limit length
}

// SQL Injection prevention (for Node.js)
// Use parameterized queries, never string concatenation
// Bad: `SELECT * FROM users WHERE id = ${userId}`
// Good: Use prepared statements with parameters
```

**Authentication & Authorization:**
```javascript
// JWT token handling
function storeToken(token) {
    // Store in httpOnly cookie (server-side) or sessionStorage
    sessionStorage.setItem('authToken', token);
}

function getAuthHeader() {
    const token = sessionStorage.getItem('authToken');
    return token ? `Bearer ${token}` : null;
}

// Secure API calls
async function secureApiCall(url, options = {}) {
    const authHeader = getAuthHeader();

    const response = await fetch(url, {
        ...options,
        headers: {
            'Content-Type': 'application/json',
            ...(authHeader && { 'Authorization': authHeader }),
            ...options.headers
        }
    });

    if (response.status === 401) {
        // Handle unauthorized - redirect to login
        window.location.href = '/login';
        return;
    }

    return response;
}
```

### Single Sign-On (SSO)

**Implementing SSO authentication flows.**

**OAuth 2.0 Flow:**
```javascript
class OAuthClient {
    constructor(clientId, redirectUri, authUrl) {
        this.clientId = clientId;
        this.redirectUri = redirectUri;
        this.authUrl = authUrl;
    }

    // Step 1: Redirect to authorization server
    initiateLogin() {
        const state = this.generateState();
        sessionStorage.setItem('oauth_state', state);

        const params = new URLSearchParams({
            response_type: 'code',
            client_id: this.clientId,
            redirect_uri: this.redirectUri,
            scope: 'openid profile email',
            state: state
        });

        window.location.href = `${this.authUrl}?${params}`;
    }

    // Step 2: Handle callback with authorization code
    async handleCallback() {
        const urlParams = new URLSearchParams(window.location.search);
        const code = urlParams.get('code');
        const state = urlParams.get('state');
        const storedState = sessionStorage.getItem('oauth_state');

        // Verify state to prevent CSRF
        if (state !== storedState) {
            throw new Error('Invalid state parameter');
        }

        // Exchange code for tokens
        const tokens = await this.exchangeCodeForTokens(code);
        return tokens;
    }

    async exchangeCodeForTokens(code) {
        const response = await fetch('/api/oauth/token', {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({
                grant_type: 'authorization_code',
                code: code,
                redirect_uri: this.redirectUri,
                client_id: this.clientId
            })
        });

        return response.json();
    }

    generateState() {
        return Math.random().toString(36).substring(2, 15) +
               Math.random().toString(36).substring(2, 15);
    }
}

// Usage
const oauthClient = new OAuthClient(
    'your-client-id',
    'https://yourapp.com/callback',
    'https://auth.provider.com/oauth/authorize'
);

// Initiate login
document.getElementById('login-btn').addEventListener('click', () => {
    oauthClient.initiateLogin();
});

// Handle callback (on callback page)
if (window.location.pathname === '/callback') {
    oauthClient.handleCallback()
        .then(tokens => {
            // Store tokens and redirect to app
            sessionStorage.setItem('access_token', tokens.access_token);
            window.location.href = '/dashboard';
        })
        .catch(error => {
            console.error('OAuth error:', error);
        });
}
```

### File Upload Techniques

**Implementing various file upload strategies.**

**Basic File Upload:**
```javascript
// HTML: <input type="file" id="fileInput" multiple>

const fileInput = document.getElementById('fileInput');

fileInput.addEventListener('change', function(event) {
    const files = Array.from(event.target.files);

    files.forEach(file => {
        uploadFile(file);
    });
});

async function uploadFile(file) {
    const formData = new FormData();
    formData.append('file', file);

    try {
        const response = await fetch('/api/upload', {
            method: 'POST',
            body: formData
        });

        const result = await response.json();
        console.log('Upload successful:', result);
    } catch (error) {
        console.error('Upload failed:', error);
    }
}
```

**Upload with Progress:**
```javascript
function uploadWithProgress(file, onProgress) {
    return new Promise((resolve, reject) => {
        const xhr = new XMLHttpRequest();
        const formData = new FormData();
        formData.append('file', file);

        // Track upload progress
        xhr.upload.addEventListener('progress', (event) => {
            if (event.lengthComputable) {
                const percentComplete = (event.loaded / event.total) * 100;
                onProgress(percentComplete);
            }
        });

        xhr.addEventListener('load', () => {
            if (xhr.status === 200) {
                resolve(JSON.parse(xhr.responseText));
            } else {
                reject(new Error(`Upload failed: ${xhr.status}`));
            }
        });

        xhr.addEventListener('error', () => {
            reject(new Error('Upload failed'));
        });

        xhr.open('POST', '/api/upload');
        xhr.send(formData);
    });
}

// Usage
const progressBar = document.getElementById('progressBar');

uploadWithProgress(file, (progress) => {
    progressBar.style.width = `${progress}%`;
    progressBar.textContent = `${Math.round(progress)}%`;
});
```

**Chunked Upload (Large Files):**
```javascript
class ChunkedUploader {
    constructor(file, chunkSize = 1024 * 1024) { // 1MB chunks
        this.file = file;
        this.chunkSize = chunkSize;
        this.totalChunks = Math.ceil(file.size / chunkSize);
        this.uploadedChunks = 0;
    }

    async upload(onProgress) {
        const uploadId = await this.initializeUpload();

        for (let i = 0; i < this.totalChunks; i++) {
            await this.uploadChunk(uploadId, i);
            this.uploadedChunks++;

            const progress = (this.uploadedChunks / this.totalChunks) * 100;
            onProgress(progress);
        }

        return this.finalizeUpload(uploadId);
    }

    async initializeUpload() {
        const response = await fetch('/api/upload/init', {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({
                filename: this.file.name,
                filesize: this.file.size,
                totalChunks: this.totalChunks
            })
        });

        const { uploadId } = await response.json();
        return uploadId;
    }

    async uploadChunk(uploadId, chunkIndex) {
        const start = chunkIndex * this.chunkSize;
        const end = Math.min(start + this.chunkSize, this.file.size);
        const chunk = this.file.slice(start, end);

        const formData = new FormData();
        formData.append('chunk', chunk);
        formData.append('uploadId', uploadId);
        formData.append('chunkIndex', chunkIndex);

        const response = await fetch('/api/upload/chunk', {
            method: 'POST',
            body: formData
        });

        if (!response.ok) {
            throw new Error(`Chunk upload failed: ${response.status}`);
        }
    }

    async finalizeUpload(uploadId) {
        const response = await fetch('/api/upload/finalize', {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({ uploadId })
        });

        return response.json();
    }
}

// Usage
const uploader = new ChunkedUploader(largeFile);
uploader.upload((progress) => {
    console.log(`Upload progress: ${progress}%`);
});
```

### Pull-to-Refresh and Infinite Scroll

**Implementing mobile-friendly scrolling patterns.**

**Pull-to-Refresh:**
```javascript
class PullToRefresh {
    constructor(container, onRefresh) {
        this.container = container;
        this.onRefresh = onRefresh;
        this.startY = 0;
        this.currentY = 0;
        this.isRefreshing = false;
        this.threshold = 80;

        this.init();
    }

    init() {
        this.container.addEventListener('touchstart', this.handleTouchStart.bind(this));
        this.container.addEventListener('touchmove', this.handleTouchMove.bind(this));
        this.container.addEventListener('touchend', this.handleTouchEnd.bind(this));
    }

    handleTouchStart(event) {
        if (this.container.scrollTop === 0) {
            this.startY = event.touches[0].clientY;
        }
    }

    handleTouchMove(event) {
        if (this.isRefreshing || this.container.scrollTop > 0) return;

        this.currentY = event.touches[0].clientY;
        const pullDistance = this.currentY - this.startY;

        if (pullDistance > 0) {
            event.preventDefault();

            // Visual feedback
            const pullIndicator = document.getElementById('pull-indicator');
            pullIndicator.style.transform = `translateY(${Math.min(pullDistance, this.threshold)}px)`;

            if (pullDistance > this.threshold) {
                pullIndicator.textContent = 'Release to refresh';
            } else {
                pullIndicator.textContent = 'Pull to refresh';
            }
        }
    }

    async handleTouchEnd(event) {
        const pullDistance = this.currentY - this.startY;

        if (pullDistance > this.threshold && !this.isRefreshing) {
            this.isRefreshing = true;

            try {
                await this.onRefresh();
            } finally {
                this.isRefreshing = false;
                this.resetPullIndicator();
            }
        } else {
            this.resetPullIndicator();
        }
    }

    resetPullIndicator() {
        const pullIndicator = document.getElementById('pull-indicator');
        pullIndicator.style.transform = 'translateY(0)';
        pullIndicator.textContent = 'Pull to refresh';
    }
}

// Usage
const pullToRefresh = new PullToRefresh(
    document.getElementById('content'),
    async () => {
        // Refresh data
        const newData = await fetchLatestData();
        updateUI(newData);
    }
);
```

**Infinite Scroll:**
```javascript
class InfiniteScroll {
    constructor(container, loadMore, options = {}) {
        this.container = container;
        this.loadMore = loadMore;
        this.threshold = options.threshold || 100;
        this.isLoading = false;
        this.hasMore = true;

        this.init();
    }

    init() {
        this.container.addEventListener('scroll', this.handleScroll.bind(this));
    }

    async handleScroll() {
        if (this.isLoading || !this.hasMore) return;

        const { scrollTop, scrollHeight, clientHeight } = this.container;
        const distanceFromBottom = scrollHeight - scrollTop - clientHeight;

        if (distanceFromBottom < this.threshold) {
            this.isLoading = true;
            this.showLoadingIndicator();

            try {
                const result = await this.loadMore();

                if (!result || result.length === 0) {
                    this.hasMore = false;
                    this.showEndMessage();
                }
            } catch (error) {
                console.error('Failed to load more:', error);
            } finally {
                this.isLoading = false;
                this.hideLoadingIndicator();
            }
        }
    }

    showLoadingIndicator() {
        const indicator = document.getElementById('loading-indicator');
        indicator.style.display = 'block';
    }

    hideLoadingIndicator() {
        const indicator = document.getElementById('loading-indicator');
        indicator.style.display = 'none';
    }

    showEndMessage() {
        const endMessage = document.getElementById('end-message');
        endMessage.style.display = 'block';
    }

    reset() {
        this.hasMore = true;
        this.isLoading = false;
        document.getElementById('end-message').style.display = 'none';
    }
}

// Usage
let currentPage = 1;

const infiniteScroll = new InfiniteScroll(
    document.getElementById('content'),
    async () => {
        const response = await fetch(`/api/posts?page=${currentPage}`);
        const posts = await response.json();

        posts.forEach(post => {
            const postElement = createPostElement(post);
            document.getElementById('posts-container').appendChild(postElement);
        });

        currentPage++;
        return posts;
    },
    { threshold: 200 }
);
```

### Page Visibility API

**Detecting when page becomes visible or hidden.**

```javascript
// Page Visibility API
function handleVisibilityChange() {
    if (document.hidden) {
        // Page is hidden
        console.log('Page is hidden');
        pauseVideo();
        stopPolling();
    } else {
        // Page is visible
        console.log('Page is visible');
        resumeVideo();
        startPolling();
    }
}

document.addEventListener('visibilitychange', handleVisibilityChange);

// Check current visibility state
if (document.hidden) {
    console.log('Page is currently hidden');
} else {
    console.log('Page is currently visible');
}

// Practical applications
class ActivityTracker {
    constructor() {
        this.startTime = Date.now();
        this.totalTime = 0;
        this.isActive = !document.hidden;

        document.addEventListener('visibilitychange', this.handleVisibilityChange.bind(this));
    }

    handleVisibilityChange() {
        const now = Date.now();

        if (document.hidden) {
            // Page became hidden
            if (this.isActive) {
                this.totalTime += now - this.startTime;
                this.isActive = false;
            }
        } else {
            // Page became visible
            this.startTime = now;
            this.isActive = true;
        }
    }

    getTotalActiveTime() {
        let total = this.totalTime;

        if (this.isActive) {
            total += Date.now() - this.startTime;
        }

        return total;
    }
}

// Usage
const tracker = new ActivityTracker();

// Get total active time after some period
setTimeout(() => {
    console.log(`User was active for ${tracker.getTotalActiveTime()}ms`);
}, 60000);
```

### Caching Strategies

**Implementing various caching mechanisms in JavaScript.**

**Memory Cache:**
```javascript
class MemoryCache {
    constructor(maxSize = 100) {
        this.cache = new Map();
        this.maxSize = maxSize;
    }

    get(key) {
        if (this.cache.has(key)) {
            // Move to end (LRU)
            const value = this.cache.get(key);
            this.cache.delete(key);
            this.cache.set(key, value);
            return value;
        }
        return null;
    }

    set(key, value) {
        if (this.cache.has(key)) {
            this.cache.delete(key);
        } else if (this.cache.size >= this.maxSize) {
            // Remove oldest entry
            const firstKey = this.cache.keys().next().value;
            this.cache.delete(firstKey);
        }

        this.cache.set(key, value);
    }

    clear() {
        this.cache.clear();
    }

    size() {
        return this.cache.size;
    }
}
```

**LocalStorage Cache with Expiration:**
```javascript
class LocalStorageCache {
    constructor(prefix = 'cache_') {
        this.prefix = prefix;
    }

    set(key, value, ttl = 3600000) { // Default 1 hour
        const item = {
            value: value,
            expiry: Date.now() + ttl
        };

        try {
            localStorage.setItem(this.prefix + key, JSON.stringify(item));
        } catch (error) {
            console.warn('LocalStorage cache set failed:', error);
        }
    }

    get(key) {
        try {
            const itemStr = localStorage.getItem(this.prefix + key);

            if (!itemStr) return null;

            const item = JSON.parse(itemStr);

            if (Date.now() > item.expiry) {
                localStorage.removeItem(this.prefix + key);
                return null;
            }

            return item.value;
        } catch (error) {
            console.warn('LocalStorage cache get failed:', error);
            return null;
        }
    }

    remove(key) {
        localStorage.removeItem(this.prefix + key);
    }

    clear() {
        const keys = Object.keys(localStorage);
        keys.forEach(key => {
            if (key.startsWith(this.prefix)) {
                localStorage.removeItem(key);
            }
        });
    }

    // Clean expired entries
    cleanup() {
        const keys = Object.keys(localStorage);
        keys.forEach(key => {
            if (key.startsWith(this.prefix)) {
                this.get(key.substring(this.prefix.length)); // Will remove if expired
            }
        });
    }
}

// Usage
const cache = new LocalStorageCache('myapp_');

// Cache API response
async function fetchUserData(userId) {
    const cacheKey = `user_${userId}`;
    let userData = cache.get(cacheKey);

    if (!userData) {
        const response = await fetch(`/api/users/${userId}`);
        userData = await response.json();
        cache.set(cacheKey, userData, 300000); // Cache for 5 minutes
    }

    return userData;
}
```

---

## React

### React Fundamentals

**React is a JavaScript library for building user interfaces with a component-based architecture.**

**Core Concepts:**
```javascript
// Component-based architecture
function Welcome(props) {
    return <h1>Hello, {props.name}!</h1>;
}

// JSX syntax
const element = <h1>Hello, world!</h1>;

// Props (read-only)
function Button({ onClick, children, disabled = false }) {
    return (
        <button onClick={onClick} disabled={disabled}>
            {children}
        </button>
    );
}

// State management
function Counter() {
    const [count, setCount] = useState(0);

    return (
        <div>
            <p>Count: {count}</p>
            <button onClick={() => setCount(count + 1)}>
                Increment
            </button>
        </div>
    );
}
```

**React Philosophy:**
- **Declarative:** Describe what the UI should look like
- **Component-based:** Encapsulated components manage their own state
- **Learn once, write anywhere:** React Native, React VR, etc.

### JSX to DOM

**JSX is syntactic sugar that gets transpiled to React.createElement calls.**

**JSX Transformation:**
```javascript
// JSX
const element = (
    <div className="container">
        <h1>Hello, {name}!</h1>
        <p>Welcome to React</p>
    </div>
);

// Transpiled to:
const element = React.createElement(
    'div',
    { className: 'container' },
    React.createElement('h1', null, 'Hello, ', name, '!'),
    React.createElement('p', null, 'Welcome to React')
);

// React Element (Virtual DOM)
const element = {
    type: 'div',
    props: {
        className: 'container',
        children: [
            {
                type: 'h1',
                props: { children: ['Hello, ', name, '!'] }
            },
            {
                type: 'p',
                props: { children: 'Welcome to React' }
            }
        ]
    }
};
```

**JSX Rules:**
```javascript
// Must return single parent element
function Component() {
    return (
        <div>
            <h1>Title</h1>
            <p>Content</p>
        </div>
    );
}

// Or use React Fragment
function Component() {
    return (
        <>
            <h1>Title</h1>
            <p>Content</p>
        </>
    );
}

// JavaScript expressions in curly braces
function Greeting({ user }) {
    return (
        <div>
            <h1>Hello, {user.name}!</h1>
            <p>You have {user.messages.length} messages</p>
            {user.isAdmin && <button>Admin Panel</button>}
        </div>
    );
}

// Event handlers
function Button() {
    const handleClick = (event) => {
        event.preventDefault();
        console.log('Button clicked');
    };

    return <button onClick={handleClick}>Click me</button>;
}
```

### Virtual DOM vs Real DOM

**Virtual DOM is a JavaScript representation of the actual DOM for performance optimization.**

**Real DOM Problems:**
```javascript
// Expensive DOM operations
document.getElementById('list').innerHTML = ''; // Reflow/repaint
for (let i = 0; i < 1000; i++) {
    const li = document.createElement('li');
    li.textContent = `Item ${i}`;
    document.getElementById('list').appendChild(li); // Multiple reflows
}
```

**Virtual DOM Solution:**
```javascript
// Virtual DOM representation
const virtualDOM = {
    type: 'ul',
    props: {
        id: 'list',
        children: [
            { type: 'li', props: { children: 'Item 1' } },
            { type: 'li', props: { children: 'Item 2' } },
            // ... more items
        ]
    }
};

// React's reconciliation process:
// 1. Create new Virtual DOM tree
// 2. Compare with previous Virtual DOM tree (diffing)
// 3. Calculate minimal changes needed
// 4. Apply only necessary changes to real DOM
```

**Benefits:**
- **Performance:** Batched updates, minimal DOM manipulation
- **Predictability:** Declarative programming model
- **Cross-browser:** Consistent behavior across browsers
- **Developer Experience:** Easier debugging and testing

**Reconciliation Algorithm:**
```javascript
// React's diffing heuristics:

// 1. Different element types = complete rebuild
// Old: <div><Counter /></div>
// New: <span><Counter /></span>
// Result: Unmount div and Counter, mount new span and Counter

// 2. Same element type = update props
// Old: <div className="old" title="Old" />
// New: <div className="new" title="New" />
// Result: Update className and title attributes

// 3. Component elements = update props and re-render
// Old: <Counter count={1} />
// New: <Counter count={2} />
// Result: Update props and re-render Counter component
```

### Component Types (Class vs Function)

**React supports both class and function components, with hooks making function components more powerful.**

**Class Components:**
```javascript
class ClassComponent extends React.Component {
    constructor(props) {
        super(props);
        this.state = {
            count: 0,
            name: props.initialName || ''
        };

        // Bind methods
        this.handleClick = this.handleClick.bind(this);
    }

    // Lifecycle methods
    componentDidMount() {
        console.log('Component mounted');
        this.fetchData();
    }

    componentDidUpdate(prevProps, prevState) {
        if (prevState.count !== this.state.count) {
            console.log('Count updated');
        }
    }

    componentWillUnmount() {
        console.log('Component will unmount');
        this.cleanup();
    }

    // Event handlers
    handleClick() {
        this.setState(prevState => ({
            count: prevState.count + 1
        }));
    }

    fetchData = async () => {
        try {
            const response = await fetch('/api/data');
            const data = await response.json();
            this.setState({ data });
        } catch (error) {
            this.setState({ error: error.message });
        }
    }

    render() {
        const { count, name, data, error } = this.state;

        if (error) {
            return <div>Error: {error}</div>;
        }

        return (
            <div>
                <h1>Hello, {name}!</h1>
                <p>Count: {count}</p>
                <button onClick={this.handleClick}>
                    Increment
                </button>
                {data && <DataDisplay data={data} />}
            </div>
        );
    }
}
```

**Function Components with Hooks:**
```javascript
function FunctionComponent({ initialName = '' }) {
    const [count, setCount] = useState(0);
    const [name, setName] = useState(initialName);
    const [data, setData] = useState(null);
    const [error, setError] = useState(null);

    // Equivalent to componentDidMount and componentDidUpdate
    useEffect(() => {
        console.log('Component mounted or count updated');
    }, [count]);

    // Equivalent to componentDidMount only
    useEffect(() => {
        console.log('Component mounted');
        fetchData();

        // Equivalent to componentWillUnmount
        return () => {
            console.log('Component will unmount');
            cleanup();
        };
    }, []);

    const fetchData = useCallback(async () => {
        try {
            const response = await fetch('/api/data');
            const data = await response.json();
            setData(data);
        } catch (error) {
            setError(error.message);
        }
    }, []);

    const handleClick = useCallback(() => {
        setCount(prevCount => prevCount + 1);
    }, []);

    if (error) {
        return <div>Error: {error}</div>;
    }

    return (
        <div>
            <h1>Hello, {name}!</h1>
            <p>Count: {count}</p>
            <button onClick={handleClick}>
                Increment
            </button>
            {data && <DataDisplay data={data} />}
        </div>
    );
}
```

**Comparison:**

| Aspect | Class Components | Function Components |
|--------|------------------|-------------------|
| Syntax | More verbose | Cleaner, concise |
| State | this.state | useState hook |
| Lifecycle | Lifecycle methods | useEffect hook |
| Performance | Can use PureComponent | React.memo + hooks |
| this binding | Required | Not needed |
| Code reuse | HOCs, render props | Custom hooks |
| Learning curve | Steeper | Easier |

### React Hooks

**Hooks enable state and lifecycle features in functional components.**

**useState:**
```javascript
function Counter() {
    const [count, setCount] = useState(0);

    // Multiple state variables
    const [name, setName] = useState('');
    const [user, setUser] = useState({ id: null, email: '' });

    // Functional updates
    const increment = () => {
        setCount(prevCount => prevCount + 1);
    };

    // Object state updates
    const updateUser = (field, value) => {
        setUser(prevUser => ({
            ...prevUser,
            [field]: value
        }));
    };

    return (
        <div>
            <p>Count: {count}</p>
            <button onClick={increment}>+</button>

            <input
                value={name}
                onChange={(e) => setName(e.target.value)}
                placeholder="Name"
            />

            <input
                value={user.email}
                onChange={(e) => updateUser('email', e.target.value)}
                placeholder="Email"
            />
        </div>
    );
}
```

**useEffect:**
```javascript
function DataComponent({ userId }) {
    const [data, setData] = useState(null);
    const [loading, setLoading] = useState(true);

    // Effect with dependencies
    useEffect(() => {
        let cancelled = false;

        async function fetchData() {
            setLoading(true);
            try {
                const response = await fetch(`/api/users/${userId}`);
                const userData = await response.json();

                if (!cancelled) {
                    setData(userData);
                }
            } catch (error) {
                if (!cancelled) {
                    console.error('Fetch error:', error);
                }
            } finally {
                if (!cancelled) {
                    setLoading(false);
                }
            }
        }

        fetchData();

        // Cleanup function
        return () => {
            cancelled = true;
        };
    }, [userId]); // Re-run when userId changes

    // Effect for subscriptions
    useEffect(() => {
        const subscription = subscribeToUserUpdates(userId, (update) => {
            setData(prevData => ({ ...prevData, ...update }));
        });

        return () => {
            subscription.unsubscribe();
        };
    }, [userId]);

    if (loading) return <div>Loading...</div>;

    return <div>{data ? data.name : 'No data'}</div>;
}
```

**Custom Hooks:**
```javascript
// Custom hook for API calls
function useApi(url) {
    const [data, setData] = useState(null);
    const [loading, setLoading] = useState(true);
    const [error, setError] = useState(null);

    useEffect(() => {
        let cancelled = false;

        async function fetchData() {
            try {
                setLoading(true);
                setError(null);

                const response = await fetch(url);
                if (!response.ok) {
                    throw new Error(`HTTP ${response.status}`);
                }

                const result = await response.json();

                if (!cancelled) {
                    setData(result);
                }
            } catch (err) {
                if (!cancelled) {
                    setError(err.message);
                }
            } finally {
                if (!cancelled) {
                    setLoading(false);
                }
            }
        }

        fetchData();

        return () => {
            cancelled = true;
        };
    }, [url]);

    return { data, loading, error };
}

// Custom hook for local storage
function useLocalStorage(key, initialValue) {
    const [storedValue, setStoredValue] = useState(() => {
        try {
            const item = window.localStorage.getItem(key);
            return item ? JSON.parse(item) : initialValue;
        } catch (error) {
            console.error('Error reading localStorage:', error);
            return initialValue;
        }
    });

    const setValue = (value) => {
        try {
            const valueToStore = value instanceof Function ? value(storedValue) : value;
            setStoredValue(valueToStore);
            window.localStorage.setItem(key, JSON.stringify(valueToStore));
        } catch (error) {
            console.error('Error setting localStorage:', error);
        }
    };

    return [storedValue, setValue];
}

// Usage
function App() {
    const { data: users, loading, error } = useApi('/api/users');
    const [theme, setTheme] = useLocalStorage('theme', 'light');

    if (loading) return <div>Loading...</div>;
    if (error) return <div>Error: {error}</div>;

    return (
        <div className={`app theme-${theme}`}>
            <button onClick={() => setTheme(theme === 'light' ? 'dark' : 'light')}>
                Toggle Theme
            </button>
            {users?.map(user => <UserCard key={user.id} user={user} />)}
        </div>
    );
}
```

### Component Lifecycle

**Understanding React component lifecycle phases and their corresponding hooks.**

**Class Component Lifecycle:**
```javascript
class LifecycleExample extends React.Component {
    constructor(props) {
        super(props);
        this.state = { count: 0 };
        console.log('1. Constructor');
    }

    static getDerivedStateFromProps(props, state) {
        console.log('2. getDerivedStateFromProps');
        // Return new state or null
        return null;
    }

    componentDidMount() {
        console.log('3. componentDidMount');
        // API calls, subscriptions, timers
        this.timer = setInterval(() => {
            this.setState(prev => ({ count: prev.count + 1 }));
        }, 1000);
    }

    shouldComponentUpdate(nextProps, nextState) {
        console.log('4. shouldComponentUpdate');
        // Return true/false to control re-rendering
        return nextState.count !== this.state.count;
    }

    getSnapshotBeforeUpdate(prevProps, prevState) {
        console.log('5. getSnapshotBeforeUpdate');
        // Capture info before DOM update (scroll position, etc.)
        return null;
    }

    componentDidUpdate(prevProps, prevState, snapshot) {
        console.log('6. componentDidUpdate');
        // DOM updates, API calls based on prop/state changes
        if (prevState.count !== this.state.count) {
            document.title = `Count: ${this.state.count}`;
        }
    }

    componentWillUnmount() {
        console.log('7. componentWillUnmount');
        // Cleanup: clear timers, cancel requests, unsubscribe
        clearInterval(this.timer);
    }

    componentDidCatch(error, errorInfo) {
        console.log('8. componentDidCatch');
        // Error boundary
        this.setState({ hasError: true });
    }

    render() {
        console.log('Render');
        return <div>Count: {this.state.count}</div>;
    }
}
```

**Hooks Equivalent:**
```javascript
function LifecycleHooks() {
    const [count, setCount] = useState(0);
    const [hasError, setHasError] = useState(false);

    // componentDidMount
    useEffect(() => {
        console.log('Component mounted');

        const timer = setInterval(() => {
            setCount(prev => prev + 1);
        }, 1000);

        // componentWillUnmount
        return () => {
            console.log('Component will unmount');
            clearInterval(timer);
        };
    }, []); // Empty dependency array = mount/unmount only

    // componentDidUpdate (for count changes)
    useEffect(() => {
        console.log('Count updated');
        document.title = `Count: ${count}`;
    }, [count]); // Runs when count changes

    // getDerivedStateFromProps equivalent
    useEffect(() => {
        // Update state based on props
    }, [/* props */]);

    // Error boundary (requires class component or error boundary library)

    return <div>Count: {count}</div>;
}
```

**Lifecycle Phases:**

1. **Mounting:**
   - constructor → getDerivedStateFromProps → render → componentDidMount

2. **Updating:**
   - getDerivedStateFromProps → shouldComponentUpdate → render → getSnapshotBeforeUpdate → componentDidUpdate

3. **Unmounting:**
   - componentWillUnmount

4. **Error Handling:**
   - componentDidCatch

### React Hooks

**Hooks enable state and lifecycle features in functional components.**

**useState:**
```js
const [count, setCount] = useState(0);
// Equivalent to class component state management
```

**useEffect:**
```js
useEffect(() => {
    document.title = `Count: ${count}`;
    
    // Cleanup function (componentWillUnmount equivalent)
    return () => {
        // cleanup code
    };
}, [count]); // Dependency array
```

**Key Benefits:**
- Eliminates `this` binding complexity
- Better code reuse through custom hooks
- Simplified component logic organization
- Functional programming approach

**Custom Hook Example:**
```js
function useCounter(initialValue = 0) {
    const [count, setCount] = useState(initialValue);
    
    const increment = () => setCount(count + 1);
    const decrement = () => setCount(count - 1);
    
    return { count, increment, decrement };
}
```

### Performance Optimization

**React provides several tools for optimizing component performance.**

**React.memo:**
```javascript
// Prevents re-renders when props haven't changed
const ExpensiveComponent = React.memo(function ExpensiveComponent({ data, onUpdate }) {
    console.log('ExpensiveComponent rendered');

    return (
        <div>
            {data.map(item => (
                <div key={item.id} onClick={() => onUpdate(item.id)}>
                    {item.name}
                </div>
            ))}
        </div>
    );
});

// Custom comparison function
const SmartComponent = React.memo(function SmartComponent({ user, settings }) {
    return <div>{user.name} - {settings.theme}</div>;
}, (prevProps, nextProps) => {
    // Return true if props are equal (skip re-render)
    return prevProps.user.id === nextProps.user.id &&
           prevProps.settings.theme === nextProps.settings.theme;
});
```

**useMemo:**
```javascript
function ExpensiveCalculation({ items, filter }) {
    // Expensive calculation only runs when dependencies change
    const filteredItems = useMemo(() => {
        console.log('Filtering items...');
        return items.filter(item =>
            item.name.toLowerCase().includes(filter.toLowerCase())
        ).sort((a, b) => a.name.localeCompare(b.name));
    }, [items, filter]);

    // Expensive object creation
    const chartData = useMemo(() => {
        console.log('Generating chart data...');
        return {
            labels: filteredItems.map(item => item.name),
            datasets: [{
                data: filteredItems.map(item => item.value),
                backgroundColor: filteredItems.map(item => item.color)
            }]
        };
    }, [filteredItems]);

    return (
        <div>
            <ItemList items={filteredItems} />
            <Chart data={chartData} />
        </div>
    );
}
```

**useCallback:**
```javascript
function ParentComponent({ items }) {
    const [filter, setFilter] = useState('');
    const [sortOrder, setSortOrder] = useState('asc');

    // Without useCallback, this function is recreated on every render
    // causing child components to re-render unnecessarily
    const handleItemClick = useCallback((itemId) => {
        console.log('Item clicked:', itemId);
        // Handle item click
    }, []); // No dependencies, function never changes

    const handleItemUpdate = useCallback((itemId, newData) => {
        setItems(prevItems =>
            prevItems.map(item =>
                item.id === itemId ? { ...item, ...newData } : item
            )
        );
    }, []); // setItems is stable, so no dependencies needed

    const sortedItems = useMemo(() => {
        return [...items].sort((a, b) => {
            const result = a.name.localeCompare(b.name);
            return sortOrder === 'asc' ? result : -result;
        });
    }, [items, sortOrder]);

    return (
        <div>
            <input
                value={filter}
                onChange={(e) => setFilter(e.target.value)}
                placeholder="Filter items..."
            />

            <button onClick={() => setSortOrder(prev => prev === 'asc' ? 'desc' : 'asc')}>
                Sort {sortOrder === 'asc' ? 'Descending' : 'Ascending'}
            </button>

            {sortedItems.map(item => (
                <ItemComponent
                    key={item.id}
                    item={item}
                    onClick={handleItemClick}
                    onUpdate={handleItemUpdate}
                />
            ))}
        </div>
    );
}

// Child component wrapped with React.memo
const ItemComponent = React.memo(function ItemComponent({ item, onClick, onUpdate }) {
    console.log(`Rendering item ${item.id}`);

    return (
        <div onClick={() => onClick(item.id)}>
            <h3>{item.name}</h3>
            <p>{item.description}</p>
            <button onClick={() => onUpdate(item.id, { viewed: true })}>
                Mark as Viewed
            </button>
        </div>
    );
});
```

**useRef:**
```javascript
function RefExamples() {
    const inputRef = useRef(null);
    const countRef = useRef(0);
    const timerRef = useRef(null);

    // DOM reference
    const focusInput = () => {
        inputRef.current.focus();
    };

    // Mutable value that doesn't trigger re-renders
    const incrementCount = () => {
        countRef.current += 1;
        console.log('Count:', countRef.current);
        // Component doesn't re-render when countRef changes
    };

    // Store timer reference for cleanup
    const startTimer = () => {
        if (timerRef.current) {
            clearInterval(timerRef.current);
        }

        timerRef.current = setInterval(() => {
            console.log('Timer tick');
        }, 1000);
    };

    const stopTimer = () => {
        if (timerRef.current) {
            clearInterval(timerRef.current);
            timerRef.current = null;
        }
    };

    useEffect(() => {
        // Cleanup timer on unmount
        return () => {
            if (timerRef.current) {
                clearInterval(timerRef.current);
            }
        };
    }, []);

    return (
        <div>
            <input ref={inputRef} placeholder="Focus me" />
            <button onClick={focusInput}>Focus Input</button>

            <button onClick={incrementCount}>Increment Count</button>
            <button onClick={startTimer}>Start Timer</button>
            <button onClick={stopTimer}>Stop Timer</button>
        </div>
    );
}
```

**Performance Best Practices:**
```javascript
// 1. Avoid creating objects/functions in render
function BadComponent({ items }) {
    return (
        <div>
            {items.map(item => (
                <ItemComponent
                    key={item.id}
                    item={item}
                    style={{ color: 'red' }} // ❌ New object every render
                    onClick={() => console.log(item.id)} // ❌ New function every render
                />
            ))}
        </div>
    );
}

function GoodComponent({ items }) {
    const itemStyle = useMemo(() => ({ color: 'red' }), []);
    const handleClick = useCallback((itemId) => {
        console.log(itemId);
    }, []);

    return (
        <div>
            {items.map(item => (
                <ItemComponent
                    key={item.id}
                    item={item}
                    style={itemStyle} // ✅ Stable reference
                    onClick={handleClick} // ✅ Stable function
                />
            ))}
        </div>
    );
}

// 2. Use proper keys for lists
function ListComponent({ items }) {
    return (
        <ul>
            {items.map((item, index) => (
                // ❌ Using index as key can cause issues
                <li key={index}>{item.name}</li>
            ))}
        </ul>
    );
}

function BetterListComponent({ items }) {
    return (
        <ul>
            {items.map(item => (
                // ✅ Using stable, unique identifier
                <li key={item.id}>{item.name}</li>
            ))}
        </ul>
    );
}
```

### State vs Props

**Understanding the difference between state and props in React.**

**Props (Properties):**
```javascript
// Props are read-only data passed from parent to child
function ChildComponent({ name, age, onUpdate, children }) {
    // Props cannot be modified directly
    // name = "New Name"; // ❌ This would cause an error

    return (
        <div>
            <h2>{name}</h2>
            <p>Age: {age}</p>
            <button onClick={() => onUpdate(name)}>
                Update Parent
            </button>
            {children}
        </div>
    );
}

function ParentComponent() {
    const [users, setUsers] = useState([
        { id: 1, name: 'John', age: 25 },
        { id: 2, name: 'Jane', age: 30 }
    ]);

    const handleUpdate = (name) => {
        console.log(`Update requested for ${name}`);
    };

    return (
        <div>
            {users.map(user => (
                <ChildComponent
                    key={user.id}
                    name={user.name}
                    age={user.age}
                    onUpdate={handleUpdate}
                >
                    <p>Additional content</p>
                </ChildComponent>
            ))}
        </div>
    );
}
```

**Key Differences:**

| Aspect | Props | State |
|--------|-------|-------|
| **Mutability** | Immutable (read-only) | Mutable (via setState) |
| **Source** | Passed from parent | Internal to component |
| **Purpose** | Configure component | Track changing data |
| **Triggers re-render** | When parent re-renders | When state changes |
| **Access** | this.props / function params | this.state / useState |

### Component Communication

**Different patterns for components to communicate with each other.**

**Parent to Child (Props):**
```javascript
function Parent() {
    const [message, setMessage] = useState("Hello from parent");

    return (
        <Child
            message={message}
            onMessageChange={setMessage}
        />
    );
}

function Child({ message, onMessageChange }) {
    return (
        <div>
            <p>{message}</p>
            <button onClick={() => onMessageChange("Updated message")}>
                Update Message
            </button>
        </div>
    );
}
```

**Child to Parent (Callback Props):**
```javascript
function Parent() {
    const [data, setData] = useState([]);

    const handleDataFromChild = (newData) => {
        setData(prevData => [...prevData, newData]);
    };

    return (
        <div>
            <Child onDataSubmit={handleDataFromChild} />
            <DataDisplay data={data} />
        </div>
    );
}

function Child({ onDataSubmit }) {
    const [input, setInput] = useState('');

    const handleSubmit = (e) => {
        e.preventDefault();
        onDataSubmit(input);
        setInput('');
    };

    return (
        <form onSubmit={handleSubmit}>
            <input
                value={input}
                onChange={(e) => setInput(e.target.value)}
            />
            <button type="submit">Submit</button>
        </form>
    );
}
```

**Sibling Communication (Lift State Up):**
```javascript
function Parent() {
    const [selectedItem, setSelectedItem] = useState(null);

    return (
        <div>
            <ItemList onItemSelect={setSelectedItem} />
            <ItemDetails item={selectedItem} />
        </div>
    );
}

function ItemList({ onItemSelect }) {
    const items = ['Item 1', 'Item 2', 'Item 3'];

    return (
        <ul>
            {items.map(item => (
                <li key={item} onClick={() => onItemSelect(item)}>
                    {item}
                </li>
            ))}
        </ul>
    );
}

function ItemDetails({ item }) {
    return (
        <div>
            {item ? `Selected: ${item}` : 'No item selected'}
        </div>
    );
}
```

**Context API (Deep Component Tree):**
```javascript
const ThemeContext = createContext();
const UserContext = createContext();

function App() {
    const [theme, setTheme] = useState('light');
    const [user, setUser] = useState(null);

    return (
        <ThemeContext.Provider value={{ theme, setTheme }}>
            <UserContext.Provider value={{ user, setUser }}>
                <Header />
                <Main />
                <Footer />
            </UserContext.Provider>
        </ThemeContext.Provider>
    );
}

function Header() {
    const { theme, setTheme } = useContext(ThemeContext);
    const { user } = useContext(UserContext);

    return (
        <header className={`header-${theme}`}>
            <h1>Welcome {user?.name || 'Guest'}</h1>
            <button onClick={() => setTheme(theme === 'light' ? 'dark' : 'light')}>
                Toggle Theme
            </button>
        </header>
    );
}
```

### Controlled vs Uncontrolled Components

**Two approaches to handling form inputs in React.**

**Controlled Components:**
```javascript
function ControlledForm() {
    const [formData, setFormData] = useState({
        name: '',
        email: '',
        message: ''
    });

    const handleChange = (e) => {
        const { name, value } = e.target;
        setFormData(prev => ({
            ...prev,
            [name]: value
        }));
    };

    const handleSubmit = (e) => {
        e.preventDefault();
        console.log('Form data:', formData);
    };

    return (
        <form onSubmit={handleSubmit}>
            <input
                type="text"
                name="name"
                value={formData.name}
                onChange={handleChange}
                placeholder="Name"
            />
            <input
                type="email"
                name="email"
                value={formData.email}
                onChange={handleChange}
                placeholder="Email"
            />
            <textarea
                name="message"
                value={formData.message}
                onChange={handleChange}
                placeholder="Message"
            />
            <button type="submit">Submit</button>
        </form>
    );
}
```

**Uncontrolled Components:**
```javascript
function UncontrolledForm() {
    const nameRef = useRef();
    const emailRef = useRef();
    const messageRef = useRef();

    const handleSubmit = (e) => {
        e.preventDefault();

        const formData = {
            name: nameRef.current.value,
            email: emailRef.current.value,
            message: messageRef.current.value
        };

        console.log('Form data:', formData);
    };

    return (
        <form onSubmit={handleSubmit}>
            <input
                type="text"
                ref={nameRef}
                defaultValue=""
                placeholder="Name"
            />
            <input
                type="email"
                ref={emailRef}
                defaultValue=""
                placeholder="Email"
            />
            <textarea
                ref={messageRef}
                defaultValue=""
                placeholder="Message"
            />
            <button type="submit">Submit</button>
        </form>
    );
}
```

**When to Use Each:**

| Aspect | Controlled | Uncontrolled |
|--------|------------|--------------|
| **Data flow** | React state controls value | DOM controls value |
| **Validation** | Real-time validation | Validation on submit |
| **Performance** | Re-renders on every change | No re-renders |
| **Testing** | Easier to test | Harder to test |
| **Use case** | Complex forms, validation | Simple forms, performance critical |

### React Keys

**Keys help React identify which items have changed, been added, or removed.**

**Why Keys Matter:**
```javascript
// Without proper keys - React can't efficiently update
function BadList({ items }) {
    return (
        <ul>
            {items.map((item, index) => (
                <li key={index}> {/* ❌ Using index as key */}
                    <input type="text" defaultValue={item.name} />
                    <button onClick={() => deleteItem(item.id)}>Delete</button>
                </li>
            ))}
        </ul>
    );
}

// With proper keys - React can efficiently update
function GoodList({ items }) {
    return (
        <ul>
            {items.map(item => (
                <li key={item.id}> {/* ✅ Using unique, stable ID */}
                    <input type="text" defaultValue={item.name} />
                    <button onClick={() => deleteItem(item.id)}>Delete</button>
                </li>
            ))}
        </ul>
    );
}
```

**Key Rules:**
```javascript
// ✅ Good key examples
<div key={user.id}>           // Unique ID
<div key={`${user.id}-${user.email}`}> // Composite key
<div key={item.slug}>         // Unique slug

// ❌ Bad key examples
<div key={Math.random()}>     // Random (changes every render)
<div key={index}>             // Array index (not stable)
<div key={item.name}>         // Non-unique value
```

**Dynamic Lists:**
```javascript
function TodoList() {
    const [todos, setTodos] = useState([
        { id: 1, text: 'Learn React', completed: false },
        { id: 2, text: 'Build an app', completed: false }
    ]);

    const addTodo = (text) => {
        const newTodo = {
            id: Date.now(), // Simple ID generation
            text,
            completed: false
        };
        setTodos(prev => [...prev, newTodo]);
    };

    const toggleTodo = (id) => {
        setTodos(prev =>
            prev.map(todo =>
                todo.id === id
                    ? { ...todo, completed: !todo.completed }
                    : todo
            )
        );
    };

    return (
        <div>
            {todos.map(todo => (
                <TodoItem
                    key={todo.id} // ✅ Stable, unique key
                    todo={todo}
                    onToggle={toggleTodo}
                />
            ))}
        </div>
    );
}
```

### React Refs

**Refs provide access to DOM elements or component instances.**

**useRef Hook:**
```javascript
function RefExamples() {
    const inputRef = useRef(null);
    const videoRef = useRef(null);
    const countRef = useRef(0);

    // Focus input
    const focusInput = () => {
        inputRef.current.focus();
    };

    // Control video
    const playVideo = () => {
        videoRef.current.play();
    };

    const pauseVideo = () => {
        videoRef.current.pause();
    };

    // Mutable value (doesn't trigger re-render)
    const incrementCount = () => {
        countRef.current += 1;
        console.log('Count:', countRef.current);
    };

    return (
        <div>
            <input ref={inputRef} placeholder="Focus me" />
            <button onClick={focusInput}>Focus Input</button>

            <video ref={videoRef} src="video.mp4" />
            <button onClick={playVideo}>Play</button>
            <button onClick={pauseVideo}>Pause</button>

            <button onClick={incrementCount}>Increment Count</button>
        </div>
    );
}
```

**Forwarding Refs:**
```javascript
// Forward ref to allow parent access to child's DOM
const FancyInput = forwardRef((props, ref) => (
    <div className="fancy-input">
        <input ref={ref} {...props} />
    </div>
));

function Parent() {
    const inputRef = useRef();

    return (
        <div>
            <FancyInput ref={inputRef} placeholder="Type here" />
            <button onClick={() => inputRef.current.focus()}>
                Focus Input
            </button>
        </div>
    );
}
```

### Event Binding

**Different ways to bind event handlers in React.**

**Function Components:**
```javascript
function EventBindingFunction() {
    const [count, setCount] = useState(0);

    // Method 1: useCallback for optimization
    const handleClick = useCallback(() => {
        setCount(prev => prev + 1);
    }, []);

    // Method 2: Regular function (recreated on each render)
    const handleClick2 = () => {
        setCount(prev => prev + 1);
    };

    return (
        <div>
            <p>Count: {count}</p>

            <button onClick={handleClick}>
                Optimized Click
            </button>

            <button onClick={handleClick2}>
                Regular Click
            </button>

            <button onClick={() => setCount(prev => prev + 1)}>
                Inline Click
            </button>
        </div>
    );
}
```

### SyntheticEvent

**React's cross-browser event wrapper.**

**SyntheticEvent Properties:**
```javascript
function EventExample() {
    const handleEvent = (event) => {
        // SyntheticEvent properties
        console.log('Event type:', event.type);
        console.log('Target element:', event.target);
        console.log('Current target:', event.currentTarget);

        // Prevent default behavior
        event.preventDefault();

        // Stop event propagation
        event.stopPropagation();

        // Mouse events
        if (event.type === 'click') {
            console.log('Mouse position:', event.clientX, event.clientY);
            console.log('Modifier keys:', {
                ctrl: event.ctrlKey,
                shift: event.shiftKey,
                alt: event.altKey
            });
        }

        // Keyboard events
        if (event.type === 'keydown') {
            console.log('Key pressed:', event.key);
            console.log('Key code:', event.keyCode);
        }
    };

    return (
        <div>
            <button onClick={handleEvent}>Click me</button>
            <input onChange={handleEvent} onKeyDown={handleEvent} />
        </div>
    );
}
```

### Higher Order Components (HOC)

**HOCs are functions that take a component and return a new component.**

**Basic HOC Pattern:**
```javascript
// HOC that adds loading functionality
function withLoading(WrappedComponent) {
    return function WithLoadingComponent(props) {
        if (props.isLoading) {
            return <div>Loading...</div>;
        }

        return <WrappedComponent {...props} />;
    };
}

// Usage
const UserList = ({ users }) => (
    <ul>
        {users.map(user => (
            <li key={user.id}>{user.name}</li>
        ))}
    </ul>
);

const UserListWithLoading = withLoading(UserList);
```

**Authentication HOC:**
```javascript
function withAuth(WrappedComponent) {
    return function WithAuthComponent(props) {
        const { user, isAuthenticated } = useAuth();

        if (!isAuthenticated) {
            return <LoginForm />;
        }

        return <WrappedComponent {...props} user={user} />;
    };
}
```

### Render Props

**Render props is a pattern for sharing code between components using a prop whose value is a function.**

**Basic Render Props:**
```javascript
class MouseTracker extends React.Component {
    state = { x: 0, y: 0 };

    handleMouseMove = (event) => {
        this.setState({
            x: event.clientX,
            y: event.clientY
        });
    };

    render() {
        return (
            <div onMouseMove={this.handleMouseMove}>
                {this.props.render(this.state)}
            </div>
        );
    }
}

// Usage
function App() {
    return (
        <MouseTracker
            render={({ x, y }) => (
                <h1>Mouse position: ({x}, {y})</h1>
            )}
        />
    );
}
```

**Function as Children:**
```javascript
class DataFetcher extends React.Component {
    state = { data: null, loading: true, error: null };

    componentDidMount() {
        fetch(this.props.url)
            .then(response => response.json())
            .then(data => this.setState({ data, loading: false }))
            .catch(error => this.setState({ error, loading: false }));
    }

    render() {
        return this.props.children(this.state);
    }
}

// Usage
function UserProfile({ userId }) {
    return (
        <DataFetcher url={`/api/users/${userId}`}>
            {({ data, loading, error }) => {
                if (loading) return <div>Loading...</div>;
                if (error) return <div>Error: {error.message}</div>;
                return <div>Hello, {data.name}!</div>;
            }}
        </DataFetcher>
    );
}
```

**Modern Hook Alternative:**
```javascript
// Custom hook replaces render props pattern
function useMousePosition() {
    const [position, setPosition] = useState({ x: 0, y: 0 });

    useEffect(() => {
        const handleMouseMove = (event) => {
            setPosition({ x: event.clientX, y: event.clientY });
        };

        window.addEventListener('mousemove', handleMouseMove);
        return () => window.removeEventListener('mousemove', handleMouseMove);
    }, []);

    return position;
}

// Usage
function App() {
    const { x, y } = useMousePosition();
    return <h1>Mouse position: ({x}, {y})</h1>;
}
```

### React Fiber

**React Fiber is the new reconciliation algorithm in React 16+.**

**Key Concepts:**
```javascript
// Fiber enables:
// 1. Incremental rendering - work can be split into chunks
// 2. Ability to pause, abort, or reuse work
// 3. Priority assignment to different types of updates
// 4. Concurrent features

// Priority levels (simplified)
const priorities = {
    Immediate: 1,     // User input, animations
    UserBlocking: 2,  // User interactions
    Normal: 3,        // Network responses
    Low: 4,           // Analytics, logging
    Idle: 5           // Background tasks
};

// Time slicing example
function heavyComponent() {
    // Before Fiber: would block the main thread
    const items = [];
    for (let i = 0; i < 10000; i++) {
        items.push(<Item key={i} data={complexCalculation(i)} />);
    }
    return <div>{items}</div>;
}

// With Fiber: work is split into chunks
// React can pause rendering to handle higher priority updates
```

**Concurrent Features:**
```javascript
// React 18 concurrent features enabled by Fiber
import { startTransition, useDeferredValue } from 'react';

function SearchResults() {
    const [query, setQuery] = useState('');
    const [results, setResults] = useState([]);

    // Defer expensive updates
    const deferredQuery = useDeferredValue(query);

    const handleSearch = (newQuery) => {
        setQuery(newQuery); // Immediate update for input

        // Mark expensive update as transition
        startTransition(() => {
            setResults(searchData(newQuery)); // Can be interrupted
        });
    };

    return (
        <div>
            <input onChange={(e) => handleSearch(e.target.value)} />
            <SearchResultsList query={deferredQuery} results={results} />
        </div>
    );
}
```

### Diff Algorithm

**React's reconciliation process for efficiently updating the DOM.**

**Reconciliation Rules:**
```javascript
// 1. Different element types = complete rebuild
// Old tree:
<div>
    <Counter />
</div>

// New tree:
<span>
    <Counter />
</span>

// Result: Unmount div and Counter, mount new span and Counter

// 2. Same element type = update props
// Old: <div className="old" title="Old Title" />
// New: <div className="new" title="New Title" />
// Result: Update className and title attributes only

// 3. Component elements = update props and re-render
// Old: <Counter count={1} />
// New: <Counter count={2} />
// Result: Update props and re-render Counter component
```

**Key Optimization:**
```javascript
// Without keys - inefficient
function TodoList({ todos }) {
    return (
        <ul>
            {todos.map((todo, index) => (
                <li key={index}> {/* ❌ Index as key */}
                    <input defaultValue={todo.text} />
                    <button onClick={() => deleteTodo(todo.id)}>Delete</button>
                </li>
            ))}
        </ul>
    );
}

// With proper keys - efficient
function TodoList({ todos }) {
    return (
        <ul>
            {todos.map(todo => (
                <li key={todo.id}> {/* ✅ Stable unique key */}
                    <input defaultValue={todo.text} />
                    <button onClick={() => deleteTodo(todo.id)}>Delete</button>
                </li>
            ))}
        </ul>
    );
}

// When a todo is deleted from the middle:
// Without keys: React re-renders all subsequent items
// With keys: React only removes the specific item
```

**Optimization Strategies:**
```javascript
// 1. Stable keys
const items = data.map(item => (
    <Item key={item.id} data={item} /> // ✅ Stable
));

// 2. Avoid inline objects/functions
// Bad:
<Component style={{ color: 'red' }} onClick={() => doSomething()} />

// Good:
const style = { color: 'red' };
const handleClick = useCallback(() => doSomething(), []);
<Component style={style} onClick={handleClick} />

// 3. Split components to limit re-render scope
function App() {
    const [count, setCount] = useState(0);
    const [users, setUsers] = useState([]);

    return (
        <div>
            <Counter count={count} setCount={setCount} />
            <UserList users={users} /> {/* Won't re-render when count changes */}
        </div>
    );
}
```

### Error Boundaries

**Error boundaries catch JavaScript errors in component trees.**

**Class-based Error Boundary:**
```javascript
class ErrorBoundary extends React.Component {
    constructor(props) {
        super(props);
        this.state = { hasError: false, error: null, errorInfo: null };
    }

    static getDerivedStateFromError(error) {
        // Update state to show error UI
        return { hasError: true };
    }

    componentDidCatch(error, errorInfo) {
        // Log error to error reporting service
        console.error('Error caught by boundary:', error, errorInfo);

        this.setState({
            error: error,
            errorInfo: errorInfo
        });

        // Report to error tracking service
        // logErrorToService(error, errorInfo);
    }

    render() {
        if (this.state.hasError) {
            return (
                <div className="error-boundary">
                    <h2>Something went wrong!</h2>
                    <details style={{ whiteSpace: 'pre-wrap' }}>
                        {this.state.error && this.state.error.toString()}
                        <br />
                        {this.state.errorInfo.componentStack}
                    </details>
                </div>
            );
        }

        return this.props.children;
    }
}

// Usage
function App() {
    return (
        <ErrorBoundary>
            <Header />
            <MainContent />
            <Footer />
        </ErrorBoundary>
    );
}
```

**Hook-based Error Boundary (using library):**
```javascript
// Using react-error-boundary library
import { ErrorBoundary } from 'react-error-boundary';

function ErrorFallback({ error, resetErrorBoundary }) {
    return (
        <div role="alert" className="error-fallback">
            <h2>Oops! Something went wrong:</h2>
            <pre>{error.message}</pre>
            <button onClick={resetErrorBoundary}>Try again</button>
        </div>
    );
}

function App() {
    return (
        <ErrorBoundary
            FallbackComponent={ErrorFallback}
            onError={(error, errorInfo) => {
                console.error('Error logged:', error, errorInfo);
            }}
            onReset={() => {
                // Reset app state if needed
                window.location.reload();
            }}
        >
            <MyApp />
        </ErrorBoundary>
    );
}
```

**What Error Boundaries Catch:**
```javascript
// ✅ Error boundaries catch:
// - Errors in render methods
// - Errors in lifecycle methods
// - Errors in constructors

// ❌ Error boundaries do NOT catch:
// - Event handlers
// - Asynchronous code (setTimeout, promises)
// - Server-side rendering errors
// - Errors in the error boundary itself

// For event handlers, use try-catch:
function Button() {
    const handleClick = () => {
        try {
            riskyOperation();
        } catch (error) {
            console.error('Button click error:', error);
            // Handle error appropriately
        }
    };

    return <button onClick={handleClick}>Click me</button>;
}
```

---

## CSS

### CSS Selectors

**CSS selectors determine which elements styles are applied to.**

**Basic Selectors:**
```css
/* Element selector */
p { color: blue; }

/* Class selector */
.highlight { background: yellow; }

/* ID selector */
#header { font-size: 24px; }

/* Universal selector */
* { margin: 0; padding: 0; }

/* Attribute selectors */
[type="text"] { border: 1px solid gray; }
[href^="https"] { color: green; } /* Starts with */
[href$=".pdf"] { color: red; }   /* Ends with */
[href*="example"] { color: blue; } /* Contains */
```

**Combinators:**
```css
/* Descendant selector */
.container p { color: gray; }

/* Child selector */
.container > p { font-weight: bold; }

/* Adjacent sibling */
h1 + p { margin-top: 0; }

/* General sibling */
h1 ~ p { color: darkgray; }
```

**Pseudo-classes:**
```css
/* State pseudo-classes */
a:hover { color: red; }
a:visited { color: purple; }
a:active { color: orange; }
input:focus { outline: 2px solid blue; }
input:disabled { opacity: 0.5; }

/* Structural pseudo-classes */
li:first-child { font-weight: bold; }
li:last-child { border-bottom: none; }
li:nth-child(odd) { background: #f0f0f0; }
li:nth-child(3n+1) { color: red; }
p:not(.special) { color: gray; }
```

**Pseudo-elements:**
```css
/* Content pseudo-elements */
p::before { content: "→ "; }
p::after { content: " ←"; }

/* Text pseudo-elements */
p::first-line { font-weight: bold; }
p::first-letter { font-size: 2em; float: left; }

/* Selection pseudo-element */
::selection { background: yellow; color: black; }
```

**Specificity:**
```css
/* Specificity calculation: inline, IDs, classes, elements */
/* 1000 */ style="color: red"
/* 0100 */ #header
/* 0010 */ .nav, [type="text"], :hover
/* 0001 */ div, p, a

/* Examples */
div p { color: blue; }        /* 0002 */
.content p { color: green; }  /* 0011 */
#main .content p { color: red; } /* 0111 */
```

### Box Model

**The CSS box model describes how element dimensions are calculated.**

**Box Model Components:**
```css
.box {
    /* Content area */
    width: 200px;
    height: 100px;

    /* Padding (inside border) */
    padding: 20px;
    /* padding: 10px 20px; top/bottom left/right */
    /* padding: 10px 15px 20px 25px; top right bottom left */

    /* Border */
    border: 2px solid black;
    border-width: 2px;
    border-style: solid;
    border-color: black;

    /* Margin (outside border) */
    margin: 10px;

    /* Total width = width + padding-left + padding-right + border-left + border-right */
    /* Total width = 200 + 20 + 20 + 2 + 2 = 244px */
}
```

**Box-sizing:**
```css
/* Default: content-box */
.content-box {
    box-sizing: content-box;
    width: 200px;
    padding: 20px;
    border: 2px solid black;
    /* Total width: 244px */
}

/* Border-box: includes padding and border in width */
.border-box {
    box-sizing: border-box;
    width: 200px;
    padding: 20px;
    border: 2px solid black;
    /* Total width: 200px, content width: 156px */
}

/* Global border-box (recommended) */
*, *::before, *::after {
    box-sizing: border-box;
}
```

**Margin Collapse:**
```css
/* Vertical margins collapse between adjacent elements */
.element1 {
    margin-bottom: 20px;
}

.element2 {
    margin-top: 30px;
}
/* Actual margin between elements: 30px (not 50px) */

/* Prevent margin collapse */
.container {
    overflow: hidden; /* Creates BFC */
    /* or */
    padding: 1px 0;
    /* or */
    border: 1px solid transparent;
}
```

### BFC (Block Formatting Context)

**BFC creates isolated rendering regions with specific layout rules.**

**BFC Triggers:**
```css
/* Display values */
.bfc { display: flow-root; } /* Explicit BFC */
.bfc { display: inline-block; }
.bfc { display: table-cell; }
.bfc { display: table-caption; }
.bfc { display: flex; }
.bfc { display: grid; }

/* Position values */
.bfc { position: absolute; }
.bfc { position: fixed; }

/* Overflow values (not visible) */
.bfc { overflow: hidden; }
.bfc { overflow: scroll; }
.bfc { overflow: auto; }

/* Float values */
.bfc { float: left; }
.bfc { float: right; }
```

**BFC Applications:**

**1. Clearing Floats:**
```css
.clearfix {
    overflow: hidden; /* Creates BFC to contain floated children */
}

/* Modern clearfix */
.clearfix::after {
    content: "";
    display: table;
    clear: both;
}
```

**2. Preventing Margin Collapse:**
```css
.parent {
    overflow: hidden; /* BFC prevents margin collapse with children */
}

.child {
    margin-top: 20px; /* Won't collapse with parent's margin */
}
```

**3. Two-Column Layout:**
```css
.sidebar {
    float: left;
    width: 200px;
}

.content {
    overflow: hidden; /* BFC makes content not wrap around float */
    margin-left: 220px;
}
```

### Flexbox Layout

**Flexbox provides efficient layout control for one-dimensional layouts.**

**Container Properties:**
```css
.container {
    display: flex;
    flex-direction: row | column;
    justify-content: flex-start | center | space-between | space-around;
    align-items: flex-start | center | flex-end | stretch;
    flex-wrap: nowrap | wrap;
}
```

**Item Properties:**
```css
.item {
    flex: 1; /* flex-grow: 1, flex-shrink: 1, flex-basis: 0% */
    flex-grow: 1; /* How much to grow */
    flex-shrink: 1; /* How much to shrink */
    flex-basis: auto; /* Initial size */
    align-self: auto | flex-start | center | flex-end;
}
```

**Common Patterns:**
- **Centering:** `justify-content: center; align-items: center;`
- **Equal distribution:** `flex: 1` on all items
- **Responsive layout:** Combined with media queries

### BFC (Block Formatting Context)

**BFC creates isolated rendering regions with specific layout rules.**

**Triggers:**
- `overflow: hidden`
- `display: flow-root`
- `position: absolute/fixed`
- `float: left/right`

**Applications:**
- Clearing floats
- Preventing margin collapse
- Creating self-contained layouts

### CSS Grid

**CSS Grid provides two-dimensional layout control.**

**Grid Container:**
```css
.grid-container {
    display: grid;

    /* Define columns and rows */
    grid-template-columns: 200px 1fr 100px;
    grid-template-rows: auto 1fr auto;

    /* Or using repeat */
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(auto-fit, minmax(200px, 1fr));

    /* Gap between items */
    gap: 20px;
    /* grid-gap: 20px; (deprecated) */

    /* Named grid lines */
    grid-template-columns: [start] 250px [content-start] 1fr [content-end] 250px [end];
}
```

**Grid Items:**
```css
.grid-item {
    /* Position by line numbers */
    grid-column: 1 / 3; /* From line 1 to line 3 */
    grid-row: 2 / 4;

    /* Position by line names */
    grid-column: start / content-end;

    /* Span syntax */
    grid-column: span 2; /* Span 2 columns */
    grid-row: span 3;    /* Span 3 rows */

    /* Shorthand */
    grid-area: 2 / 1 / 4 / 3; /* row-start / col-start / row-end / col-end */
}
```

**Grid Template Areas:**
```css
.layout {
    display: grid;
    grid-template-areas:
        "header header header"
        "sidebar content ads"
        "footer footer footer";
    grid-template-columns: 200px 1fr 150px;
    grid-template-rows: auto 1fr auto;
    gap: 20px;
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.content { grid-area: content; }
.ads { grid-area: ads; }
.footer { grid-area: footer; }
```

**Responsive Grid:**
```css
.responsive-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

/* Auto-placement */
.masonry-like {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    grid-auto-rows: minmax(100px, auto);
    gap: 15px;
}
```

### Positioning and Layout

**CSS positioning controls element placement in the document flow.**

**Position Values:**
```css
/* Static (default) - normal document flow */
.static {
    position: static;
}

/* Relative - positioned relative to normal position */
.relative {
    position: relative;
    top: 10px;    /* Move down 10px from normal position */
    left: 20px;   /* Move right 20px from normal position */
}

/* Absolute - positioned relative to nearest positioned ancestor */
.absolute {
    position: absolute;
    top: 0;       /* 0px from top of positioned parent */
    right: 0;     /* 0px from right of positioned parent */
}

/* Fixed - positioned relative to viewport */
.fixed {
    position: fixed;
    bottom: 20px; /* Always 20px from bottom of viewport */
    right: 20px;  /* Always 20px from right of viewport */
}

/* Sticky - switches between relative and fixed */
.sticky {
    position: sticky;
    top: 0;       /* Sticks to top when scrolling */
}
```

**Z-index and Stacking Context:**
```css
.modal-backdrop {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
    z-index: 1000;
}

.modal {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background: white;
    z-index: 1001; /* Higher than backdrop */
}

/* Stacking context creators */
.stacking-context {
    /* Any of these create a new stacking context */
    opacity: 0.99;
    transform: translateZ(0);
    filter: blur(0);
    will-change: transform;
    isolation: isolate;
}
```

### Centering Techniques

**Various methods to center elements horizontally and vertically.**

**Horizontal Centering:**
```css
/* Text and inline elements */
.text-center {
    text-align: center;
}

/* Block elements with known width */
.block-center {
    width: 300px;
    margin: 0 auto;
}

/* Flexbox */
.flex-center {
    display: flex;
    justify-content: center;
}

/* Grid */
.grid-center {
    display: grid;
    justify-content: center;
}
```

**Vertical Centering:**
```css
/* Single line text */
.line-height {
    height: 100px;
    line-height: 100px;
}

/* Table cell */
.table-cell {
    display: table-cell;
    vertical-align: middle;
    height: 200px;
}

/* Flexbox */
.flex-vertical {
    display: flex;
    align-items: center;
    height: 200px;
}

/* Grid */
.grid-vertical {
    display: grid;
    align-content: center;
    height: 200px;
}

/* Absolute positioning */
.absolute-center {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
}
```

**Perfect Centering (Horizontal + Vertical):**
```css
/* Flexbox (recommended) */
.flex-perfect {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

/* Grid */
.grid-perfect {
    display: grid;
    place-items: center;
    height: 100vh;
}

/* Absolute positioning */
.absolute-perfect {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

/* Absolute with known dimensions */
.absolute-known {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 200px;
    height: 100px;
    margin-left: -100px; /* -width/2 */
    margin-top: -50px;   /* -height/2 */
}
```

### Responsive Design

**Creating layouts that adapt to different screen sizes and devices.**

**Viewport Meta Tag:**
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

**Media Queries:**
```css
/* Mobile first approach */
.container {
    width: 100%;
    padding: 10px;
}

/* Tablet */
@media (min-width: 768px) {
    .container {
        max-width: 750px;
        margin: 0 auto;
        padding: 20px;
    }
}

/* Desktop */
@media (min-width: 1024px) {
    .container {
        max-width: 1200px;
        padding: 30px;
    }
}

/* High DPI displays */
@media (-webkit-min-device-pixel-ratio: 2), (min-resolution: 192dpi) {
    .logo {
        background-image: url('logo@2x.png');
        background-size: 100px 50px;
    }
}

/* Orientation */
@media (orientation: landscape) {
    .sidebar {
        width: 300px;
    }
}

@media (orientation: portrait) {
    .sidebar {
        width: 100%;
    }
}
```

**Responsive Units:**
```css
/* Relative to font size */
.em-based {
    padding: 1em;     /* 16px if font-size is 16px */
    margin: 0.5em;    /* 8px if font-size is 16px */
}

/* Relative to root font size */
.rem-based {
    font-size: 1.2rem; /* 19.2px if root font-size is 16px */
    padding: 2rem;     /* 32px if root font-size is 16px */
}

/* Viewport units */
.viewport-units {
    width: 50vw;       /* 50% of viewport width */
    height: 100vh;     /* 100% of viewport height */
    font-size: 4vmin;  /* 4% of smaller viewport dimension */
    padding: 2vmax;    /* 2% of larger viewport dimension */
}

/* Percentage */
.percentage {
    width: 50%;        /* 50% of parent width */
    height: 75%;       /* 75% of parent height */
}
```

**Responsive Images:**
```css
/* Fluid images */
img {
    max-width: 100%;
    height: auto;
}

/* Responsive background images */
.hero {
    background-image: url('hero-mobile.jpg');
    background-size: cover;
    background-position: center;
}

@media (min-width: 768px) {
    .hero {
        background-image: url('hero-tablet.jpg');
    }
}

@media (min-width: 1024px) {
    .hero {
        background-image: url('hero-desktop.jpg');
    }
}
```

**Container Queries (Modern):**
```css
/* Container queries allow styling based on container size */
.card-container {
    container-type: inline-size;
}

@container (min-width: 300px) {
    .card {
        display: flex;
        flex-direction: row;
    }
}

@container (max-width: 299px) {
    .card {
        display: block;
    }
}
```

### Column Layouts

**Creating multi-column layouts with CSS.**

**CSS Multi-Column:**
```css
.multi-column {
    column-count: 3;
    column-gap: 20px;
    column-rule: 1px solid #ccc;
    column-fill: balance;
}

/* Responsive columns */
.responsive-columns {
    column-width: 250px; /* Minimum column width */
    column-gap: 20px;
}

/* Control column breaks */
.no-break {
    break-inside: avoid;
    page-break-inside: avoid; /* Fallback */
}

.break-before {
    break-before: column;
}
```

**Flexbox Columns:**
```css
.flex-columns {
    display: flex;
    gap: 20px;
}

.flex-column {
    flex: 1; /* Equal width columns */
}

/* Specific column widths */
.sidebar {
    flex: 0 0 250px; /* Fixed width sidebar */
}

.main-content {
    flex: 1; /* Flexible main content */
}
```

**Grid Columns:**
```css
.grid-layout {
    display: grid;
    grid-template-columns: 250px 1fr 200px; /* Sidebar, main, aside */
    gap: 20px;
}

/* Responsive grid columns */
.responsive-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}
```

### CSS Units (px, em, rem, vh, vw)

**Understanding different CSS units and when to use them.**

**Absolute Units:**
```css
/* Pixels - absolute unit */
.pixel-based {
    width: 300px;
    height: 200px;
    font-size: 16px;
    margin: 10px;
}

/* Points, inches, centimeters (print media) */
@media print {
    .print-text {
        font-size: 12pt;
        margin: 1in;
    }
}
```

**Relative Units:**
```css
/* em - relative to parent font size */
.em-based {
    font-size: 1.2em;    /* 1.2 × parent font size */
    padding: 0.5em;      /* 0.5 × current font size */
    margin: 1em 0;       /* 1 × current font size */
}

/* rem - relative to root font size */
.rem-based {
    font-size: 1.5rem;   /* 1.5 × root font size (usually 16px) */
    padding: 2rem;       /* 2 × root font size */
    margin: 1rem 0;      /* 1 × root font size */
}

/* Percentage - relative to parent */
.percentage-based {
    width: 50%;          /* 50% of parent width */
    height: 75%;         /* 75% of parent height */
    font-size: 120%;     /* 120% of parent font size */
}
```

**Viewport Units:**
```css
/* Viewport width and height */
.viewport-units {
    width: 50vw;         /* 50% of viewport width */
    height: 100vh;       /* 100% of viewport height */
    font-size: 4vw;      /* 4% of viewport width */
}

/* Viewport minimum and maximum */
.viewport-min-max {
    font-size: 3vmin;    /* 3% of smaller viewport dimension */
    padding: 2vmax;      /* 2% of larger viewport dimension */
}

/* Practical examples */
.hero-section {
    height: 100vh;       /* Full viewport height */
    width: 100vw;        /* Full viewport width */
}

.responsive-text {
    font-size: calc(16px + 2vw); /* Fluid typography */
}
```

**When to Use Each:**
```css
/* Use px for: */
.borders { border: 1px solid #ccc; }
.shadows { box-shadow: 0 2px 4px rgba(0,0,0,0.1); }

/* Use em for: */
.component-spacing {
    padding: 1em;        /* Scales with component font size */
    margin-bottom: 0.5em;
}

/* Use rem for: */
.consistent-spacing {
    margin: 1rem 0;      /* Consistent across components */
    font-size: 1.2rem;   /* Predictable sizing */
}

/* Use % for: */
.layout-widths {
    width: 70%;          /* Responsive layouts */
}

/* Use vh/vw for: */
.full-screen {
    height: 100vh;       /* Full screen sections */
    width: 100vw;
}
```

### Device Pixels and DPR

**Understanding device pixels, CSS pixels, and device pixel ratio.**

**Concepts:**
```css
/* CSS pixels vs Device pixels */
.image {
    width: 100px;        /* 100 CSS pixels */
    height: 100px;       /* May be 200+ device pixels on high-DPI displays */
}

/* High-DPI image handling */
.logo {
    background-image: url('logo.png');
    background-size: 100px 50px;
}

@media (-webkit-min-device-pixel-ratio: 2), (min-resolution: 192dpi) {
    .logo {
        background-image: url('logo@2x.png');
    }
}

@media (-webkit-min-device-pixel-ratio: 3), (min-resolution: 288dpi) {
    .logo {
        background-image: url('logo@3x.png');
    }
}
```

**Responsive Images:**
```html
<!-- Using srcset for different DPR -->
<img src="image.jpg"
     srcset="image.jpg 1x, image@2x.jpg 2x, image@3x.jpg 3x"
     alt="Responsive image">

<!-- Using picture element -->
<picture>
    <source media="(min-width: 800px)"
            srcset="large.jpg 1x, large@2x.jpg 2x">
    <source media="(min-width: 400px)"
            srcset="medium.jpg 1x, medium@2x.jpg 2x">
    <img src="small.jpg"
         srcset="small.jpg 1x, small@2x.jpg 2x"
         alt="Responsive image">
</picture>
```

**JavaScript DPR Detection:**
```javascript
// Detect device pixel ratio
const dpr = window.devicePixelRatio || 1;
console.log('Device Pixel Ratio:', dpr);

// Load appropriate image based on DPR
function getImageUrl(baseName, extension = 'jpg') {
    const dpr = window.devicePixelRatio || 1;

    if (dpr >= 3) {
        return `${baseName}@3x.${extension}`;
    } else if (dpr >= 2) {
        return `${baseName}@2x.${extension}`;
    } else {
        return `${baseName}.${extension}`;
    }
}

// Usage
const imageUrl = getImageUrl('logo', 'png');
document.querySelector('.logo').src = imageUrl;
```

### CSS3 Features

**Modern CSS3 features and properties.**

**Border Radius and Shadows:**
```css
.modern-card {
    /* Rounded corners */
    border-radius: 8px;
    border-radius: 50%; /* Circle */
    border-radius: 10px 20px 30px 40px; /* Individual corners */

    /* Box shadows */
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    box-shadow: 0 4px 8px rgba(0,0,0,0.1), 0 2px 4px rgba(0,0,0,0.06);
    box-shadow: inset 0 2px 4px rgba(0,0,0,0.1); /* Inner shadow */

    /* Text shadows */
    text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
}
```

**Gradients:**
```css
.gradients {
    /* Linear gradients */
    background: linear-gradient(to right, #ff0000, #00ff00);
    background: linear-gradient(45deg, #ff0000, #00ff00, #0000ff);
    background: linear-gradient(to bottom, #ff0000 0%, #00ff00 50%, #0000ff 100%);

    /* Radial gradients */
    background: radial-gradient(circle, #ff0000, #00ff00);
    background: radial-gradient(ellipse at center, #ff0000, #00ff00);

    /* Conic gradients */
    background: conic-gradient(from 0deg, red, yellow, green, blue, red);
}
```

**Transforms:**
```css
.transforms {
    /* 2D transforms */
    transform: translate(50px, 100px);
    transform: rotate(45deg);
    transform: scale(1.5);
    transform: skew(10deg, 20deg);

    /* 3D transforms */
    transform: translateZ(50px);
    transform: rotateX(45deg);
    transform: rotateY(45deg);
    transform: rotateZ(45deg);

    /* Combined transforms */
    transform: translate(50px, 100px) rotate(45deg) scale(1.2);

    /* Transform origin */
    transform-origin: top left;
    transform-origin: 50% 50%;
    transform-origin: center bottom;
}
```

**Transitions:**
```css
.transitions {
    transition: all 0.3s ease;
    transition: opacity 0.5s ease-in-out;
    transition: transform 0.3s cubic-bezier(0.4, 0, 0.2, 1);

    /* Multiple properties */
    transition:
        opacity 0.3s ease,
        transform 0.3s ease,
        background-color 0.2s ease;
}

.transitions:hover {
    opacity: 0.8;
    transform: translateY(-2px);
    background-color: #f0f0f0;
}
```

### CSS Animations

**Creating smooth animations and transitions with CSS.**

**CSS Transitions:**
```css
.button {
    background-color: #007bff;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;

    /* Transition properties */
    transition: all 0.3s ease;
    transition: background-color 0.3s ease, transform 0.2s ease;
    transition: opacity 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}

.button:hover {
    background-color: #0056b3;
    transform: translateY(-2px);
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

.button:active {
    transform: translateY(0);
    transition-duration: 0.1s;
}
```

**CSS Keyframe Animations:**
```css
/* Define keyframes */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes bounce {
    0%, 20%, 53%, 80%, 100% {
        transform: translate3d(0, 0, 0);
    }
    40%, 43% {
        transform: translate3d(0, -30px, 0);
    }
    70% {
        transform: translate3d(0, -15px, 0);
    }
    90% {
        transform: translate3d(0, -4px, 0);
    }
}

@keyframes spin {
    from {
        transform: rotate(0deg);
    }
    to {
        transform: rotate(360deg);
    }
}

/* Apply animations */
.fade-in {
    animation: fadeIn 0.6s ease-out;
}

.bounce {
    animation: bounce 1s ease-in-out;
}

.loading-spinner {
    animation: spin 1s linear infinite;
}

/* Animation properties */
.complex-animation {
    animation-name: fadeIn;
    animation-duration: 2s;
    animation-timing-function: ease-in-out;
    animation-delay: 0.5s;
    animation-iteration-count: infinite;
    animation-direction: alternate;
    animation-fill-mode: both;
    animation-play-state: running;

    /* Shorthand */
    animation: fadeIn 2s ease-in-out 0.5s infinite alternate both;
}
```

**Advanced Animation Techniques:**
```css
/* Staggered animations */
.list-item {
    opacity: 0;
    animation: fadeIn 0.6s ease-out forwards;
}

.list-item:nth-child(1) { animation-delay: 0.1s; }
.list-item:nth-child(2) { animation-delay: 0.2s; }
.list-item:nth-child(3) { animation-delay: 0.3s; }
.list-item:nth-child(4) { animation-delay: 0.4s; }

/* Or using CSS custom properties */
.list-item {
    animation: fadeIn 0.6s ease-out forwards;
    animation-delay: calc(var(--index) * 0.1s);
}

/* 3D animations */
.card {
    perspective: 1000px;
}

.card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.6s;
    transform-style: preserve-3d;
}

.card:hover .card-inner {
    transform: rotateY(180deg);
}

.card-front, .card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
}

.card-back {
    transform: rotateY(180deg);
}

/* Performance optimizations */
.optimized-animation {
    /* Use transform and opacity for best performance */
    transform: translateZ(0); /* Force hardware acceleration */
    will-change: transform, opacity; /* Hint to browser */
}

/* Reduce motion for accessibility */
@media (prefers-reduced-motion: reduce) {
    .animation {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }
}
```

**JavaScript Animation Control:**
```css
/* CSS classes for JavaScript control */
.slide-enter {
    transform: translateX(-100%);
    opacity: 0;
}

.slide-enter-active {
    transform: translateX(0);
    opacity: 1;
    transition: transform 0.3s ease, opacity 0.3s ease;
}

.slide-exit {
    transform: translateX(0);
    opacity: 1;
}

.slide-exit-active {
    transform: translateX(100%);
    opacity: 0;
    transition: transform 0.3s ease, opacity 0.3s ease;
}

/* Animation states */
.modal {
    opacity: 0;
    transform: scale(0.8);
    transition: all 0.3s ease;
    pointer-events: none;
}

.modal.is-open {
    opacity: 1;
    transform: scale(1);
    pointer-events: auto;
}

.modal.is-closing {
    opacity: 0;
    transform: scale(0.8);
}
```

### CSS Performance

**Optimizing CSS for better performance.**

**Efficient Selectors:**
```css
/* ❌ Inefficient selectors */
* { margin: 0; }                    /* Universal selector */
div > div > div > p { color: red; } /* Deep nesting */
.nav li a:hover { color: blue; }    /* Complex descendant */

/* ✅ Efficient selectors */
.reset { margin: 0; }               /* Class selector */
.content-text { color: red; }       /* Direct class */
.nav-link:hover { color: blue; }    /* Simple class with pseudo */

/* Selector performance (fastest to slowest) */
/* 1. ID selectors: #header */
/* 2. Class selectors: .nav */
/* 3. Type selectors: div */
/* 4. Adjacent sibling: h1 + p */
/* 5. Child: ul > li */
/* 6. Descendant: div p */
/* 7. Universal: * */
/* 8. Attribute: [type="text"] */
/* 9. Pseudo-classes: :hover */
```

**CSS Architecture:**
```css
/* BEM methodology for maintainable CSS */
.block { }
.block__element { }
.block--modifier { }

/* Example */
.card { }
.card__header { }
.card__body { }
.card__footer { }
.card--featured { }
.card--large { }

/* Utility classes */
.u-margin-bottom-small { margin-bottom: 1rem; }
.u-text-center { text-align: center; }
.u-hidden { display: none; }

/* Component-based organization */
/* components/button.css */
.btn {
    display: inline-block;
    padding: 0.5rem 1rem;
    border: none;
    border-radius: 0.25rem;
    cursor: pointer;
}

.btn--primary { background-color: #007bff; }
.btn--secondary { background-color: #6c757d; }
.btn--large { padding: 0.75rem 1.5rem; }
```

**Critical CSS:**
```css
/* Inline critical CSS for above-the-fold content */
/* This should be inlined in <head> */
.header {
    background: #fff;
    padding: 1rem;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.hero {
    height: 100vh;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    display: flex;
    align-items: center;
    justify-content: center;
}

.hero__title {
    font-size: 3rem;
    color: white;
    text-align: center;
}

/* Non-critical CSS loaded asynchronously */
/* This can be loaded after page load */
.footer { /* ... */ }
.sidebar { /* ... */ }
.modal { /* ... */ }
```

**CSS Optimization Techniques:**
```css
/* 1. Minimize reflows and repaints */
.optimized {
    /* Use transform instead of changing position */
    transform: translateX(100px); /* ✅ Composite layer */
    /* left: 100px; ❌ Causes reflow */

    /* Use opacity instead of visibility */
    opacity: 0; /* ✅ Composite layer */
    /* visibility: hidden; ❌ Causes repaint */
}

/* 2. Use will-change for animations */
.animated-element {
    will-change: transform, opacity;
}

/* Remove will-change after animation */
.animated-element.animation-complete {
    will-change: auto;
}

/* 3. Avoid expensive properties */
.expensive {
    /* These properties are expensive to animate */
    /* box-shadow, border-radius, filter, etc. */

    /* Use transform for movement */
    transform: translateX(10px); /* ✅ */
    /* margin-left: 10px; ❌ */
}

/* 4. Use contain property */
.contained {
    contain: layout style paint;
    /* Tells browser this element is isolated */
}

/* 5. Optimize images */
.image-container {
    /* Use object-fit for responsive images */
    object-fit: cover;
    object-position: center;

    /* Lazy loading hint */
    content-visibility: auto;
    contain-intrinsic-size: 300px 200px;
}
```

---

## ES6

### Variable Declarations (var, let, const)

**ES6 introduced `let` and `const` to address issues with `var`.**

**var Issues:**
```javascript
// Function scoping (not block scoping)
function varExample() {
    if (true) {
        var x = 1;
    }
    console.log(x); // 1 (accessible outside block)
}

// Hoisting behavior
console.log(hoisted); // undefined (not ReferenceError)
var hoisted = "I'm hoisted";

// Loop variable problem
for (var i = 0; i < 3; i++) {
    setTimeout(() => console.log(i), 100); // Prints 3, 3, 3
}
```

**let and const Solutions:**
```javascript
// Block scoping
function letExample() {
    if (true) {
        let x = 1;
        const y = 2;
    }
    // console.log(x); // ReferenceError
    // console.log(y); // ReferenceError
}

// Temporal Dead Zone
console.log(notHoisted); // ReferenceError
let notHoisted = "I'm not hoisted";

// Loop variable fix
for (let i = 0; i < 3; i++) {
    setTimeout(() => console.log(i), 100); // Prints 0, 1, 2
}

// const immutability
const obj = { name: 'John' };
obj.name = 'Jane'; // ✅ Object properties can be modified
obj.age = 30;      // ✅ Can add properties
// obj = {};       // ❌ Cannot reassign the variable

const arr = [1, 2, 3];
arr.push(4);       // ✅ Array methods work
// arr = [];       // ❌ Cannot reassign
```

**Best Practices:**
```javascript
// Use const by default
const API_URL = 'https://api.example.com';
const users = [];

// Use let when reassignment is needed
let currentUser = null;
let isLoading = false;

// Avoid var in modern JavaScript
// var should only be used for legacy compatibility
```

### Arrow Functions

**Arrow functions provide concise syntax and lexical `this` binding.**

**Syntax Variations:**
```javascript
// Traditional function
function add(a, b) {
    return a + b;
}

// Arrow function - full syntax
const add = (a, b) => {
    return a + b;
};

// Arrow function - implicit return
const add = (a, b) => a + b;

// Single parameter (parentheses optional)
const square = x => x * x;
const square = (x) => x * x; // Also valid

// No parameters
const greet = () => 'Hello!';

// Returning object literal (wrap in parentheses)
const createUser = (name, age) => ({ name, age });

// Multiple statements
const processData = (data) => {
    const processed = data.map(item => item.value);
    const filtered = processed.filter(value => value > 0);
    return filtered.reduce((sum, value) => sum + value, 0);
};
```

**Lexical `this` Binding:**
```javascript
// Traditional function - dynamic this
function Timer() {
    this.seconds = 0;

    setInterval(function() {
        this.seconds++; // `this` refers to global object or undefined
        console.log(this.seconds); // NaN or error
    }, 1000);
}

// Arrow function - lexical this
function Timer() {
    this.seconds = 0;

    setInterval(() => {
        this.seconds++; // `this` refers to Timer instance
        console.log(this.seconds); // Works correctly
    }, 1000);
}

// Class methods
class EventHandler {
    constructor() {
        this.count = 0;
    }

    // Traditional method
    handleClick() {
        this.count++;
    }

    // Arrow method (binds this automatically)
    handleClickArrow = () => {
        this.count++;
    }

    setupListeners() {
        // Need to bind traditional method
        button.addEventListener('click', this.handleClick.bind(this));

        // Arrow method is automatically bound
        button.addEventListener('click', this.handleClickArrow);
    }
}
```

**When NOT to Use Arrow Functions:**
```javascript
// Object methods (this doesn't work as expected)
const obj = {
    name: 'John',
    greet: () => {
        console.log(`Hello, ${this.name}`); // this is not obj
    }
};

// Constructor functions
const Person = (name) => {
    this.name = name; // Error: arrow functions can't be constructors
};

// Methods that need dynamic this
const button = {
    text: 'Click me',
    handleClick: () => {
        console.log(this.text); // this is not the button object
    }
};
```

### Template Literals

**Template literals provide string interpolation and multiline strings.**

**Basic Syntax:**
```javascript
// String interpolation
const name = 'John';
const age = 30;

// Old way
const message = 'Hello, my name is ' + name + ' and I am ' + age + ' years old.';

// Template literal
const message = `Hello, my name is ${name} and I am ${age} years old.`;

// Expressions in interpolation
const price = 19.99;
const tax = 0.08;
const total = `Total: $${(price * (1 + tax)).toFixed(2)}`;
```

**Multiline Strings:**
```javascript
// Old way (awkward)
const html = '<div>\n' +
             '  <h1>Title</h1>\n' +
             '  <p>Content</p>\n' +
             '</div>';

// Template literal (natural)
const html = `
<div>
  <h1>Title</h1>
  <p>Content</p>
</div>
`;

// SQL queries
const query = `
    SELECT users.name, users.email, profiles.bio
    FROM users
    JOIN profiles ON users.id = profiles.user_id
    WHERE users.active = true
    ORDER BY users.created_at DESC
    LIMIT ${limit}
`;
```

**Tagged Template Literals:**
```javascript
// Custom template processing
function highlight(strings, ...values) {
    return strings.reduce((result, string, i) => {
        const value = values[i] ? `<mark>${values[i]}</mark>` : '';
        return result + string + value;
    }, '');
}

const searchTerm = 'JavaScript';
const text = highlight`Learn ${searchTerm} programming with ${searchTerm} examples`;
// Result: "Learn <mark>JavaScript</mark> programming with <mark>JavaScript</mark> examples"

// Styled components example
function css(strings, ...values) {
    return strings.reduce((result, string, i) => {
        const value = values[i] || '';
        return result + string + value;
    }, '');
}

const primaryColor = '#007bff';
const buttonStyles = css`
    background-color: ${primaryColor};
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 4px;
`;
```

### Destructuring

**Destructuring allows extracting values from arrays and objects into variables.**

**Array Destructuring:**
```javascript
// Basic array destructuring
const numbers = [1, 2, 3, 4, 5];
const [first, second, third] = numbers;
console.log(first, second, third); // 1, 2, 3

// Skip elements
const [first, , third, , fifth] = numbers;
console.log(first, third, fifth); // 1, 3, 5

// Rest operator
const [head, ...tail] = numbers;
console.log(head); // 1
console.log(tail); // [2, 3, 4, 5]

// Default values
const [a, b, c = 0] = [1, 2];
console.log(a, b, c); // 1, 2, 0

// Swapping variables
let x = 1, y = 2;
[x, y] = [y, x];
console.log(x, y); // 2, 1

// Function return values
function getCoordinates() {
    return [10, 20];
}
const [x, y] = getCoordinates();
```

**Object Destructuring:**
```javascript
// Basic object destructuring
const user = {
    name: 'John',
    age: 30,
    email: 'john@example.com',
    address: {
        city: 'New York',
        country: 'USA'
    }
};

const { name, age, email } = user;
console.log(name, age, email); // John, 30, john@example.com

// Renaming variables
const { name: userName, age: userAge } = user;
console.log(userName, userAge); // John, 30

// Default values
const { name, age, phone = 'N/A' } = user;
console.log(phone); // N/A

// Nested destructuring
const { address: { city, country } } = user;
console.log(city, country); // New York, USA

// Rest operator
const { name, ...otherProps } = user;
console.log(otherProps); // { age: 30, email: '...', address: {...} }
```

**Function Parameters:**
```javascript
// Object parameter destructuring
function createUser({ name, age, email = 'unknown' }) {
    return {
        id: Math.random(),
        name,
        age,
        email,
        createdAt: new Date()
    };
}

const newUser = createUser({
    name: 'Jane',
    age: 25
});

// Array parameter destructuring
function calculateDistance([x1, y1], [x2, y2]) {
    return Math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2);
}

const distance = calculateDistance([0, 0], [3, 4]); // 5

// Mixed destructuring
function processApiResponse({ data: { users, total }, status }) {
    if (status === 'success') {
        return users.map(({ id, name, email }) => ({ id, name, email }));
    }
    return [];
}
```

### Promises

**Promises provide elegant asynchronous programming compared to callbacks.**

**States:**
- **Pending:** Initial state
- **Fulfilled:** Operation completed successfully
- **Rejected:** Operation failed

**Basic Usage:**
```js
const promise = new Promise((resolve, reject) => {
    // Async operation
    if (success) {
        resolve(result);
    } else {
        reject(error);
    }
});

promise
    .then(result => console.log(result))
    .catch(error => console.error(error))
    .finally(() => console.log('Cleanup'));
```

**Promise Methods:**
```js
// All must resolve
Promise.all([p1, p2, p3]).then(results => {});

// First to resolve/reject
Promise.race([p1, p2, p3]).then(result => {});

// All settle (resolve or reject)
Promise.allSettled([p1, p2, p3]).then(results => {});
```

**Practical Applications:**
- API request management
- Image loading with timeout
- Parallel request coordination
- Error handling chains

### Async/Await

**Syntactic sugar over Promises for cleaner asynchronous code.**

```js
async function fetchData() {
    try {
        const response = await fetch('/api/data');
        const data = await response.json();
        return data;
    } catch (error) {
        console.error('Error:', error);
    }
}
```

### Modules

**ES6 modules provide standardized import/export syntax.**

```js
// Named exports
export const utils = {};
export function helper() {}

// Default export
export default class Component {}

// Imports
import Component, { utils, helper } from './module';
import * as Everything from './module';
```

### Classes

**ES6 classes provide a cleaner syntax for creating objects and inheritance.**

**Basic Class Syntax:**
```javascript
class Person {
    constructor(name, age) {
        this.name = name;
        this.age = age;
    }

    // Method
    greet() {
        return `Hello, I'm ${this.name}`;
    }

    // Getter
    get info() {
        return `${this.name} is ${this.age} years old`;
    }

    // Setter
    set age(value) {
        if (value < 0) {
            throw new Error('Age cannot be negative');
        }
        this._age = value;
    }

    get age() {
        return this._age;
    }

    // Static method
    static createGuest() {
        return new Person('Guest', 0);
    }
}

// Usage
const person = new Person('John', 30);
console.log(person.greet()); // "Hello, I'm John"
console.log(person.info);    // "John is 30 years old"

const guest = Person.createGuest();
```

**Inheritance:**
```javascript
class Employee extends Person {
    constructor(name, age, jobTitle, salary) {
        super(name, age); // Call parent constructor
        this.jobTitle = jobTitle;
        this.salary = salary;
    }

    // Override method
    greet() {
        return `${super.greet()}, I'm a ${this.jobTitle}`;
    }

    // New method
    getAnnualSalary() {
        return this.salary * 12;
    }
}

const employee = new Employee('Jane', 28, 'Developer', 5000);
console.log(employee.greet()); // "Hello, I'm Jane, I'm a Developer"
```

### Generators

**Generators are functions that can pause and resume execution.**

**Basic Generator:**
```javascript
function* simpleGenerator() {
    yield 1;
    yield 2;
    yield 3;
}

const gen = simpleGenerator();
console.log(gen.next()); // { value: 1, done: false }
console.log(gen.next()); // { value: 2, done: false }
console.log(gen.next()); // { value: 3, done: false }
console.log(gen.next()); // { value: undefined, done: true }

// Using for...of
for (const value of simpleGenerator()) {
    console.log(value); // 1, 2, 3
}
```

**Practical Examples:**
```javascript
// ID generator
function* idGenerator() {
    let id = 1;
    while (true) {
        yield id++;
    }
}

const getId = idGenerator();
console.log(getId.next().value); // 1
console.log(getId.next().value); // 2

// Fibonacci sequence
function* fibonacci() {
    let a = 0, b = 1;
    while (true) {
        yield a;
        [a, b] = [b, a + b];
    }
}

const fib = fibonacci();
for (let i = 0; i < 10; i++) {
    console.log(fib.next().value);
}

// Async data processing
function* processData(data) {
    for (const item of data) {
        const processed = yield item * 2;
        console.log('Received:', processed);
    }
}

const processor = processData([1, 2, 3, 4]);
console.log(processor.next());      // { value: 2, done: false }
console.log(processor.next('OK'));  // Logs: "Received: OK"
```

### Iterators

**Iterators provide a way to access elements of a collection sequentially.**

**Iterator Protocol:**
```javascript
// Custom iterator
function createIterator(array) {
    let index = 0;

    return {
        next() {
            if (index < array.length) {
                return { value: array[index++], done: false };
            } else {
                return { done: true };
            }
        }
    };
}

const iterator = createIterator([1, 2, 3]);
console.log(iterator.next()); // { value: 1, done: false }
console.log(iterator.next()); // { value: 2, done: false }
console.log(iterator.next()); // { value: 3, done: false }
console.log(iterator.next()); // { done: true }
```

**Iterable Protocol:**
```javascript
// Custom iterable object
const range = {
    start: 1,
    end: 5,

    [Symbol.iterator]() {
        let current = this.start;
        const end = this.end;

        return {
            next() {
                if (current <= end) {
                    return { value: current++, done: false };
                } else {
                    return { done: true };
                }
            }
        };
    }
};

// Usage
for (const num of range) {
    console.log(num); // 1, 2, 3, 4, 5
}

// Spread operator works too
console.log([...range]); // [1, 2, 3, 4, 5]
```

### Set and Map

**New data structures for storing unique values and key-value pairs.**

**Set:**
```javascript
// Creating sets
const set = new Set();
const setWithValues = new Set([1, 2, 3, 3, 4]); // [1, 2, 3, 4]

// Set methods
set.add(1);
set.add(2);
set.add(2); // Duplicate, won't be added
console.log(set.size); // 2

console.log(set.has(1)); // true
set.delete(1);
console.log(set.has(1)); // false

// Iteration
for (const value of set) {
    console.log(value);
}

// Convert to array
const array = [...set];

// Practical uses
const uniqueArray = [...new Set([1, 2, 2, 3, 3, 4])]; // [1, 2, 3, 4]

// Set operations
const setA = new Set([1, 2, 3]);
const setB = new Set([3, 4, 5]);

// Union
const union = new Set([...setA, ...setB]); // [1, 2, 3, 4, 5]

// Intersection
const intersection = new Set([...setA].filter(x => setB.has(x))); // [3]

// Difference
const difference = new Set([...setA].filter(x => !setB.has(x))); // [1, 2]
```

**Map:**
```javascript
// Creating maps
const map = new Map();
const mapWithValues = new Map([
    ['key1', 'value1'],
    ['key2', 'value2']
]);

// Map methods
map.set('name', 'John');
map.set('age', 30);
map.set(1, 'number key');
map.set(true, 'boolean key');

console.log(map.get('name')); // 'John'
console.log(map.has('age'));  // true
console.log(map.size);        // 4

map.delete('age');
console.log(map.has('age'));  // false

// Iteration
for (const [key, value] of map) {
    console.log(`${key}: ${value}`);
}

// Get all keys/values
console.log([...map.keys()]);   // ['name', 1, true]
console.log([...map.values()]); // ['John', 'number key', 'boolean key']

// Object vs Map
const obj = {};
const map2 = new Map();

// Objects have prototype keys
console.log('toString' in obj); // true

// Maps only have what you put in
console.log(map2.has('toString')); // false

// Any type can be a key in Map
const keyObj = {};
const keyFunc = function() {};
map2.set(keyObj, 'object key');
map2.set(keyFunc, 'function key');
```

---

## HTTP

### HTTP vs HTTPS

**HTTP (HyperText Transfer Protocol) vs HTTPS (HTTP Secure)**

**HTTP Characteristics:**
```
- Port: 80 (default)
- Protocol: Plain text
- Security: None
- URL: http://example.com
- Speed: Faster (no encryption overhead)
- Use case: Development, non-sensitive data
```

**HTTPS Characteristics:**
```
- Port: 443 (default)
- Protocol: HTTP over TLS/SSL
- Security: Encrypted, authenticated, integrity-checked
- URL: https://example.com
- Speed: Slightly slower (encryption overhead)
- Use case: Production, sensitive data, required by browsers
```

**HTTPS Benefits:**
- **Data Encryption:** Prevents eavesdropping
- **Data Integrity:** Prevents tampering
- **Authentication:** Verifies server identity
- **SEO Benefits:** Google ranking factor
- **Browser Features:** Required for modern APIs (geolocation, camera, etc.)
- **User Trust:** Green lock icon, no "Not Secure" warning

### HTTP Versions (1.0, 1.1, 2.0)

**HTTP/1.0 (1996):**
```
- One request per connection
- No persistent connections
- Simple request/response model
- Limited caching
- No host header (one domain per IP)
```

**HTTP/1.1 (1997):**
```
- Persistent connections (keep-alive)
- Request pipelining
- Chunked transfer encoding
- Host header (virtual hosting)
- Better caching mechanisms
- Range requests (partial content)
```

**HTTP/1.1 Example:**
```http
GET /api/users HTTP/1.1
Host: example.com
Connection: keep-alive
Accept: application/json
User-Agent: Mozilla/5.0...

HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1234
Connection: keep-alive

{"users": [...]}
```

**HTTP/2.0 (2015):**
```
- Binary framing (not text-based)
- Multiplexing (multiple requests over single connection)
- Header compression (HPACK)
- Server push
- Stream prioritization
- Backward compatible with HTTP/1.1
```

**HTTP/2 Benefits:**
```javascript
// HTTP/1.1 - Multiple connections needed
fetch('/api/users');     // Connection 1
fetch('/api/posts');     // Connection 2
fetch('/api/comments');  // Connection 3

// HTTP/2 - Single connection, multiplexed
fetch('/api/users');     // Stream 1
fetch('/api/posts');     // Stream 2
fetch('/api/comments');  // Stream 3
// All over same connection simultaneously
```

### HTTP Status Codes

**Status codes indicate the result of HTTP requests.**

**1xx Informational:**
```
100 Continue - Server received headers, client should send body
101 Switching Protocols - Server switching to different protocol
```

**2xx Success:**
```
200 OK - Request successful
201 Created - Resource created successfully
202 Accepted - Request accepted for processing
204 No Content - Success but no content to return
206 Partial Content - Range request successful
```

**3xx Redirection:**
```
301 Moved Permanently - Resource permanently moved
302 Found - Resource temporarily moved
304 Not Modified - Resource not changed (cache valid)
307 Temporary Redirect - Temporary redirect, method preserved
308 Permanent Redirect - Permanent redirect, method preserved
```

**4xx Client Error:**
```
400 Bad Request - Invalid request syntax
401 Unauthorized - Authentication required
403 Forbidden - Server understood but refuses
404 Not Found - Resource not found
405 Method Not Allowed - HTTP method not supported
409 Conflict - Request conflicts with current state
422 Unprocessable Entity - Validation errors
429 Too Many Requests - Rate limit exceeded
```

**5xx Server Error:**
```
500 Internal Server Error - Generic server error
501 Not Implemented - Server doesn't support functionality
502 Bad Gateway - Invalid response from upstream
503 Service Unavailable - Server temporarily unavailable
504 Gateway Timeout - Upstream server timeout
```

**Practical Usage:**
```javascript
async function handleApiResponse(response) {
    switch (response.status) {
        case 200:
            return await response.json();
        case 201:
            console.log('Resource created');
            return await response.json();
        case 204:
            console.log('Success, no content');
            return null;
        case 400:
            throw new Error('Bad request - check your data');
        case 401:
            // Redirect to login
            window.location.href = '/login';
            break;
        case 403:
            throw new Error('Access forbidden');
        case 404:
            throw new Error('Resource not found');
        case 429:
            throw new Error('Rate limit exceeded - try again later');
        case 500:
            throw new Error('Server error - try again later');
        default:
            throw new Error(`Unexpected status: ${response.status}`);
    }
}
```

### HTTP Headers

**Headers provide metadata about requests and responses.**

**Common Request Headers:**
```http
GET /api/users HTTP/1.1
Host: api.example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64)
Accept: application/json, text/plain, */*
Accept-Language: en-US,en;q=0.9
Accept-Encoding: gzip, deflate, br
Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
Content-Type: application/json
Content-Length: 123
Cache-Control: no-cache
If-None-Match: "abc123"
Origin: https://example.com
Referer: https://example.com/dashboard
```

**Common Response Headers:**
```http
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8
Content-Length: 1234
Content-Encoding: gzip
Cache-Control: public, max-age=3600
ETag: "abc123"
Last-Modified: Wed, 21 Oct 2023 07:28:00 GMT
Access-Control-Allow-Origin: https://example.com
Access-Control-Allow-Methods: GET, POST, PUT, DELETE
Access-Control-Allow-Headers: Content-Type, Authorization
Set-Cookie: sessionId=abc123; HttpOnly; Secure; SameSite=Strict
X-RateLimit-Limit: 1000
X-RateLimit-Remaining: 999
X-RateLimit-Reset: 1634567890
```

**Security Headers:**
```http
Strict-Transport-Security: max-age=31536000; includeSubDomains
Content-Security-Policy: default-src 'self'; script-src 'self' 'unsafe-inline'
X-Content-Type-Options: nosniff
X-Frame-Options: DENY
X-XSS-Protection: 1; mode=block
Referrer-Policy: strict-origin-when-cross-origin
```

**JavaScript Header Manipulation:**
```javascript
// Setting request headers
const response = await fetch('/api/data', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
        'Authorization': `Bearer ${token}`,
        'X-Custom-Header': 'custom-value'
    },
    body: JSON.stringify(data)
});

// Reading response headers
const contentType = response.headers.get('Content-Type');
const rateLimit = response.headers.get('X-RateLimit-Remaining');

// Iterating headers
for (const [key, value] of response.headers) {
    console.log(`${key}: ${value}`);
}
```

### GET vs POST

**Understanding the differences between HTTP methods.**

**GET Method:**
```http
GET /api/users?page=1&limit=10&sort=name HTTP/1.1
Host: api.example.com
Accept: application/json
```

**GET Characteristics:**
- **Purpose:** Retrieve data
- **Data location:** URL query parameters
- **Caching:** Can be cached
- **Bookmarking:** Can be bookmarked
- **History:** Stored in browser history
- **Data length:** Limited by URL length (~2048 chars)
- **Security:** Less secure (data visible in URL)
- **Idempotent:** Yes (same result on multiple calls)

**POST Method:**
```http
POST /api/users HTTP/1.1
Host: api.example.com
Content-Type: application/json
Content-Length: 123

{
    "name": "John Doe",
    "email": "john@example.com",
    "age": 30
}
```

**POST Characteristics:**
- **Purpose:** Submit data, create resources
- **Data location:** Request body
- **Caching:** Not cached by default
- **Bookmarking:** Cannot be bookmarked
- **History:** Not stored in browser history
- **Data length:** No practical limit
- **Security:** More secure (data in body)
- **Idempotent:** No (may have side effects)

**Other HTTP Methods:**
```javascript
// PUT - Update/replace entire resource
await fetch('/api/users/123', {
    method: 'PUT',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(updatedUser)
});

// PATCH - Partial update
await fetch('/api/users/123', {
    method: 'PATCH',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email: 'newemail@example.com' })
});

// DELETE - Remove resource
await fetch('/api/users/123', {
    method: 'DELETE'
});

// HEAD - Get headers only (no body)
const response = await fetch('/api/users/123', {
    method: 'HEAD'
});
console.log(response.headers.get('Content-Length'));

// OPTIONS - Get allowed methods
const response = await fetch('/api/users', {
    method: 'OPTIONS'
});
console.log(response.headers.get('Allow')); // GET, POST, PUT, DELETE
```

### HTTP Versions

**HTTP/1.0:**
- Single request per connection
- No persistent connections
- Simple request/response model

**HTTP/1.1:**
- Persistent connections (`keep-alive`)
- Request pipelining
- Chunked transfer encoding
- Host header for virtual hosting

**HTTP/2.0:**
- **Binary framing** for efficiency
- **Multiplexing** - multiple requests over single connection
- **Header compression** (HPACK)
- **Server push** capabilities

### HTTPS Security

**HTTPS = HTTP + TLS/SSL encryption**

**Security Features:**
- **Encryption:** Data protection in transit
- **Authentication:** Server identity verification
- **Integrity:** Data tampering detection

**Handshake Process:**
1. Client Hello (supported ciphers)
2. Server Hello (chosen cipher, certificate)
3. Key exchange and verification
4. Encrypted communication begins

### WebSocket

**Full-duplex communication protocol for real-time applications.**

**Features:**
- Persistent connection after handshake
- Low latency bidirectional communication
- Binary and text frame support
- Built on TCP, uses HTTP for initial handshake

**Use Cases:**
- Real-time chat applications
- Live data feeds (stocks, sports)
- Collaborative editing
- Gaming applications
- Live streaming

**WebSocket Implementation:**
```javascript
// Client-side WebSocket
class WebSocketClient {
    constructor(url) {
        this.url = url;
        this.ws = null;
        this.reconnectAttempts = 0;
        this.maxReconnectAttempts = 5;
    }

    connect() {
        this.ws = new WebSocket(this.url);

        this.ws.onopen = (event) => {
            console.log('WebSocket connected');
            this.reconnectAttempts = 0;
        };

        this.ws.onmessage = (event) => {
            try {
                const data = JSON.parse(event.data);
                this.handleMessage(data);
            } catch (error) {
                console.error('Invalid JSON received:', event.data);
            }
        };

        this.ws.onclose = (event) => {
            console.log('WebSocket closed:', event.code, event.reason);
            this.handleReconnect();
        };

        this.ws.onerror = (error) => {
            console.error('WebSocket error:', error);
        };
    }

    send(data) {
        if (this.ws && this.ws.readyState === WebSocket.OPEN) {
            this.ws.send(JSON.stringify(data));
        } else {
            console.error('WebSocket not connected');
        }
    }

    handleReconnect() {
        if (this.reconnectAttempts < this.maxReconnectAttempts) {
            this.reconnectAttempts++;
            setTimeout(() => {
                console.log(`Reconnecting... Attempt ${this.reconnectAttempts}`);
                this.connect();
            }, 1000 * this.reconnectAttempts);
        }
    }

    handleMessage(data) {
        // Override in subclass
        console.log('Received:', data);
    }

    close() {
        if (this.ws) {
            this.ws.close();
        }
    }
}

// Usage
const client = new WebSocketClient('wss://api.example.com/ws');
client.connect();
client.send({ type: 'subscribe', channel: 'chat' });
```

### TCP vs UDP

**Understanding the transport layer protocols underlying HTTP.**

**TCP (Transmission Control Protocol):**
```
Characteristics:
- Connection-oriented (handshake required)
- Reliable delivery (guaranteed order, no loss)
- Error checking and correction
- Flow control and congestion control
- Higher overhead
- Slower but more reliable

Use Cases:
- HTTP/HTTPS
- Email (SMTP, POP3, IMAP)
- File transfer (FTP)
- SSH, Telnet
- Database connections
```

**UDP (User Datagram Protocol):**
```
Characteristics:
- Connectionless (no handshake)
- Unreliable delivery (no guarantee of order or delivery)
- No error correction
- No flow control
- Lower overhead
- Faster but less reliable

Use Cases:
- DNS queries
- Video streaming
- Online gaming
- VoIP
- DHCP
```

**Comparison:**
```javascript
// TCP-like behavior (HTTP)
async function reliableRequest(url, data) {
    let attempts = 0;
    const maxAttempts = 3;

    while (attempts < maxAttempts) {
        try {
            const response = await fetch(url, {
                method: 'POST',
                body: JSON.stringify(data),
                headers: { 'Content-Type': 'application/json' }
            });

            if (response.ok) {
                return await response.json();
            }
            throw new Error(`HTTP ${response.status}`);
        } catch (error) {
            attempts++;
            if (attempts >= maxAttempts) throw error;

            // Exponential backoff
            await new Promise(resolve =>
                setTimeout(resolve, 1000 * Math.pow(2, attempts))
            );
        }
    }
}

// UDP-like behavior (fire and forget)
function unreliableRequest(url, data) {
    fetch(url, {
        method: 'POST',
        body: JSON.stringify(data),
        headers: { 'Content-Type': 'application/json' }
    }).catch(() => {
        // Ignore errors - fire and forget
    });
}
```

### TCP/IP Protocol

**The foundation of internet communication.**

**TCP/IP Stack Layers:**
```
Application Layer (HTTP, HTTPS, FTP, SMTP)
    ↓
Transport Layer (TCP, UDP)
    ↓
Internet Layer (IP, ICMP)
    ↓
Network Access Layer (Ethernet, WiFi)
```

**IP Addressing:**
```javascript
// IPv4 addresses
const ipv4Examples = [
    '192.168.1.1',    // Private network
    '10.0.0.1',       // Private network
    '172.16.0.1',     // Private network
    '8.8.8.8',        // Google DNS (public)
    '127.0.0.1'       // Localhost
];

// IPv6 addresses
const ipv6Examples = [
    '2001:0db8:85a3:0000:0000:8a2e:0370:7334',
    '::1',            // Localhost
    '::'              // All zeros
];

// Port numbers
const commonPorts = {
    HTTP: 80,
    HTTPS: 443,
    FTP: 21,
    SSH: 22,
    SMTP: 25,
    DNS: 53,
    POP3: 110,
    IMAP: 143
};
```

### OSI Model

**Seven-layer model for network communication.**

**OSI Layers:**
```
7. Application Layer
   - HTTP, HTTPS, FTP, SMTP, DNS
   - User interface and network services

6. Presentation Layer
   - Encryption, compression, data formatting
   - SSL/TLS encryption

5. Session Layer
   - Session management, authentication
   - SQL sessions, RPC

4. Transport Layer
   - TCP, UDP
   - End-to-end communication, error recovery

3. Network Layer
   - IP, ICMP, routing
   - Logical addressing, path determination

2. Data Link Layer
   - Ethernet, WiFi, switches
   - Physical addressing, error detection

1. Physical Layer
   - Cables, hubs, repeaters
   - Electrical signals, bits
```

**Web Request OSI Flow:**
```javascript
// Application Layer (Layer 7)
fetch('https://api.example.com/users')

// Presentation Layer (Layer 6)
// - HTTPS encryption applied
// - JSON data formatting

// Session Layer (Layer 5)
// - TLS session established
// - Authentication handled

// Transport Layer (Layer 4)
// - TCP connection established
// - Data segmented into packets

// Network Layer (Layer 3)
// - IP routing to destination
// - Packet forwarding

// Data Link Layer (Layer 2)
// - Ethernet frame creation
// - MAC address resolution

// Physical Layer (Layer 1)
// - Electrical signals transmitted
// - Physical medium (cable/wireless)
```

### DNS Resolution

**Domain Name System translates domain names to IP addresses.**

**DNS Resolution Process:**
```
1. Browser cache check
2. OS cache check
3. Router cache check
4. ISP DNS server query
5. Root DNS server query
6. TLD DNS server query (.com, .org, etc.)
7. Authoritative DNS server query
8. IP address returned
```

**DNS Record Types:**
```javascript
const dnsRecords = {
    A: '192.168.1.1',           // IPv4 address
    AAAA: '2001:db8::1',        // IPv6 address
    CNAME: 'example.com',       // Canonical name (alias)
    MX: 'mail.example.com',     // Mail exchange
    TXT: 'v=spf1 include:_spf.google.com ~all', // Text record
    NS: 'ns1.example.com',      // Name server
    SOA: 'ns1.example.com admin.example.com', // Start of authority
    PTR: 'example.com'          // Reverse DNS lookup
};

// DNS lookup simulation
async function dnsLookup(domain) {
    try {
        // Modern browsers don't expose direct DNS API
        // This simulates the process
        const response = await fetch(`https://dns.google/resolve?name=${domain}&type=A`);
        const data = await response.json();

        return data.Answer?.map(record => ({
            name: record.name,
            type: record.type,
            data: record.data,
            ttl: record.TTL
        }));
    } catch (error) {
        console.error('DNS lookup failed:', error);
        return null;
    }
}
```

### CDN (Content Delivery Network)

**Distributed network of servers for faster content delivery.**

**CDN Benefits:**
```
- Reduced latency (geographically closer servers)
- Improved availability (redundancy)
- Reduced bandwidth costs
- DDoS protection
- Caching static assets
- Global reach
```

**CDN Implementation:**
```html
<!-- CDN for libraries -->
<script src="https://cdn.jsdelivr.net/npm/react@18/umd/react.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/lodash.js/4.17.21/lodash.min.js"></script>

<!-- CDN for fonts -->
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">

<!-- CDN for images -->
<img src="https://images.unsplash.com/photo-1234567890" alt="Example">
```

**CDN Configuration:**
```javascript
// CDN cache headers
const cdnHeaders = {
    'Cache-Control': 'public, max-age=31536000', // 1 year
    'ETag': '"abc123"',
    'Last-Modified': 'Wed, 21 Oct 2023 07:28:00 GMT',
    'Vary': 'Accept-Encoding',
    'Content-Encoding': 'gzip'
};

// CDN fallback strategy
function loadWithFallback(cdnUrl, fallbackUrl) {
    return new Promise((resolve, reject) => {
        const script = document.createElement('script');
        script.src = cdnUrl;

        script.onload = () => resolve(script);
        script.onerror = () => {
            // Fallback to local version
            script.src = fallbackUrl;
            script.onload = () => resolve(script);
            script.onerror = () => reject(new Error('Both CDN and fallback failed'));
        };

        document.head.appendChild(script);
    });
}

// Usage
loadWithFallback(
    'https://cdn.jsdelivr.net/npm/react@18/umd/react.production.min.js',
    '/js/react.min.js'
);
```

### TCP Handshakes and Termination

**Understanding TCP connection establishment and teardown.**

**TCP Three-Way Handshake:**
```
Client                    Server
  |                         |
  |-------- SYN ----------->|  (1. Client initiates)
  |                         |
  |<----- SYN-ACK ----------|  (2. Server acknowledges)
  |                         |
  |-------- ACK ----------->|  (3. Client confirms)
  |                         |
  |    Connection Established
```

**TCP Four-Way Termination:**
```
Client                    Server
  |                         |
  |-------- FIN ----------->|  (1. Client initiates close)
  |                         |
  |<------- ACK ------------|  (2. Server acknowledges)
  |                         |
  |<------- FIN ------------|  (3. Server initiates close)
  |                         |
  |-------- ACK ----------->|  (4. Client acknowledges)
  |                         |
  |    Connection Closed
```

**Connection States:**
```javascript
const tcpStates = {
    CLOSED: 'No connection',
    LISTEN: 'Server waiting for connections',
    SYN_SENT: 'Client sent SYN, waiting for SYN-ACK',
    SYN_RECEIVED: 'Server received SYN, sent SYN-ACK',
    ESTABLISHED: 'Connection established',
    FIN_WAIT_1: 'Client sent FIN, waiting for ACK',
    FIN_WAIT_2: 'Client received ACK, waiting for FIN',
    CLOSE_WAIT: 'Server received FIN, waiting to close',
    CLOSING: 'Both sides closing simultaneously',
    LAST_ACK: 'Server sent FIN, waiting for ACK',
    TIME_WAIT: 'Client waiting for delayed packets'
};
```

### URL to Page Load Process

**Complete process from URL entry to page display.**

**Step-by-Step Process:**
```javascript
// 1. URL Parsing
const url = new URL('https://example.com/path?query=value#fragment');
console.log({
    protocol: url.protocol,  // 'https:'
    hostname: url.hostname,  // 'example.com'
    pathname: url.pathname,  // '/path'
    search: url.search,      // '?query=value'
    hash: url.hash          // '#fragment'
});

// 2. DNS Resolution
// Browser checks cache, then queries DNS servers

// 3. TCP Connection
// Three-way handshake with server

// 4. TLS Handshake (for HTTPS)
// Certificate verification, key exchange

// 5. HTTP Request
const request = `
GET /path?query=value HTTP/1.1
Host: example.com
User-Agent: Mozilla/5.0...
Accept: text/html,application/xhtml+xml
Accept-Language: en-US,en;q=0.9
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
`;

// 6. Server Processing
// Route handling, database queries, business logic

// 7. HTTP Response
const response = `
HTTP/1.1 200 OK
Content-Type: text/html; charset=utf-8
Content-Length: 1234
Cache-Control: public, max-age=3600
Set-Cookie: sessionId=abc123

<!DOCTYPE html>
<html>...
`;

// 8. Browser Processing
// HTML parsing, DOM construction, CSS parsing, JavaScript execution

// 9. Resource Loading
// Images, stylesheets, scripts, fonts

// 10. Rendering
// Layout calculation, painting, compositing
```

**Performance Timeline:**
```javascript
// Measuring page load performance
window.addEventListener('load', () => {
    const perfData = performance.getEntriesByType('navigation')[0];

    console.log({
        dnsLookup: perfData.domainLookupEnd - perfData.domainLookupStart,
        tcpConnect: perfData.connectEnd - perfData.connectStart,
        tlsHandshake: perfData.secureConnectionStart > 0 ?
            perfData.connectEnd - perfData.secureConnectionStart : 0,
        httpRequest: perfData.responseStart - perfData.requestStart,
        httpResponse: perfData.responseEnd - perfData.responseStart,
        domParsing: perfData.domContentLoadedEventStart - perfData.responseEnd,
        resourceLoading: perfData.loadEventStart - perfData.domContentLoadedEventEnd,
        totalTime: perfData.loadEventEnd - perfData.navigationStart
    });
});
```

---

## TypeScript

### TypeScript vs JavaScript

**TypeScript is a superset of JavaScript that adds static type checking.**

**Key Differences:**
```typescript
// JavaScript - Dynamic typing
let message = "Hello";
message = 42;           // Valid at runtime
message.toUpperCase();  // Runtime error

// TypeScript - Static typing
let message: string = "Hello";
// message = 42;        // ❌ Compile-time error
message.toUpperCase();  // ✅ Type-safe
```

**Benefits of TypeScript:**
- **Early Error Detection:** Catch errors at compile time
- **Better IDE Support:** IntelliSense, autocomplete, refactoring
- **Self-Documenting Code:** Types serve as documentation
- **Safer Refactoring:** Compiler ensures type consistency
- **Enhanced Team Collaboration:** Clear contracts between modules

**TypeScript Compilation:**
```bash
# Install TypeScript
npm install -g typescript

# Compile TypeScript to JavaScript
tsc app.ts

# Watch mode
tsc app.ts --watch

# Project compilation
tsc --init  # Creates tsconfig.json
tsc         # Compiles entire project
```

### Data Types

**TypeScript provides both primitive and complex types.**

**Primitive Types:**
```typescript
// Basic types
let name: string = "John";
let age: number = 30;
let isActive: boolean = true;
let value: null = null;
let notDefined: undefined = undefined;

// Symbol and BigInt
let sym: symbol = Symbol("id");
let bigNumber: bigint = 100n;

// Any type (avoid when possible)
let anything: any = "hello";
anything = 42;
anything = true;

// Unknown type (safer than any)
let userInput: unknown = getUserInput();
if (typeof userInput === "string") {
    console.log(userInput.toUpperCase()); // Type guard required
}

// Void type
function logMessage(msg: string): void {
    console.log(msg);
    // No return value
}

// Never type
function throwError(message: string): never {
    throw new Error(message);
}

function infiniteLoop(): never {
    while (true) {
        // Never returns
    }
}
```

**Array and Tuple Types:**
```typescript
// Array types
let numbers: number[] = [1, 2, 3];
let strings: Array<string> = ["a", "b", "c"];

// Mixed array
let mixed: (string | number)[] = ["hello", 42, "world"];

// Tuple types
let person: [string, number] = ["John", 30];
let rgb: [number, number, number] = [255, 0, 0];

// Optional tuple elements
let point: [number, number, number?] = [10, 20]; // z is optional

// Rest elements in tuples
let scores: [string, ...number[]] = ["John", 95, 87, 92];

// Named tuple elements
let employee: [name: string, age: number, salary: number] = ["John", 30, 50000];
```

**Object Types:**
```typescript
// Object type annotation
let user: {
    name: string;
    age: number;
    email?: string; // Optional property
} = {
    name: "John",
    age: 30
};

// Index signatures
let scores: { [subject: string]: number } = {
    math: 95,
    science: 87,
    english: 92
};

// Nested objects
let company: {
    name: string;
    address: {
        street: string;
        city: string;
        country: string;
    };
    employees: {
        name: string;
        position: string;
    }[];
} = {
    name: "Tech Corp",
    address: {
        street: "123 Main St",
        city: "New York",
        country: "USA"
    },
    employees: [
        { name: "John", position: "Developer" },
        { name: "Jane", position: "Designer" }
    ]
};
```

### Data Types

**TypeScript provides both primitive and complex types.**

**Union and Intersection Types:**
```typescript
// Union types
type StringOrNumber = string | number;
let value: StringOrNumber = "hello";
value = 42; // Both valid

// Discriminated unions
type Shape =
    | { kind: "circle"; radius: number }
    | { kind: "rectangle"; width: number; height: number }
    | { kind: "square"; size: number };

function getArea(shape: Shape): number {
    switch (shape.kind) {
        case "circle":
            return Math.PI * shape.radius ** 2;
        case "rectangle":
            return shape.width * shape.height;
        case "square":
            return shape.size ** 2;
        default:
            // Exhaustiveness check
            const _exhaustive: never = shape;
            return _exhaustive;
    }
}

// Intersection types
type Person = { name: string; age: number };
type Employee = { employeeId: string; department: string };
type PersonEmployee = Person & Employee;

let worker: PersonEmployee = {
    name: "John",
    age: 30,
    employeeId: "E001",
    department: "Engineering"
};
```

**Literal Types:**
```typescript
// String literals
type Theme = "light" | "dark" | "auto";
let currentTheme: Theme = "light";

// Numeric literals
type DiceRoll = 1 | 2 | 3 | 4 | 5 | 6;
let roll: DiceRoll = 4;

// Boolean literals
type Success = true;
type Failure = false;

// Template literal types
type EventName<T extends string> = `on${Capitalize<T>}`;
type ClickEvent = EventName<"click">; // "onClick"
type HoverEvent = EventName<"hover">; // "onHover"

// Pattern matching with template literals
type ExtractRouteParams<T extends string> =
    T extends `${string}/:${infer Param}/${infer Rest}`
        ? { [K in Param | keyof ExtractRouteParams<`/${Rest}`>]: string }
        : T extends `${string}/:${infer Param}`
        ? { [K in Param]: string }
        : {};

type UserRoute = ExtractRouteParams<"/users/:id/posts/:postId">;
// { id: string; postId: string }
```

### Type System

**TypeScript adds static typing to JavaScript for better development experience.**

**Basic Types:**
```typescript
let name: string = "John";
let age: number = 30;
let isActive: boolean = true;
let items: string[] = ["a", "b", "c"];
let tuple: [string, number] = ["hello", 42];
```

**Advanced Types:**
```typescript
// Union types
let value: string | number;

// Intersection types
type User = { name: string } & { age: number };

// Generic types
function identity<T>(arg: T): T {
    return arg;
}
```

### Interfaces

**Interfaces define contracts for object shapes.**

```typescript
interface User {
    readonly id: number;
    name: string;
    age?: number; // Optional property
    [key: string]: any; // Index signature
}

// Function interface
interface SearchFunc {
    (source: string, subString: string): boolean;
}

// Extending interfaces
interface Admin extends User {
    permissions: string[];
}
```

**Applications:**
- API response typing
- Component props definition
- Function parameter contracts
- Class implementation requirements

### Classes

**TypeScript enhances JavaScript classes with type annotations and access modifiers.**

**Basic Class Syntax:**
```typescript
class Person {
    // Property declarations
    private _name: string;
    protected age: number;
    public email: string;
    readonly id: string;

    // Constructor with parameter properties
    constructor(
        name: string,
        age: number,
        email: string,
        public address?: string // Parameter property
    ) {
        this._name = name;
        this.age = age;
        this.email = email;
        this.id = Math.random().toString(36);
    }

    // Getter and setter
    get name(): string {
        return this._name;
    }

    set name(value: string) {
        if (value.length < 2) {
            throw new Error("Name must be at least 2 characters");
        }
        this._name = value;
    }

    // Methods
    greet(): string {
        return `Hello, I'm ${this._name}`;
    }

    // Static methods
    static createGuest(): Person {
        return new Person("Guest", 0, "guest@example.com");
    }
}

// Inheritance
class Employee extends Person {
    constructor(
        name: string,
        age: number,
        email: string,
        private salary: number,
        public department: string
    ) {
        super(name, age, email);
    }

    // Override method
    greet(): string {
        return `${super.greet()}, I work in ${this.department}`;
    }

    // Protected method (accessible in subclasses)
    protected calculateBonus(): number {
        return this.salary * 0.1;
    }
}

// Abstract classes
abstract class Animal {
    constructor(protected name: string) {}

    abstract makeSound(): string; // Must be implemented by subclasses

    move(): string {
        return `${this.name} is moving`;
    }
}

class Dog extends Animal {
    makeSound(): string {
        return `${this.name} barks`;
    }
}
```

**Access Modifiers:**
```typescript
class BankAccount {
    private balance: number = 0;        // Only accessible within class
    protected accountType: string;     // Accessible in subclasses
    public accountNumber: string;      // Accessible everywhere
    readonly createdAt: Date;          // Cannot be modified after initialization

    constructor(accountNumber: string, accountType: string) {
        this.accountNumber = accountNumber;
        this.accountType = accountType;
        this.createdAt = new Date();
    }

    private validateAmount(amount: number): boolean {
        return amount > 0 && amount <= 10000;
    }

    public deposit(amount: number): void {
        if (this.validateAmount(amount)) {
            this.balance += amount;
        }
    }

    public getBalance(): number {
        return this.balance;
    }
}
```

### Functions

**TypeScript provides comprehensive function typing capabilities.**

**Function Type Annotations:**
```typescript
// Function declaration
function add(a: number, b: number): number {
    return a + b;
}

// Function expression
const multiply = function(a: number, b: number): number {
    return a * b;
};

// Arrow function
const divide = (a: number, b: number): number => a / b;

// Optional parameters
function greet(name: string, greeting?: string): string {
    return `${greeting || "Hello"}, ${name}!`;
}

// Default parameters
function createUser(name: string, age: number = 18): User {
    return { name, age };
}

// Rest parameters
function sum(...numbers: number[]): number {
    return numbers.reduce((total, num) => total + num, 0);
}

// Function overloads
function process(value: string): string;
function process(value: number): number;
function process(value: boolean): boolean;
function process(value: string | number | boolean): string | number | boolean {
    if (typeof value === "string") {
        return value.toUpperCase();
    } else if (typeof value === "number") {
        return value * 2;
    } else {
        return !value;
    }
}
```

**Function Types:**
```typescript
// Function type aliases
type MathOperation = (a: number, b: number) => number;
type Predicate<T> = (item: T) => boolean;
type EventHandler<T> = (event: T) => void;

// Using function types
const operations: { [key: string]: MathOperation } = {
    add: (a, b) => a + b,
    subtract: (a, b) => a - b,
    multiply: (a, b) => a * b,
    divide: (a, b) => a / b
};

// Higher-order functions
function createFilter<T>(predicate: Predicate<T>) {
    return function(items: T[]): T[] {
        return items.filter(predicate);
    };
}

const filterEven = createFilter<number>(n => n % 2 === 0);
const evenNumbers = filterEven([1, 2, 3, 4, 5, 6]); // [2, 4, 6]

// Callback functions
function fetchData<T>(
    url: string,
    onSuccess: (data: T) => void,
    onError: (error: Error) => void
): void {
    fetch(url)
        .then(response => response.json())
        .then(onSuccess)
        .catch(onError);
}
```

### Generics

**Generics enable writing reusable, type-safe code.**

**Basic Generics:**
```typescript
// Generic function
function identity<T>(arg: T): T {
    return arg;
}

const stringResult = identity<string>("hello");
const numberResult = identity<number>(42);
const boolResult = identity(true); // Type inference

// Generic interface
interface Container<T> {
    value: T;
    getValue(): T;
    setValue(value: T): void;
}

class Box<T> implements Container<T> {
    constructor(public value: T) {}

    getValue(): T {
        return this.value;
    }

    setValue(value: T): void {
        this.value = value;
    }
}

const stringBox = new Box<string>("hello");
const numberBox = new Box<number>(42);
```

**Generic Constraints:**
```typescript
// Constraint with extends
interface Lengthwise {
    length: number;
}

function logLength<T extends Lengthwise>(arg: T): T {
    console.log(arg.length);
    return arg;
}

logLength("hello");     // ✅ string has length
logLength([1, 2, 3]);   // ✅ array has length
// logLength(42);       // ❌ number doesn't have length

// Keyof constraint
function getProperty<T, K extends keyof T>(obj: T, key: K): T[K] {
    return obj[key];
}

const person = { name: "John", age: 30, email: "john@example.com" };
const name = getProperty(person, "name");     // string
const age = getProperty(person, "age");       // number
// const invalid = getProperty(person, "invalid"); // ❌ Error

// Multiple constraints
interface Serializable {
    serialize(): string;
}

interface Timestamped {
    timestamp: Date;
}

function processData<T extends Serializable & Timestamped>(data: T): string {
    return `${data.timestamp.toISOString()}: ${data.serialize()}`;
}
```

**Advanced Generic Patterns:**
```typescript
// Conditional types
type NonNullable<T> = T extends null | undefined ? never : T;
type StringOrNumber<T> = T extends string ? string : number;

// Mapped types
type Partial<T> = {
    [P in keyof T]?: T[P];
};

type Required<T> = {
    [P in keyof T]-?: T[P];
};

type Readonly<T> = {
    readonly [P in keyof T]: T[P];
};

// Utility types in action
interface User {
    id: number;
    name: string;
    email: string;
    password: string;
}

type PartialUser = Partial<User>;        // All properties optional
type PublicUser = Omit<User, 'password'>; // Exclude password
type UserUpdate = Pick<User, 'name' | 'email'>; // Only name and email
type UserKeys = keyof User;              // 'id' | 'name' | 'email' | 'password'

// Generic API response type
interface ApiResponse<T> {
    data: T;
    status: 'success' | 'error';
    message?: string;
    timestamp: string;
}

interface PaginatedResponse<T> extends ApiResponse<T[]> {
    pagination: {
        page: number;
        limit: number;
        total: number;
        hasNext: boolean;
    };
}

// Usage
type UserListResponse = PaginatedResponse<User>;
type SingleUserResponse = ApiResponse<User>;
```

### Advanced Types

**TypeScript provides powerful advanced type features.**

**Conditional Types:**
```typescript
// Basic conditional type
type IsString<T> = T extends string ? true : false;

type Test1 = IsString<string>; // true
type Test2 = IsString<number>; // false

// Practical conditional types
type NonNullable<T> = T extends null | undefined ? never : T;
type ArrayElement<T> = T extends (infer U)[] ? U : never;

type StringArray = string[];
type ElementType = ArrayElement<StringArray>; // string

// Distributive conditional types
type ToArray<T> = T extends any ? T[] : never;
type StrArrOrNumArr = ToArray<string | number>; // string[] | number[]
```

**Mapped Types:**
```typescript
// Basic mapped type
type Readonly<T> = {
    readonly [P in keyof T]: T[P];
};

type Partial<T> = {
    [P in keyof T]?: T[P];
};

type Required<T> = {
    [P in keyof T]-?: T[P];
};

// Custom mapped types
type Stringify<T> = {
    [K in keyof T]: string;
};

type Nullify<T> = {
    [K in keyof T]: T[K] | null;
};

interface User {
    id: number;
    name: string;
    email: string;
}

type StringUser = Stringify<User>; // { id: string; name: string; email: string; }
type NullableUser = Nullify<User>; // { id: number | null; name: string | null; email: string | null; }
```

**Template Literal Types:**
```typescript
// Template literal types
type EventName<T extends string> = `on${Capitalize<T>}`;
type ClickEvent = EventName<"click">; // "onClick"

// Route parameter extraction
type ExtractRouteParams<T extends string> =
    T extends `${string}/:${infer Param}/${infer Rest}`
        ? { [K in Param | keyof ExtractRouteParams<`/${Rest}`>]: string }
        : T extends `${string}/:${infer Param}`
        ? { [K in Param]: string }
        : {};

type UserRouteParams = ExtractRouteParams<"/users/:id/posts/:postId">;
// { id: string; postId: string }

// SQL query builder types
type SQLOperator = "=" | "!=" | ">" | "<" | ">=" | "<=";
type WhereClause<T extends string> = `${T} ${SQLOperator} ?`;

type UserWhereClause = WhereClause<"age">; // "age = ?" | "age != ?" | etc.
```

### Enums

**Enums allow defining named constants.**

**Numeric Enums:**
```typescript
enum Direction {
    Up,    // 0
    Down,  // 1
    Left,  // 2
    Right  // 3
}

// Custom numeric values
enum Status {
    Pending = 1,
    Approved = 2,
    Rejected = 3
}

// Usage
function move(direction: Direction) {
    switch (direction) {
        case Direction.Up:
            return "Moving up";
        case Direction.Down:
            return "Moving down";
        case Direction.Left:
            return "Moving left";
        case Direction.Right:
            return "Moving right";
    }
}

console.log(move(Direction.Up)); // "Moving up"
console.log(Direction.Up);       // 0
console.log(Direction[0]);       // "Up"
```

**String Enums:**
```typescript
enum Color {
    Red = "red",
    Green = "green",
    Blue = "blue"
}

enum ApiEndpoint {
    Users = "/api/users",
    Posts = "/api/posts",
    Comments = "/api/comments"
}

// Usage
function fetchData(endpoint: ApiEndpoint) {
    return fetch(endpoint);
}

fetchData(ApiEndpoint.Users); // fetch("/api/users")
```

**Const Enums:**
```typescript
// Const enums are inlined at compile time
const enum LogLevel {
    Error,
    Warning,
    Info,
    Debug
}

// This code:
console.log(LogLevel.Error);

// Compiles to:
console.log(0 /* Error */);
```

**Enum Best Practices:**
```typescript
// Use string enums for better debugging
enum Theme {
    Light = "light",
    Dark = "dark",
    Auto = "auto"
}

// Union types as alternative to enums
type ThemeType = "light" | "dark" | "auto";

// Enum with methods (using namespace)
enum Planet {
    Mercury = "mercury",
    Venus = "venus",
    Earth = "earth"
}

namespace Planet {
    export function getDistance(planet: Planet): number {
        switch (planet) {
            case Planet.Mercury: return 57.9;
            case Planet.Venus: return 108.2;
            case Planet.Earth: return 149.6;
            default: return 0;
        }
    }
}

console.log(Planet.getDistance(Planet.Earth)); // 149.6
```

### Decorators

**Decorators provide a way to add metadata and modify classes and methods.**

**Class Decorators:**
```typescript
// Enable experimental decorators in tsconfig.json
// "experimentalDecorators": true

function sealed(constructor: Function) {
    Object.seal(constructor);
    Object.seal(constructor.prototype);
}

@sealed
class Greeter {
    greeting: string;
    constructor(message: string) {
        this.greeting = message;
    }
    greet() {
        return "Hello, " + this.greeting;
    }
}
```

**Method Decorators:**
```typescript
function log(target: any, propertyName: string, descriptor: PropertyDescriptor) {
    const method = descriptor.value;

    descriptor.value = function (...args: any[]) {
        console.log(`Calling ${propertyName} with arguments:`, args);
        const result = method.apply(this, args);
        console.log(`${propertyName} returned:`, result);
        return result;
    };
}

class Calculator {
    @log
    add(a: number, b: number): number {
        return a + b;
    }

    @log
    multiply(a: number, b: number): number {
        return a * b;
    }
}

const calc = new Calculator();
calc.add(2, 3); // Logs method call and result
```

**Property Decorators:**
```typescript
function readonly(target: any, propertyName: string) {
    Object.defineProperty(target, propertyName, {
        writable: false
    });
}

function validate(target: any, propertyName: string) {
    let value = target[propertyName];

    Object.defineProperty(target, propertyName, {
        get: () => value,
        set: (newValue) => {
            if (typeof newValue !== 'string') {
                throw new Error(`${propertyName} must be a string`);
            }
            value = newValue;
        }
    });
}

class User {
    @readonly
    id: number = Math.random();

    @validate
    name: string = "";
}
```

### Namespaces and Modules

**Organizing code with namespaces and modules.**

**Namespaces:**
```typescript
namespace Geometry {
    export interface Point {
        x: number;
        y: number;
    }

    export class Circle {
        constructor(public center: Point, public radius: number) {}

        area(): number {
            return Math.PI * this.radius ** 2;
        }
    }

    export namespace Utils {
        export function distance(p1: Point, p2: Point): number {
            return Math.sqrt((p2.x - p1.x) ** 2 + (p2.y - p1.y) ** 2);
        }
    }
}

// Usage
const point: Geometry.Point = { x: 0, y: 0 };
const circle = new Geometry.Circle(point, 5);
const dist = Geometry.Utils.distance({ x: 0, y: 0 }, { x: 3, y: 4 });
```

**Module Augmentation:**
```typescript
// Extending existing modules
declare global {
    interface Array<T> {
        first(): T | undefined;
        last(): T | undefined;
    }
}

Array.prototype.first = function() {
    return this[0];
};

Array.prototype.last = function() {
    return this[this.length - 1];
};

// Now available on all arrays
const numbers = [1, 2, 3];
console.log(numbers.first()); // 1
console.log(numbers.last());  // 3
```

### TypeScript with React

**Using TypeScript with React for type-safe components.**

**Component Props:**
```typescript
interface ButtonProps {
    children: React.ReactNode;
    onClick: () => void;
    variant?: 'primary' | 'secondary';
    disabled?: boolean;
}

const Button: React.FC<ButtonProps> = ({
    children,
    onClick,
    variant = 'primary',
    disabled = false
}) => {
    return (
        <button
            onClick={onClick}
            disabled={disabled}
            className={`btn btn-${variant}`}
        >
            {children}
        </button>
    );
};

// Usage
<Button onClick={() => console.log('clicked')} variant="secondary">
    Click me
</Button>
```

**Hooks with TypeScript:**
```typescript
// useState with explicit types
const [user, setUser] = useState<User | null>(null);
const [loading, setLoading] = useState<boolean>(false);

// useRef with DOM elements
const inputRef = useRef<HTMLInputElement>(null);

// Custom hooks
function useApi<T>(url: string): {
    data: T | null;
    loading: boolean;
    error: string | null;
} {
    const [data, setData] = useState<T | null>(null);
    const [loading, setLoading] = useState<boolean>(true);
    const [error, setError] = useState<string | null>(null);

    useEffect(() => {
        fetch(url)
            .then(response => response.json())
            .then((data: T) => {
                setData(data);
                setLoading(false);
            })
            .catch((error: Error) => {
                setError(error.message);
                setLoading(false);
            });
    }, [url]);

    return { data, loading, error };
}

// Usage
interface User {
    id: number;
    name: string;
    email: string;
}

function UserProfile({ userId }: { userId: number }) {
    const { data: user, loading, error } = useApi<User>(`/api/users/${userId}`);

    if (loading) return <div>Loading...</div>;
    if (error) return <div>Error: {error}</div>;
    if (!user) return <div>User not found</div>;

    return (
        <div>
            <h1>{user.name}</h1>
            <p>{user.email}</p>
        </div>
    );
}
```

---

## Webpack

### Webpack Fundamentals

**Webpack is a static module bundler for modern JavaScript applications.**

**Core Concepts:**
```javascript
// webpack.config.js
const path = require('path');

module.exports = {
    // Entry point - where webpack starts building
    entry: './src/index.js',

    // Output - where webpack outputs the bundles
    output: {
        path: path.resolve(__dirname, 'dist'),
        filename: 'bundle.js',
        clean: true // Clean dist folder before each build
    },

    // Mode - development, production, or none
    mode: 'development',

    // Loaders - transform files
    module: {
        rules: [
            {
                test: /\.js$/,
                exclude: /node_modules/,
                use: 'babel-loader'
            }
        ]
    },

    // Plugins - extend webpack functionality
    plugins: [],

    // DevServer - development server configuration
    devServer: {
        static: './dist',
        port: 3000,
        hot: true
    }
};
```

**Entry Points:**
```javascript
// Single entry
module.exports = {
    entry: './src/index.js'
};

// Multiple entries
module.exports = {
    entry: {
        app: './src/app.js',
        admin: './src/admin.js'
    },
    output: {
        filename: '[name].bundle.js' // app.bundle.js, admin.bundle.js
    }
};

// Dynamic entry
module.exports = {
    entry: () => {
        return {
            app: './src/app.js',
            vendor: ['react', 'react-dom']
        };
    }
};
```

**Output Configuration:**
```javascript
module.exports = {
    output: {
        // Output directory
        path: path.resolve(__dirname, 'dist'),

        // Filename patterns
        filename: '[name].[contenthash].js', // Cache busting
        chunkFilename: '[name].[contenthash].chunk.js',

        // Asset filenames
        assetModuleFilename: 'assets/[hash][ext][query]',

        // Public path for assets
        publicPath: '/static/',

        // Clean output directory
        clean: true,

        // Library configuration (for libraries)
        library: {
            name: 'MyLibrary',
            type: 'umd'
        }
    }
};
```

### Build Process

**Understanding how webpack transforms and bundles code.**

**Module Resolution:**
```javascript
// webpack resolves modules in this order:
// 1. Exact file match
import './file.js';

// 2. File with extension
import './file'; // looks for file.js, file.json, etc.

// 3. Directory with index file
import './directory'; // looks for directory/index.js

// 4. Node modules
import 'lodash'; // looks in node_modules/lodash

// Custom resolution
module.exports = {
    resolve: {
        // File extensions to try
        extensions: ['.js', '.jsx', '.ts', '.tsx', '.json'],

        // Module directories
        modules: ['node_modules', 'src'],

        // Path aliases
        alias: {
            '@': path.resolve(__dirname, 'src'),
            'components': path.resolve(__dirname, 'src/components'),
            'utils': path.resolve(__dirname, 'src/utils')
        },

        // Fallbacks for Node.js modules
        fallback: {
            "crypto": require.resolve("crypto-browserify"),
            "stream": require.resolve("stream-browserify")
        }
    }
};
```

**Dependency Graph:**
```javascript
// Entry file: src/index.js
import { header } from './components/header.js';
import { footer } from './components/footer.js';
import './styles/main.css';

// Webpack builds dependency graph:
// index.js
//   ├── components/header.js
//   │   └── styles/header.css
//   ├── components/footer.js
//   │   └── styles/footer.css
//   └── styles/main.css
//       └── fonts/roboto.woff2

// All dependencies are bundled together
```

**Code Splitting:**
```javascript
// Dynamic imports for code splitting
async function loadModule() {
    const { default: heavyModule } = await import('./heavy-module.js');
    return heavyModule;
}

// Route-based splitting
const Home = lazy(() => import('./pages/Home'));
const About = lazy(() => import('./pages/About'));

// Vendor splitting
module.exports = {
    optimization: {
        splitChunks: {
            chunks: 'all',
            cacheGroups: {
                vendor: {
                    test: /[\\/]node_modules[\\/]/,
                    name: 'vendors',
                    chunks: 'all'
                },
                common: {
                    name: 'common',
                    minChunks: 2,
                    chunks: 'all',
                    enforce: true
                }
            }
        }
    }
};
```

### Loaders

**Loaders transform files before they're added to the dependency graph.**

**Common Loaders:**
```javascript
module.exports = {
    module: {
        rules: [
            // JavaScript/TypeScript
            {
                test: /\.(js|jsx|ts|tsx)$/,
                exclude: /node_modules/,
                use: {
                    loader: 'babel-loader',
                    options: {
                        presets: ['@babel/preset-env', '@babel/preset-react']
                    }
                }
            },

            // CSS
            {
                test: /\.css$/,
                use: ['style-loader', 'css-loader']
            },

            // Sass/SCSS
            {
                test: /\.s[ac]ss$/,
                use: [
                    'style-loader',
                    'css-loader',
                    {
                        loader: 'sass-loader',
                        options: {
                            sassOptions: {
                                includePaths: ['src/styles']
                            }
                        }
                    }
                ]
            },

            // Images
            {
                test: /\.(png|jpe?g|gif|svg)$/,
                type: 'asset/resource',
                generator: {
                    filename: 'images/[hash][ext][query]'
                }
            },

            // Fonts
            {
                test: /\.(woff|woff2|eot|ttf|otf)$/,
                type: 'asset/resource',
                generator: {
                    filename: 'fonts/[hash][ext][query]'
                }
            },

            // JSON
            {
                test: /\.json$/,
                type: 'json'
            }
        ]
    }
};
```

**Custom Loader:**
```javascript
// simple-loader.js
module.exports = function(source) {
    // Transform the source code
    const transformedSource = source.replace(/console\.log/g, 'console.info');

    // Return the transformed code
    return transformedSource;
};

// Usage in webpack.config.js
module.exports = {
    module: {
        rules: [
            {
                test: /\.js$/,
                use: path.resolve(__dirname, 'loaders/simple-loader.js')
            }
        ]
    }
};
```

### Plugins

**Plugins extend webpack's functionality and perform tasks that loaders can't.**

**Common Plugins:**
```javascript
const HtmlWebpackPlugin = require('html-webpack-plugin');
const MiniCssExtractPlugin = require('mini-css-extract-plugin');
const { CleanWebpackPlugin } = require('clean-webpack-plugin');
const webpack = require('webpack');

module.exports = {
    plugins: [
        // Generate HTML file
        new HtmlWebpackPlugin({
            template: './src/index.html',
            filename: 'index.html',
            minify: {
                removeComments: true,
                collapseWhitespace: true
            }
        }),

        // Extract CSS to separate files
        new MiniCssExtractPlugin({
            filename: '[name].[contenthash].css',
            chunkFilename: '[id].[contenthash].css'
        }),

        // Clean output directory
        new CleanWebpackPlugin(),

        // Define global constants
        new webpack.DefinePlugin({
            'process.env.NODE_ENV': JSON.stringify(process.env.NODE_ENV),
            'process.env.API_URL': JSON.stringify(process.env.API_URL)
        }),

        // Provide global modules
        new webpack.ProvidePlugin({
            $: 'jquery',
            jQuery: 'jquery',
            React: 'react'
        }),

        // Bundle analyzer
        new (require('webpack-bundle-analyzer').BundleAnalyzerPlugin)({
            analyzerMode: 'static',
            openAnalyzer: false
        })
    ]
};
```

**Custom Plugin:**
```javascript
// custom-plugin.js
class CustomPlugin {
    apply(compiler) {
        compiler.hooks.emit.tapAsync('CustomPlugin', (compilation, callback) => {
            // Access compilation assets
            const assets = compilation.assets;

            // Create a new asset
            const manifest = Object.keys(assets).map(filename => ({
                name: filename,
                size: assets[filename].size()
            }));

            // Add manifest to compilation
            compilation.assets['manifest.json'] = {
                source: () => JSON.stringify(manifest, null, 2),
                size: () => JSON.stringify(manifest, null, 2).length
            };

            callback();
        });
    }
}

module.exports = CustomPlugin;
```

### Loaders vs Plugins

**Understanding the difference between loaders and plugins.**

**Loaders:**
```javascript
// Loaders transform individual files
// They work at the module level
// Process files as they're imported

module.exports = {
    module: {
        rules: [
            {
                test: /\.scss$/,
                use: [
                    'style-loader',    // Injects CSS into DOM
                    'css-loader',      // Resolves CSS imports
                    'sass-loader'      // Compiles Sass to CSS
                ]
            }
        ]
    }
};

// Loader chain: sass-loader → css-loader → style-loader
// Each loader receives output from previous loader
```

**Plugins:**
```javascript
// Plugins work at the compilation level
// They can access the entire compilation
// Perform tasks that affect the whole bundle

const HtmlWebpackPlugin = require('html-webpack-plugin');

module.exports = {
    plugins: [
        new HtmlWebpackPlugin({
            template: './src/index.html'
        })
    ]
};

// Plugin hooks into webpack's compilation process
// Can modify assets, add new files, etc.
```

**When to Use Each:**
```
Loaders:
- Transform file content (TypeScript → JavaScript)
- Process imports (CSS, images, fonts)
- Apply transformations (Babel, PostCSS)
- Work with individual modules

Plugins:
- Generate files (HTML, manifest)
- Optimize bundles (minification, compression)
- Define environment variables
- Analyze bundle composition
- Work with entire compilation
```

### Hot Module Replacement (HMR)

**HMR allows updating modules without full page refresh during development.**

**HMR Configuration:**
```javascript
// webpack.config.js
module.exports = {
    mode: 'development',
    devServer: {
        hot: true,           // Enable HMR
        liveReload: false    // Disable live reload to use HMR only
    },
    plugins: [
        new webpack.HotModuleReplacementPlugin() // Usually automatic in dev mode
    ]
};
```

**HMR API Usage:**
```javascript
// main.js
import { render } from './app.js';

render();

// Accept HMR updates for this module
if (module.hot) {
    module.hot.accept('./app.js', () => {
        // Re-import and re-render when app.js changes
        const { render } = require('./app.js');
        render();
    });

    // Accept updates for CSS modules
    module.hot.accept('./styles.css');

    // Handle disposal
    module.hot.dispose((data) => {
        // Clean up before module is replaced
        data.cleanup = true;
    });
}
```

**React HMR:**
```javascript
// Using React Fast Refresh
const ReactRefreshWebpackPlugin = require('@pmmmwh/react-refresh-webpack-plugin');

module.exports = {
    plugins: [
        new ReactRefreshWebpackPlugin()
    ],
    module: {
        rules: [
            {
                test: /\.(js|jsx)$/,
                exclude: /node_modules/,
                use: {
                    loader: 'babel-loader',
                    options: {
                        plugins: [
                            require.resolve('react-refresh/babel')
                        ]
                    }
                }
            }
        ]
    }
};
```

### Core Concepts

**Webpack is a static module bundler for modern JavaScript applications.**

**Key Features:**
- **Module bundling:** Combines multiple files into bundles
- **Code transformation:** Babel, TypeScript, Sass compilation
- **Asset optimization:** Minification, compression, tree shaking
- **Development server:** Hot module replacement, live reloading

**Entry and Output:**
```js
module.exports = {
    entry: './src/index.js',
    output: {
        path: path.resolve(__dirname, 'dist'),
        filename: 'bundle.js'
    }
};
```

### Loaders and Plugins

**Loaders:** Transform files during bundling
```js
module: {
    rules: [
        {
            test: /\.js$/,
            use: 'babel-loader',
            exclude: /node_modules/
        },
        {
            test: /\.css$/,
            use: ['style-loader', 'css-loader']
        }
    ]
}
```

**Plugins:** Extend webpack functionality
```js
plugins: [
    new HtmlWebpackPlugin({
        template: './src/index.html'
    }),
    new MiniCssExtractPlugin({
        filename: '[name].css'
    })
]
```

### Performance Optimization

**Code Splitting:**
```js
// Dynamic imports
import('./module').then(module => {
    // Use module
});

// Split chunks configuration
optimization: {
    splitChunks: {
        chunks: 'all',
        cacheGroups: {
            vendor: {
                test: /[\\/]node_modules[\\/]/,
                name: 'vendors',
                chunks: 'all'
            }
        }
    }
}
```

**Tree Shaking:** Eliminates dead code
**Bundle Analysis:** webpack-bundle-analyzer
**Caching:** Long-term caching with content hashes

### Performance Optimization

**Webpack provides various optimization techniques for production builds.**

**Production Configuration:**
```javascript
const path = require('path');
const MiniCssExtractPlugin = require('mini-css-extract-plugin');
const TerserPlugin = require('terser-webpack-plugin');
const CssMinimizerPlugin = require('css-minimizer-webpack-plugin');

module.exports = {
    mode: 'production',

    optimization: {
        // Minimize JavaScript
        minimize: true,
        minimizer: [
            new TerserPlugin({
                terserOptions: {
                    compress: {
                        drop_console: true, // Remove console.log
                        drop_debugger: true
                    }
                }
            }),
            new CssMinimizerPlugin()
        ],

        // Split chunks
        splitChunks: {
            chunks: 'all',
            cacheGroups: {
                vendor: {
                    test: /[\\/]node_modules[\\/]/,
                    name: 'vendors',
                    chunks: 'all'
                }
            }
        },

        // Runtime chunk
        runtimeChunk: 'single'
    },

    // Source maps for production
    devtool: 'source-map',

    // Performance hints
    performance: {
        maxAssetSize: 250000,
        maxEntrypointSize: 250000,
        hints: 'warning'
    }
};
```

**Tree Shaking:**
```javascript
// Enable tree shaking
module.exports = {
    mode: 'production', // Enables tree shaking automatically

    // Ensure modules are ES6 modules
    module: {
        rules: [
            {
                test: /\.js$/,
                use: {
                    loader: 'babel-loader',
                    options: {
                        presets: [
                            ['@babel/preset-env', {
                                modules: false // Keep ES6 modules for tree shaking
                            }]
                        ]
                    }
                }
            }
        ]
    }
};

// Mark side-effect-free modules in package.json
{
    "sideEffects": false,
    // or specify files with side effects
    "sideEffects": ["*.css", "*.scss", "./src/polyfills.js"]
}

// Use ES6 imports for tree shaking
import { debounce } from 'lodash-es'; // ✅ Tree shakeable
// import _ from 'lodash'; // ❌ Imports entire library
```

**Code Splitting Strategies:**
```javascript
// 1. Entry point splitting
module.exports = {
    entry: {
        main: './src/index.js',
        vendor: './src/vendor.js'
    }
};

// 2. Dynamic imports
async function loadChart() {
    const { Chart } = await import('chart.js');
    return Chart;
}

// 3. SplitChunksPlugin
module.exports = {
    optimization: {
        splitChunks: {
            chunks: 'all',
            minSize: 20000,
            maxSize: 244000,
            cacheGroups: {
                default: {
                    minChunks: 2,
                    priority: -20,
                    reuseExistingChunk: true
                },
                vendor: {
                    test: /[\\/]node_modules[\\/]/,
                    priority: -10,
                    reuseExistingChunk: true
                },
                react: {
                    test: /[\\/]node_modules[\\/](react|react-dom)[\\/]/,
                    name: 'react',
                    chunks: 'all'
                }
            }
        }
    }
};
```

### Build Optimization

**Optimizing build performance and output size.**

**Build Performance:**
```javascript
module.exports = {
    // Cache compilation results
    cache: {
        type: 'filesystem',
        buildDependencies: {
            config: [__filename]
        }
    },

    // Resolve optimizations
    resolve: {
        modules: [path.resolve(__dirname, 'src'), 'node_modules'],
        extensions: ['.js', '.jsx'], // Limit extensions
        alias: {
            '@': path.resolve(__dirname, 'src')
        }
    },

    // Module optimizations
    module: {
        rules: [
            {
                test: /\.js$/,
                include: path.resolve(__dirname, 'src'), // Limit scope
                exclude: /node_modules/,
                use: 'babel-loader'
            }
        ]
    },

    // Parallel processing
    optimization: {
        minimizer: [
            new TerserPlugin({
                parallel: true // Use multiple processes
            })
        ]
    }
};
```

**Bundle Analysis:**
```javascript
const BundleAnalyzerPlugin = require('webpack-bundle-analyzer').BundleAnalyzerPlugin;

module.exports = {
    plugins: [
        new BundleAnalyzerPlugin({
            analyzerMode: 'static',
            reportFilename: 'bundle-report.html',
            openAnalyzer: false
        })
    ]
};

// Command line analysis
// npx webpack-bundle-analyzer dist/static/js/*.js
```

**Asset Optimization:**
```javascript
const ImageMinimizerPlugin = require('image-minimizer-webpack-plugin');

module.exports = {
    optimization: {
        minimizer: [
            new ImageMinimizerPlugin({
                minimizer: {
                    implementation: ImageMinimizerPlugin.imageminMinify,
                    options: {
                        plugins: [
                            ['imagemin-mozjpeg', { quality: 80 }],
                            ['imagemin-pngquant', { quality: [0.6, 0.8] }]
                        ]
                    }
                }
            })
        ]
    },

    module: {
        rules: [
            {
                test: /\.(png|jpe?g|gif)$/,
                type: 'asset',
                parser: {
                    dataUrlCondition: {
                        maxSize: 8 * 1024 // Inline images < 8kb
                    }
                }
            }
        ]
    }
};
```

### Development Proxy

**Configuring proxy for API calls during development.**

**DevServer Proxy:**
```javascript
module.exports = {
    devServer: {
        port: 3000,
        proxy: {
            // Proxy API calls
            '/api': {
                target: 'http://localhost:8080',
                changeOrigin: true,
                pathRewrite: {
                    '^/api': '' // Remove /api prefix
                }
            },

            // Multiple API endpoints
            '/auth': {
                target: 'http://localhost:8081',
                secure: false, // For self-signed certificates
                changeOrigin: true
            },

            // WebSocket proxy
            '/socket.io': {
                target: 'http://localhost:8080',
                ws: true
            },

            // Custom proxy function
            '/custom': {
                target: 'http://localhost:8080',
                bypass: function(req, res, proxyOptions) {
                    if (req.headers.accept.indexOf('html') !== -1) {
                        return '/index.html'; // Serve index.html for HTML requests
                    }
                }
            }
        },

        // CORS headers
        headers: {
            'Access-Control-Allow-Origin': '*',
            'Access-Control-Allow-Methods': 'GET, POST, PUT, DELETE, PATCH, OPTIONS',
            'Access-Control-Allow-Headers': 'X-Requested-With, content-type, Authorization'
        }
    }
};
```

**Environment-specific Configuration:**
```javascript
// webpack.dev.js
const { merge } = require('webpack-merge');
const common = require('./webpack.common.js');

module.exports = merge(common, {
    mode: 'development',
    devtool: 'inline-source-map',
    devServer: {
        static: './dist',
        hot: true,
        proxy: {
            '/api': 'http://localhost:3001'
        }
    }
});

// webpack.prod.js
const { merge } = require('webpack-merge');
const common = require('./webpack.common.js');

module.exports = merge(common, {
    mode: 'production',
    devtool: 'source-map'
});
```

### Alternative Bundlers

**Overview of modern alternatives to webpack.**

**Vite:**
```javascript
// vite.config.js
import { defineConfig } from 'vite';
import react from '@vitejs/plugin-react';

export default defineConfig({
    plugins: [react()],
    server: {
        port: 3000,
        proxy: {
            '/api': 'http://localhost:8080'
        }
    },
    build: {
        outDir: 'dist',
        rollupOptions: {
            output: {
                manualChunks: {
                    vendor: ['react', 'react-dom']
                }
            }
        }
    }
});

// Benefits:
// - Faster dev server (ES modules + esbuild)
// - Hot module replacement out of the box
// - Simpler configuration
// - Built on Rollup for production
```

**Parcel:**
```json
// package.json
{
    "scripts": {
        "start": "parcel src/index.html",
        "build": "parcel build src/index.html"
    }
}

// Benefits:
// - Zero configuration
// - Automatic dependency resolution
// - Built-in dev server
// - Code splitting out of the box
```

**esbuild:**
```javascript
// build.js
const esbuild = require('esbuild');

esbuild.build({
    entryPoints: ['src/index.js'],
    bundle: true,
    outfile: 'dist/bundle.js',
    minify: true,
    sourcemap: true,
    target: ['es2020']
}).catch(() => process.exit(1));

// Benefits:
// - Extremely fast (written in Go)
// - Built-in TypeScript support
// - Tree shaking
// - Minification
```

**Rollup:**
```javascript
// rollup.config.js
import resolve from '@rollup/plugin-node-resolve';
import commonjs from '@rollup/plugin-commonjs';
import { terser } from 'rollup-plugin-terser';

export default {
    input: 'src/index.js',
    output: {
        file: 'dist/bundle.js',
        format: 'iife'
    },
    plugins: [
        resolve(),
        commonjs(),
        terser()
    ]
};

// Benefits:
// - Excellent tree shaking
// - Smaller bundles
// - ES6 modules first
// - Great for libraries
```

**Comparison:**
```
Webpack:
+ Mature ecosystem
+ Extensive plugin system
+ Flexible configuration
- Complex configuration
- Slower build times

Vite:
+ Fast development
+ Simple configuration
+ Modern defaults
- Newer ecosystem
- Different dev/prod bundlers

Parcel:
+ Zero configuration
+ Fast setup
+ Good defaults
- Less flexible
- Smaller ecosystem

esbuild:
+ Extremely fast
+ Simple API
+ Built-in features
- Limited plugins
- Less mature

Rollup:
+ Excellent tree shaking
+ Clean output
+ ES6 focused
- More complex for apps
- Better for libraries
```

---

## Conclusion

This comprehensive guide covers the essential frontend interview topics with practical implementations and real-world applications. Each section provides both theoretical understanding and hands-on code examples that demonstrate proficiency in modern frontend development.

Key areas of focus for interview preparation:
1. **JavaScript fundamentals** - closures, prototypes, async programming
2. **React ecosystem** - hooks, performance, state management
3. **CSS layout techniques** - flexbox, grid, responsive design
4. **Modern JavaScript** - ES6+ features, modules, promises
5. **Web protocols** - HTTP evolution, security, real-time communication
6. **Type safety** - TypeScript interfaces, generics, type system
7. **Build tools** - webpack configuration, optimization, development workflow

Understanding these concepts deeply and being able to implement them practically will provide a strong foundation for frontend development interviews and real-world projects.

---

## Conclusion

This comprehensive guide covers the essential frontend interview topics with practical implementations and real-world applications. Each section provides both theoretical understanding and hands-on code examples that demonstrate proficiency in modern frontend development.

Key areas of focus for interview preparation:
1. **JavaScript fundamentals** - closures, prototypes, async programming
2. **React ecosystem** - hooks, performance, state management
3. **CSS layout techniques** - flexbox, grid, responsive design
4. **Modern JavaScript** - ES6+ features, modules, promises
5. **Web protocols** - HTTP evolution, security, real-time communication
6. **Type safety** - TypeScript interfaces, generics, type system
7. **Build tools** - webpack configuration, optimization, development workflow

Understanding these concepts deeply and being able to implement them practically will provide a strong foundation for frontend development interviews and real-world projects.
