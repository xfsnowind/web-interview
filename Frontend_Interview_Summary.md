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
setTimeout(() => console.log('setTimeout'), 0);
Promise.resolve().then(() => console.log('promise'));
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

---

## React

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

### Component Lifecycle and Performance

**Class Component Lifecycle:**
- **Mounting:** constructor → componentDidMount
- **Updating:** componentDidUpdate
- **Unmounting:** componentWillUnmount

**Hooks Equivalent:**
- `useEffect(() => {}, [])` → componentDidMount
- `useEffect(() => {})` → componentDidUpdate
- `useEffect(() => () => {}, [])` → componentWillUnmount

**Performance Optimization:**
- `React.memo` for component memoization
- `useMemo` for expensive calculations
- `useCallback` for function memoization
- `useRef` for DOM references and mutable values

---

## CSS

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

### Responsive Design

**Key Techniques:**
- **Viewport units:** `vw`, `vh`, `vmin`, `vmax`
- **Relative units:** `em`, `rem`, `%`
- **Media queries:** `@media (max-width: 768px)`
- **Flexible grids:** CSS Grid and Flexbox
- **Fluid images:** `max-width: 100%`

---

## ES6

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
