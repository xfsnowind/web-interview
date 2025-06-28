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

---

## TypeScript

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

---

## Webpack

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
