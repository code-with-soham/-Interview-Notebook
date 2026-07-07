# SECTION 2: JAVASCRIPT (COMPLETE)

# ═══════════════════════════════════════════════════════

---

## 2.1 Execution Context & Call Stack

### ✅ Important Topics

- [ ] Global Execution Context (GEC)
- [ ] Function Execution Context (FEC)
- [ ] Eval Execution Context
- [ ] Creation phase vs Execution phase
- [ ] Variable Environment
- [ ] Lexical Environment
- [ ] Scope Chain
- [ ] Call Stack (LIFO)
- [ ] Stack Overflow
- [ ] Execution Context lifecycle

### 📋 Conceptual Questions

1. What is an Execution Context in JavaScript?
2. What are the types of Execution Context?
3. What happens during the creation phase of an Execution Context?
4. What happens during the execution phase?
5. What is the Global Execution Context? When is it created?
6. What is the Call Stack? How does it work?
7. What is a stack overflow? When does it occur in JavaScript?
8. How does JavaScript handle function calls internally?
9. What is the relationship between the Execution Context and the scope chain?
10. Can you explain how JavaScript executes a program step-by-step using the Execution Context and Call Stack?

### 🖥️ Output Based Questions

11. What is the output?

```js
var a = 10;
function foo() {
  console.log(a);
  var a = 20;
}
foo();
```

12. What is the output?

```js
function a() {
  console.log(1);
}
a();
function a() {
  console.log(2);
}
a();
```

13. What is the output?

```js
console.log(typeof foo);
console.log(typeof bar);
var foo = "hello";
function bar() {
  return "world";
}
```

14. What is the output?

```js
var x = 1;
function outer() {
  var x = 2;
  function inner() {
    console.log(x);
  }
  inner();
}
outer();
```

15. What is the output?

```js
function test() {
  console.log(a);
  console.log(b);
  var a = 1;
  let b = 2;
}
test();
```

---

## 2.2 Memory (Heap & Stack)

### ✅ Important Topics

- [ ] Stack memory (primitives)
- [ ] Heap memory (objects, arrays, functions)
- [ ] Pass by value vs Pass by reference
- [ ] Shallow copy vs Deep copy
- [ ] Garbage collection
- [ ] Mark and Sweep algorithm
- [ ] Memory leaks in JavaScript
- [ ] Reference counting
- [ ] WeakRef and FinalizationRegistry

### 📋 Interview Questions

1. How does JavaScript manage memory?
2. What is the difference between stack and heap memory in JavaScript?
3. Are JavaScript primitives stored on the stack or heap?
4. Is JavaScript pass by value or pass by reference?
5. What is garbage collection in JavaScript?
6. What is the Mark and Sweep algorithm?
7. What are common causes of memory leaks in JavaScript?
8. How do closures affect memory?
9. What is the difference between shallow copy and deep copy?
10. How do you create a deep copy of an object in JavaScript?
11. What is `structuredClone()`?
12. What is `WeakRef`? When would you use it?

### 🖥️ Output Based Questions

13. What is the output?

```js
let a = { name: "John" };
let b = a;
b.name = "Jane";
console.log(a.name);
```

14. What is the output?

```js
let x = 10;
let y = x;
y = 20;
console.log(x);
```

15. What is the output?

```js
let arr1 = [1, 2, 3];
let arr2 = [...arr1];
arr2.push(4);
console.log(arr1.length);
console.log(arr2.length);
```

16. What is the output?

```js
let obj1 = { a: 1, b: { c: 2 } };
let obj2 = { ...obj1 };
obj2.b.c = 3;
console.log(obj1.b.c);
```

---

## 2.3 Hoisting

### ✅ Important Topics

- [ ] Variable hoisting (var, let, const)
- [ ] Function hoisting (declaration vs expression)
- [ ] Class hoisting
- [ ] Hoisting in different scopes
- [ ] Temporal Dead Zone relationship

### 📋 Interview Questions

1. What is hoisting in JavaScript?
2. Are `let` and `const` hoisted?
3. What is the difference between hoisting of `var`, `let`, and `const`?
4. What is the difference between function declaration and function expression hoisting?
5. Are arrow functions hoisted?
6. Are class declarations hoisted?
7. What is the difference between `undefined` and `not defined`?
8. Why does `var` get initialized to `undefined` during hoisting but `let` doesn't?

### 🖥️ Output Based Questions

9. What is the output?

```js
console.log(a);
console.log(b);
console.log(c);
var a = 1;
let b = 2;
const c = 3;
```

10. What is the output?

```js
foo();
bar();
function foo() {
  console.log("foo");
}
var bar = function () {
  console.log("bar");
};
```

11. What is the output?

```js
var x = 1;
function x() {}
console.log(typeof x);
```

12. What is the output?

```js
console.log(foo);
var foo = 10;
function foo() {
  return 20;
}
console.log(foo);
```

13. What is the output?

```js
var a = 1;
function outer() {
  console.log(a);
  if (false) {
    var a = 2;
  }
}
outer();
```

14. What is the output?

```js
function test() {
  console.log(typeof a);
  console.log(typeof b);
  let a = 10;
  var b = 20;
}
test();
```

---

## 2.4 Temporal Dead Zone (TDZ)

### ✅ Important Topics

- [ ] What is TDZ
- [ ] TDZ with let and const
- [ ] TDZ in different scopes
- [ ] TDZ with default parameters
- [ ] ReferenceError vs undefined

### 📋 Interview Questions

1. What is the Temporal Dead Zone?
2. Which variables are affected by TDZ?
3. What error do you get when accessing a variable in the TDZ?
4. How is TDZ different from hoisting?
5. Does TDZ apply to function parameters?
6. Can TDZ occur inside a block scope?

### 🖥️ Output Based Questions

7. What is the output?

```js
let a = 10;
{
  console.log(a);
  let a = 20;
}
```

8. What is the output?

```js
const x = 10;
{
  console.log(x);
  const x = 20;
}
```

9. What is the output?

```js
function foo(a = b, b = 1) {
  console.log(a, b);
}
foo();
```

10. What is the output?

```js
console.log(typeof undeclaredVar);
console.log(typeof letVar);
let letVar = 10;
```

---

## 2.5 Closures

### ✅ Important Topics

- [ ] Definition and how closures work
- [ ] Lexical scoping
- [ ] Closure with loops
- [ ] Closure use cases (data privacy, currying, memoization)
- [ ] IIFE and closures
- [ ] Memory implications of closures
- [ ] Module pattern using closures
- [ ] Closure vs Block scope

### 📋 Interview Questions

1. What is a closure in JavaScript?
2. How do closures work internally?
3. What is the relationship between closures and lexical scope?
4. How do closures help in data encapsulation/privacy?
5. What is the classic closure problem with `var` in a loop?
6. How do you solve the closure-in-loop problem?
7. What are the advantages and disadvantages of closures?
8. How do closures affect garbage collection?
9. What is the module pattern? How does it use closures?
10. Can closures cause memory leaks? How?

### 🖥️ Output Based Questions

11. What is the output?

```js
function outer() {
  let count = 0;
  return function inner() {
    count++;
    console.log(count);
  };
}
const fn = outer();
fn();
fn();
fn();
```

12. What is the output?

```js
for (var i = 0; i < 3; i++) {
  setTimeout(function () {
    console.log(i);
  }, 1000);
}
```

13. What is the output?

```js
for (let i = 0; i < 3; i++) {
  setTimeout(function () {
    console.log(i);
  }, 1000);
}
```

14. What is the output?

```js
function createMultiplier(x) {
  return function (y) {
    return x * y;
  };
}
const double = createMultiplier(2);
const triple = createMultiplier(3);
console.log(double(5));
console.log(triple(5));
```

15. What is the output?

```js
function outer() {
  var a = 10;
  function inner() {
    console.log(a);
  }
  a = 20;
  return inner;
}
outer()();
```

16. What is the output?

```js
var result = [];
for (var i = 0; i < 5; i++) {
  result.push(
    (function (j) {
      return function () {
        return j;
      };
    })(i),
  );
}
console.log(result[2]());
console.log(result[4]());
```

### 💻 Coding Questions

17. Create a counter function using closures that has increment, decrement, and getCount methods.
18. Implement a private variable pattern using closures.
19. Create a memoize function using closures.
20. Implement a once() function that only allows a function to be called once.
21. Create a function that generates unique IDs using closures.
22. Implement a rate limiter using closures.

---

## 2.6 Lexical Scope

### ✅ Important Topics

- [ ] Lexical (static) scoping
- [ ] Dynamic scoping (concept)
- [ ] Scope chain
- [ ] Block scope
- [ ] Function scope
- [ ] Global scope
- [ ] Module scope

### 📋 Interview Questions

1. What is lexical scope in JavaScript?
2. What is the difference between lexical scope and dynamic scope?
3. What is the scope chain? How does JavaScript resolve variables?
4. What is the difference between block scope and function scope?
5. What is the scope of `var`, `let`, and `const`?
6. What is module scope?
7. Can inner functions access outer function variables? Why?
8. Can outer functions access inner function variables? Why not?

### 🖥️ Output Based Questions

9. What is the output?

```js
var x = 10;
function foo() {
  var x = 20;
  function bar() {
    console.log(x);
  }
  bar();
}
foo();
```

10. What is the output?

```js
function outer() {
  let a = 1;
  function middle() {
    let b = 2;
    function inner() {
      let c = 3;
      console.log(a + b + c);
    }
    inner();
  }
  middle();
}
outer();
```

---

## 2.7 `this` Keyword

### ✅ Important Topics

- [ ] `this` in global context
- [ ] `this` in function context (strict vs non-strict)
- [ ] `this` in object methods
- [ ] `this` in arrow functions
- [ ] `this` in event handlers
- [ ] `this` in class constructors
- [ ] `this` in callbacks
- [ ] `call()`, `apply()`, `bind()`
- [ ] Implicit binding, Explicit binding, `new` binding, Default binding
- [ ] Binding precedence

### 📋 Interview Questions

1. What is the `this` keyword in JavaScript?
2. What is `this` in the global context?
3. What is `this` inside a regular function in strict mode vs non-strict mode?
4. How does `this` work in object methods?
5. How does `this` behave in arrow functions?
6. What is the difference between `call()`, `apply()`, and `bind()`?
7. What is implicit binding?
8. What is explicit binding?
9. What is `new` binding?
10. What is the binding precedence of `this`?
11. How do you fix `this` losing context in callbacks?
12. What is `this` inside a class constructor?
13. What is `this` inside an event handler?

### 🖥️ Output Based Questions

14. What is the output?

```js
const obj = {
  name: "Alice",
  greet: function () {
    console.log(this.name);
  },
};
obj.greet();
const fn = obj.greet;
fn();
```

15. What is the output?

```js
const obj = {
  name: "Bob",
  greet: () => {
    console.log(this.name);
  },
};
obj.greet();
```

16. What is the output?

```js
const obj = {
  name: "Charlie",
  greet: function () {
    const inner = () => {
      console.log(this.name);
    };
    inner();
  },
};
obj.greet();
```

17. What is the output?

```js
function greet() {
  console.log(this.name);
}
const obj1 = { name: "A" };
const obj2 = { name: "B" };
greet.call(obj1);
greet.apply(obj2);
const bound = greet.bind(obj1);
bound.call(obj2);
```

18. What is the output?

```js
const obj = {
  x: 10,
  getX: function () {
    return this.x;
  },
};
const getX = obj.getX;
console.log(getX());
console.log(obj.getX());
```

19. What is the output?

```js
function Person(name) {
  this.name = name;
  this.greet = function () {
    setTimeout(function () {
      console.log(this.name);
    }, 100);
  };
}
const p = new Person("Dave");
p.greet();
```

20. What is the output?

```js
function Person(name) {
  this.name = name;
  this.greet = function () {
    setTimeout(() => {
      console.log(this.name);
    }, 100);
  };
}
const p = new Person("Eve");
p.greet();
```

### 💻 Coding Questions

21. Implement your own `call()` method (polyfill).
22. Implement your own `apply()` method (polyfill).
23. Implement your own `bind()` method (polyfill).

---

## 2.8 Arrow Functions

### ✅ Important Topics

- [ ] Arrow function syntax
- [ ] Implicit return
- [ ] No own `this`
- [ ] No `arguments` object
- [ ] Cannot be used as constructors
- [ ] No `prototype` property
- [ ] Arrow functions vs regular functions
- [ ] When NOT to use arrow functions

### 📋 Interview Questions

1. What are arrow functions in JavaScript?
2. What is implicit return in arrow functions?
3. Why don't arrow functions have their own `this`?
4. Can you use `arguments` inside an arrow function?
5. Can you use an arrow function as a constructor with `new`?
6. When should you NOT use arrow functions?
7. Do arrow functions have a `prototype` property?
8. What is the difference between `() => {}` and `() => ({})`?

### 🖥️ Output Based Questions

9. What is the output?

```js
const add = (a, b) => a + b;
console.log(add(2, 3));
console.log(add.prototype);
```

10. What is the output?

```js
const ArrowFunc = () => {};
const obj = new ArrowFunc();
```

11. What is the output?

```js
const obj = {
  value: 42,
  getValue: () => this.value,
  getValueRegular: function () {
    return this.value;
  },
};
console.log(obj.getValue());
console.log(obj.getValueRegular());
```

---

## 2.9 Prototype & Prototype Chain

### ✅ Important Topics

- [ ] `__proto__` vs `prototype`
- [ ] Prototype chain
- [ ] Object.create()
- [ ] Object.getPrototypeOf()
- [ ] Object.setPrototypeOf()
- [ ] hasOwnProperty()
- [ ] instanceof operator
- [ ] Constructor functions
- [ ] Prototype-based inheritance
- [ ] Property shadowing
- [ ] Prototype pollution

### 📋 Interview Questions

1. What is a prototype in JavaScript?
2. What is the difference between `__proto__` and `prototype`?
3. What is the prototype chain?
4. How does JavaScript look up properties on an object?
5. What is `Object.create()`? How does it work?
6. What does `hasOwnProperty()` do?
7. What is the `instanceof` operator?
8. What is prototype pollution? How do you prevent it?
9. How does inheritance work in JavaScript using prototypes?
10. What is at the top of the prototype chain?

### 🖥️ Output Based Questions

11. What is the output?

```js
function Animal(name) {
  this.name = name;
}
Animal.prototype.speak = function () {
  return this.name + " makes a sound";
};
const dog = new Animal("Dog");
console.log(dog.speak());
console.log(dog.hasOwnProperty("name"));
console.log(dog.hasOwnProperty("speak"));
```

12. What is the output?

```js
const obj = {};
console.log(obj.__proto__ === Object.prototype);
console.log(Object.prototype.__proto__);
```

13. What is the output?

```js
function Foo() {}
Foo.prototype.x = 10;
const a = new Foo();
const b = new Foo();
a.x = 20;
console.log(a.x);
console.log(b.x);
delete a.x;
console.log(a.x);
```

14. What is the output?

```js
console.log([] instanceof Array);
console.log([] instanceof Object);
console.log({} instanceof Array);
```

---

## 2.10 Classes & Inheritance (ES6)

### ✅ Important Topics

- [ ] Class declaration and expression
- [ ] Constructor
- [ ] Methods
- [ ] Static methods and properties
- [ ] Getters and Setters
- [ ] Private fields (#)
- [ ] extends and super
- [ ] Method overriding
- [ ] Class vs constructor function
- [ ] Abstract class pattern in JS
- [ ] Mixins

### 📋 Interview Questions

1. What are classes in JavaScript? Are they syntactic sugar?
2. What is the difference between a class and a constructor function?
3. What is the `constructor` method in a class?
4. What are static methods? How do you define them?
5. What are private fields in JavaScript? How do you declare them?
6. How does inheritance work with classes?
7. What is the `super` keyword? When do you use it?
8. Can you create an instance of a class without `new`?
9. What are getters and setters in JavaScript classes?
10. What are mixins? How do you implement them?
11. Can you have multiple constructors in a JavaScript class?
12. What is the difference between `Object.create()` and `new ClassName()`?

### 🖥️ Output Based Questions

13. What is the output?

```js
class Animal {
  constructor(name) {
    this.name = name;
  }
  speak() {
    return `${this.name} makes a noise`;
  }
}
class Dog extends Animal {
  speak() {
    return `${this.name} barks`;
  }
}
const d = new Dog("Rex");
console.log(d.speak());
console.log(d instanceof Animal);
```

14. What is the output?

```js
class Counter {
  #count = 0;
  increment() {
    this.#count++;
  }
  getCount() {
    return this.#count;
  }
}
const c = new Counter();
c.increment();
c.increment();
console.log(c.getCount());
console.log(c.#count);
```

15. What is the output?

```js
class Parent {
  static greet() {
    return "Hello from Parent";
  }
}
class Child extends Parent {}
console.log(Child.greet());
```

---

## 2.11 Promises

### ✅ Important Topics

- [ ] Promise states (pending, fulfilled, rejected)
- [ ] Promise constructor
- [ ] .then(), .catch(), .finally()
- [ ] Promise chaining
- [ ] Promise.all()
- [ ] Promise.allSettled()
- [ ] Promise.race()
- [ ] Promise.any()
- [ ] Promise.resolve() and Promise.reject()
- [ ] Error handling in promises
- [ ] Microtask queue relationship
- [ ] Promise anti-patterns

### 📋 Interview Questions

1. What is a Promise in JavaScript?
2. What are the three states of a Promise?
3. What is the difference between `.then()` and `.catch()`?
4. What is Promise chaining?
5. What is the difference between `Promise.all()` and `Promise.allSettled()`?
6. What is `Promise.race()`?
7. What is `Promise.any()`? How is it different from `Promise.race()`?
8. What happens if you don't handle a rejected Promise?
9. Can a Promise be resolved more than once?
10. What is `.finally()`? When is it called?
11. How do Promises relate to the microtask queue?
12. What is a Promise anti-pattern? Give examples.

### 🖥️ Output Based Questions

13. What is the output?

```js
const p = new Promise((resolve, reject) => {
  console.log(1);
  resolve(2);
  console.log(3);
});
p.then((val) => console.log(val));
console.log(4);
```

14. What is the output?

```js
Promise.resolve(1)
  .then((x) => x + 1)
  .then((x) => {
    throw new Error("error");
  })
  .then((x) => console.log(x))
  .catch((err) => console.log("caught"))
  .then((x) => console.log("after catch"));
```

15. What is the output?

```js
const p1 = Promise.resolve("A");
const p2 = new Promise((resolve) => setTimeout(() => resolve("B"), 1000));
const p3 = Promise.reject("C");

Promise.all([p1, p2, p3])
  .then((values) => console.log(values))
  .catch((err) => console.log("Error:", err));
```

16. What is the output?

```js
Promise.race([
  new Promise((resolve) => setTimeout(() => resolve("slow"), 2000)),
  new Promise((resolve) => setTimeout(() => resolve("fast"), 500)),
]).then((val) => console.log(val));
```

17. What is the output?

```js
console.log("start");
Promise.resolve().then(() => console.log("promise"));
console.log("end");
```

18. What is the output?

```js
const p = new Promise((resolve, reject) => {
  resolve("first");
  resolve("second");
  reject("error");
});
p.then((val) => console.log(val)).catch((err) => console.log(err));
```

### 💻 Coding Questions

19. Implement a simple Promise class from scratch (basic resolve/then).
20. Implement `Promise.all()` polyfill.
21. Implement `Promise.allSettled()` polyfill.
22. Implement `Promise.race()` polyfill.
23. Implement `Promise.any()` polyfill.
24. Implement a retry function using Promises.
25. Implement a timeout wrapper for Promises.
26. Implement sequential execution of Promises.

---

## 2.12 Async/Await

### ✅ Important Topics

- [ ] async function declaration
- [ ] await keyword
- [ ] Error handling with try/catch
- [ ] Async/await vs Promises
- [ ] Parallel execution with async/await
- [ ] Top-level await
- [ ] Sequential vs concurrent async operations
- [ ] async IIFE

### 📋 Interview Questions

1. What is `async/await` in JavaScript?
2. What does the `async` keyword do to a function?
3. What does `await` do?
4. How do you handle errors with `async/await`?
5. What is the difference between `async/await` and Promises?
6. Can you use `await` outside an `async` function?
7. How do you run multiple async operations in parallel?
8. What happens if you don't `await` an async function call?
9. What is the return type of an async function?
10. Can you use `await` with `Promise.all()`?

### 🖥️ Output Based Questions

11. What is the output?

```js
async function foo() {
  console.log(1);
  await Promise.resolve();
  console.log(2);
}
console.log(3);
foo();
console.log(4);
```

12. What is the output?

```js
async function foo() {
  return "hello";
}
foo().then((val) => console.log(val));
console.log("world");
```

13. What is the output?

```js
async function test() {
  try {
    const result = await Promise.reject("error");
    console.log(result);
  } catch (e) {
    console.log("caught:", e);
  }
}
test();
```

14. What is the output and in what order?

```js
async function one() {
  console.log("A");
  await two();
  console.log("B");
}
async function two() {
  console.log("C");
}
console.log("D");
one();
console.log("E");
```

### 💻 Coding Questions

15. Write an async function that fetches data from an API with retry logic.
16. Implement sequential and parallel async operations.
17. Create a sleep() function using async/await.
18. Implement an async queue that processes tasks one at a time.

---

## 2.13 Callbacks & Callback Hell

### ✅ Important Topics

- [ ] Callback functions
- [ ] Higher-order functions
- [ ] Synchronous vs Asynchronous callbacks
- [ ] Callback hell (Pyramid of Doom)
- [ ] Inversion of control
- [ ] Error-first callback pattern
- [ ] How Promises solve callback hell

### 📋 Interview Questions

1. What is a callback function?
2. What is a higher-order function?
3. What is the difference between synchronous and asynchronous callbacks?
4. What is callback hell? Why is it a problem?
5. What is inversion of control?
6. What is the error-first callback pattern?
7. How do Promises solve the callback hell problem?
8. Give examples of built-in functions that accept callbacks.
9. What problems can arise from deeply nested callbacks?

### 🖥️ Output Based Questions

10. What is the output?

```js
function greet(name, callback) {
  console.log("Hello " + name);
  callback();
}
greet("Alice", function () {
  console.log("Callback executed");
});
```

11. What is the output?

```js
[1, 2, 3].forEach(function (item) {
  console.log(item);
});
console.log("done");
```

### 💻 Coding Questions

12. Refactor a nested callback pattern into Promise-based code.
13. Refactor callback-based code into async/await.
14. Implement a function that executes an array of async callbacks in series.

---

## 2.14 Microtask Queue & Macrotask Queue

### ✅ Important Topics

- [ ] Microtasks (Promise callbacks, queueMicrotask, MutationObserver)
- [ ] Macrotasks (setTimeout, setInterval, setImmediate, I/O, UI rendering)
- [ ] Execution priority (microtasks before macrotasks)
- [ ] Starvation
- [ ] requestAnimationFrame

### 📋 Interview Questions

1. What is the difference between microtasks and macrotasks?
2. Give examples of microtasks.
3. Give examples of macrotasks.
4. Which has higher priority — microtasks or macrotasks?
5. What is `queueMicrotask()`?
6. What is starvation in the context of microtasks?
7. Where does `requestAnimationFrame` fit in the task queue?
8. What happens if a microtask queues another microtask?

### 🖥️ Output Based Questions (CRITICAL — asked in every interview)

9. What is the output?

```js
console.log("1");
setTimeout(() => console.log("2"), 0);
Promise.resolve().then(() => console.log("3"));
console.log("4");
```

10. What is the output?

```js
setTimeout(() => console.log("A"), 0);
Promise.resolve().then(() => console.log("B"));
Promise.resolve().then(() => setTimeout(() => console.log("C"), 0));
Promise.resolve().then(() => console.log("D"));
setTimeout(() => console.log("E"), 0);
console.log("F");
```

11. What is the output?

```js
console.log("start");
setTimeout(() => console.log("timeout 1"), 0);
Promise.resolve().then(() => {
  console.log("promise 1");
  setTimeout(() => console.log("timeout 2"), 0);
});
Promise.resolve().then(() => console.log("promise 2"));
setTimeout(() => console.log("timeout 3"), 0);
console.log("end");
```

12. What is the output?

```js
async function async1() {
  console.log("async1 start");
  await async2();
  console.log("async1 end");
}
async function async2() {
  console.log("async2");
}
console.log("script start");
setTimeout(() => console.log("setTimeout"), 0);
async1();
new Promise((resolve) => {
  console.log("promise1");
  resolve();
}).then(() => console.log("promise2"));
console.log("script end");
```

13. What is the output?

```js
queueMicrotask(() => console.log("microtask"));
setTimeout(() => console.log("timeout"), 0);
Promise.resolve().then(() => console.log("promise"));
console.log("sync");
```

---

## 2.15 Event Loop

### ✅ Important Topics

- [ ] How the Event Loop works
- [ ] Call Stack
- [ ] Web APIs
- [ ] Callback Queue (Task Queue)
- [ ] Microtask Queue
- [ ] Render Queue
- [ ] Event Loop phases
- [ ] Non-blocking I/O
- [ ] Single-threaded nature of JavaScript
- [ ] setTimeout(fn, 0) behavior

### 📋 Interview Questions

1. What is the Event Loop in JavaScript?
2. How does the Event Loop work step by step?
3. Why is JavaScript single-threaded?
4. What are Web APIs? Give examples.
5. What is the Callback Queue?
6. What is the difference between the Callback Queue and the Microtask Queue?
7. What is `setTimeout(fn, 0)`? Does it execute immediately?
8. What is the minimum delay for `setTimeout`?
9. How does `setInterval` work with the Event Loop?
10. What is the relationship between the Event Loop and rendering?
11. Can the Event Loop be blocked? How?
12. What happens when the Call Stack is not empty and there are tasks in the queue?

### 🎯 Scenario Based Questions

13. A user clicks a button and the callback takes 5 seconds to execute. What happens to other events during this time?
14. You have a heavy computation in JavaScript. How do you prevent it from blocking the UI?
15. Explain step by step what happens when you execute a `fetch()` request in the browser.

---

## 2.16 Map, Set, WeakMap, WeakSet

### ✅ Important Topics

- [ ] Map vs Object
- [ ] Map methods (set, get, has, delete, clear, size)
- [ ] Map iteration
- [ ] Set vs Array
- [ ] Set methods (add, has, delete, clear, size)
- [ ] WeakMap (keys must be objects, garbage collectible)
- [ ] WeakSet (values must be objects, garbage collectible)
- [ ] Use cases for each

### 📋 Interview Questions

1. What is a `Map` in JavaScript? How is it different from a plain object?
2. What are the advantages of `Map` over a plain object?
3. Can a `Map` have non-string keys?
4. What is a `Set`? How is it different from an array?
5. What is a `WeakMap`? When would you use it?
6. What is a `WeakSet`? When would you use it?
7. Why are `WeakMap` and `WeakSet` not iterable?
8. What happens to entries in a `WeakMap` when the key object is garbage collected?
9. What are practical use cases for `WeakMap`?
10. What is the difference between `Map.size` and `Object.keys(obj).length`?

### 💻 Coding Questions

11. Remove duplicates from an array using `Set`.
12. Implement a cache using `Map`.
13. Find the first non-repeating character using `Map`.
14. Implement an object metadata store using `WeakMap`.
15. Count word frequency using `Map`.

---

## 2.17 Array Methods

### ✅ Important Topics

- [ ] map(), filter(), reduce()
- [ ] forEach(), find(), findIndex()
- [ ] some(), every()
- [ ] includes(), indexOf()
- [ ] flat(), flatMap()
- [ ] sort(), reverse()
- [ ] splice(), slice()
- [ ] push(), pop(), shift(), unshift()
- [ ] concat(), join()
- [ ] Array.from(), Array.of(), Array.isArray()
- [ ] fill(), copyWithin()
- [ ] entries(), keys(), values()
- [ ] at()

### 📋 Interview Questions

1. What is the difference between `map()` and `forEach()`?
2. What is the difference between `map()` and `filter()`?
3. How does `reduce()` work?
4. What is the difference between `find()` and `filter()`?
5. What is the difference between `some()` and `every()`?
6. What is the difference between `splice()` and `slice()`?
7. What is the difference between `indexOf()` and `includes()`?
8. How does `sort()` work in JavaScript? What is the default sorting behavior?
9. What is `flat()`? What does `flat(Infinity)` do?
10. What is `flatMap()`?
11. Does `map()` mutate the original array?
12. Which array methods mutate the original array?
13. What is `Array.from()`? Give use cases.

### 🖥️ Output Based Questions

14. What is the output?

```js
const arr = [1, 2, 3, 4, 5];
const result = arr
  .map((x) => x * 2)
  .filter((x) => x > 4)
  .reduce((acc, x) => acc + x, 0);
console.log(result);
```

15. What is the output?

```js
const arr = [3, 1, 4, 1, 5, 9];
console.log(arr.sort());
console.log(arr.sort((a, b) => a - b));
```

16. What is the output?

```js
const arr = [1, [2, [3, [4]]]];
console.log(arr.flat());
console.log(arr.flat(Infinity));
```

17. What is the output?

```js
const arr = [1, 2, 3];
arr.splice(1, 1, "a", "b");
console.log(arr);
```

### 💻 Coding Questions

18. Implement `map()` polyfill.
19. Implement `filter()` polyfill.
20. Implement `reduce()` polyfill.
21. Implement `flat()` polyfill.
22. Implement `forEach()` polyfill.
23. Implement `find()` polyfill.

---

## 2.18 Debouncing & Throttling

### ✅ Important Topics

- [ ] Debouncing concept
- [ ] Throttling concept
- [ ] Difference between debouncing and throttling
- [ ] Leading vs trailing edge
- [ ] Use cases (search, scroll, resize, button click)
- [ ] Implementation using closures and setTimeout

### 📋 Interview Questions

1. What is debouncing?
2. What is throttling?
3. What is the difference between debouncing and throttling?
4. When would you use debouncing vs throttling?
5. What are real-world use cases for debouncing?
6. What are real-world use cases for throttling?
7. What is the difference between leading edge and trailing edge debounce?

### 💻 Coding Questions (MOST ASKED)

8. Implement a debounce function from scratch.
9. Implement a throttle function from scratch.
10. Implement a debounce with leading edge option.
11. Implement a debounce with cancel functionality.
12. Implement a throttle with trailing edge execution.
13. Implement a debounced search input handler.

---

## 2.19 Modules (ES6+ and CommonJS)

### ✅ Important Topics

- [ ] ES6 Modules (import/export)
- [ ] CommonJS Modules (require/module.exports)
- [ ] Default export vs Named export
- [ ] Dynamic imports
- [ ] Module bundling
- [ ] Tree shaking
- [ ] Circular dependencies
- [ ] Module scope

### 📋 Interview Questions

1. What are JavaScript modules?
2. What is the difference between ES6 modules and CommonJS modules?
3. What is the difference between default export and named export?
4. Can you have multiple default exports in a module?
5. What is dynamic import? When would you use it?
6. What is tree shaking?
7. What happens with circular dependencies in modules?
8. What is the difference between `import` and `require`?
9. Are ES6 modules synchronous or asynchronous?
10. What is the `type="module"` attribute in `<script>` tags?

---

## 2.20 ES6+ Features

### ✅ Important Topics

- [ ] let, const (block scoping)
- [ ] Template literals
- [ ] Destructuring (arrays and objects)
- [ ] Spread operator (...)
- [ ] Rest parameters
- [ ] Default parameters
- [ ] Optional chaining (?.)
- [ ] Nullish coalescing (??)
- [ ] Logical assignment (||=, &&=, ??=)
- [ ] Short circuit evaluation
- [ ] Symbol
- [ ] for...of vs for...in
- [ ] Tagged template literals
- [ ] Object shorthand
- [ ] Computed property names
- [ ] Object.assign()
- [ ] Object.entries(), Object.keys(), Object.values()
- [ ] Object.freeze(), Object.seal()
- [ ] Proxy and Reflect
- [ ] globalThis

### 📋 Interview Questions

1. What is the difference between `let`, `const`, and `var`?
2. What are template literals? What are tagged template literals?
3. What is destructuring? Give examples with arrays and objects.
4. What is the spread operator? How is it different from rest parameters?
5. What are default parameters?
6. What is optional chaining (`?.`)? Why is it useful?
7. What is nullish coalescing (`??`)? How is it different from `||`?
8. What is a Symbol? When would you use it?
9. What is the difference between `for...in` and `for...of`?
10. What is `Object.freeze()`? Is it deep or shallow?
11. What is the difference between `Object.freeze()` and `Object.seal()`?
12. What is short circuit evaluation?
13. What is a Proxy in JavaScript?
14. What are logical assignment operators?
15. What is `Object.assign()`? Does it deep copy?

### 🖥️ Output Based Questions

16. What is the output?

```js
const [a, , b, ...rest] = [1, 2, 3, 4, 5];
console.log(a, b, rest);
```

17. What is the output?

```js
const { name: n, age: a = 25 } = { name: "Alice" };
console.log(n, a);
```

18. What is the output?

```js
const obj = Object.freeze({ a: 1, b: { c: 2 } });
obj.a = 10;
obj.b.c = 20;
console.log(obj.a, obj.b.c);
```

19. What is the output?

```js
console.log(null ?? "default");
console.log(undefined ?? "default");
console.log(0 ?? "default");
console.log("" ?? "default");
console.log(0 || "default");
console.log("" || "default");
```

20. What is the output?

```js
const user = { address: { street: null } };
console.log(user?.address?.street);
console.log(user?.contact?.phone);
console.log(user?.address?.street?.length);
```

---

## 2.21 Currying

### ✅ Important Topics

- [ ] Function currying concept
- [ ] Partial application
- [ ] Currying vs Partial application
- [ ] Infinite currying
- [ ] Use cases

### 📋 Interview Questions

1. What is currying in JavaScript?
2. What is the difference between currying and partial application?
3. What are the advantages of currying?
4. Where is currying used in real-world applications?

### 💻 Coding Questions (FREQUENTLY ASKED)

5. Convert `f(a, b, c)` into `f(a)(b)(c)`.
6. Implement a generic curry function that works for any number of arguments.
7. Implement infinite currying: `add(1)(2)(3)...(n)()`.
8. Implement `sum(1)(2)(3)` that returns 6 and `sum(1)(2)(3).valueOf()` that returns 6.
9. Create a curried version of `multiply(a, b, c)`.

### 🖥️ Output Based Questions

10. What is the output?

```js
function add(a) {
  return function (b) {
    return function (c) {
      return a + b + c;
    };
  };
}
console.log(add(1)(2)(3));
```

---

## 2.22 Memoization

### ✅ Important Topics

- [ ] Memoization concept
- [ ] Cache strategy
- [ ] Memoization with closures
- [ ] Memoization for recursive functions
- [ ] Cache invalidation
- [ ] WeakMap for memoization

### 📋 Interview Questions

1. What is memoization?
2. How does memoization improve performance?
3. When should you use memoization?
4. What data structure would you use for the cache?
5. How is memoization different from caching?

### 💻 Coding Questions

6. Implement a generic memoize function.
7. Memoize a Fibonacci function.
8. Implement memoize that handles multiple arguments.
9. Implement memoize with cache expiration.
10. Implement memoize using WeakMap for object arguments.

---

## 2.23 Generators & Iterators

### ✅ Important Topics

- [ ] Iterator protocol (next(), value, done)
- [ ] Iterable protocol (Symbol.iterator)
- [ ] Generator functions (function\*)
- [ ] yield keyword
- [ ] Generator delegation (yield\*)
- [ ] Infinite sequences
- [ ] Lazy evaluation
- [ ] for...of with iterators
- [ ] Async generators (async function\*)

### 📋 Interview Questions

1. What is an iterator in JavaScript?
2. What is the iterator protocol?
3. What makes an object iterable?
4. What is a generator function?
5. What does the `yield` keyword do?
6. What is the difference between `return` and `yield`?
7. What is `yield*`?
8. What are async generators?
9. What are use cases for generators?
10. How do you create a custom iterable?

### 🖥️ Output Based Questions

11. What is the output?

```js
function* gen() {
  yield 1;
  yield 2;
  yield 3;
}
const g = gen();
console.log(g.next());
console.log(g.next());
console.log(g.next());
console.log(g.next());
```

12. What is the output?

```js
function* gen() {
  const x = yield "first";
  console.log("x:", x);
  const y = yield "second";
  console.log("y:", y);
}
const g = gen();
console.log(g.next());
console.log(g.next(10));
console.log(g.next(20));
```

### 💻 Coding Questions

13. Create an infinite Fibonacci sequence using a generator.
14. Implement a range function using generators.
15. Create a custom iterable for a linked list.

---

## 2.24 DOM (Document Object Model)

### ✅ Important Topics

- [ ] DOM tree structure
- [ ] Selecting elements (getElementById, querySelector, querySelectorAll)
- [ ] Creating elements
- [ ] Modifying elements (textContent, innerHTML, setAttribute)
- [ ] Adding/removing elements
- [ ] DOM traversal (parentNode, childNodes, nextSibling, previousSibling)
- [ ] classList API
- [ ] Dataset API
- [ ] DocumentFragment
- [ ] Shadow DOM
- [ ] DOM vs Virtual DOM
- [ ] Reflow and Repaint

### 📋 Interview Questions

1. What is the DOM?
2. What is the difference between the DOM and HTML?
3. What is the difference between `getElementById()` and `querySelector()`?
4. What is the difference between `innerHTML` and `textContent`?
5. What is the difference between `createElement` and `innerHTML` for adding elements?
6. What is a `DocumentFragment`? Why is it useful?
7. What is the difference between `appendChild` and `append`?
8. What is reflow? What is repaint?
9. How do you minimize DOM manipulation for better performance?
10. What is the Shadow DOM?
11. What is the difference between DOM and Virtual DOM?
12. What is `dataset`?

---

## 2.25 Browser Rendering

### ✅ Important Topics

- [ ] Critical Rendering Path
- [ ] DOM construction
- [ ] CSSOM construction
- [ ] Render Tree
- [ ] Layout (Reflow)
- [ ] Paint (Repaint)
- [ ] Compositing
- [ ] script tag (async, defer)
- [ ] DOMContentLoaded vs load event
- [ ] requestAnimationFrame
- [ ] requestIdleCallback

### 📋 Interview Questions

1. What is the Critical Rendering Path?
2. What steps does the browser take to render a page?
3. What is the Render Tree? How is it different from the DOM tree?
4. What is the difference between reflow and repaint?
5. What triggers reflow? What triggers repaint?
6. What is the difference between `async` and `defer` in script tags?
7. What is the difference between `DOMContentLoaded` and `load` event?
8. What is `requestAnimationFrame`? When should you use it?
9. What is compositing?
10. How do you optimize rendering performance?
11. What is layout thrashing? How do you avoid it?

---

## 2.26 Virtual DOM & Shadow DOM

### ✅ Important Topics

- [ ] Virtual DOM concept
- [ ] Diffing algorithm
- [ ] Reconciliation
- [ ] Why Virtual DOM is faster
- [ ] Shadow DOM and encapsulation
- [ ] Shadow DOM vs Virtual DOM
- [ ] Web Components

### 📋 Interview Questions

1. What is the Virtual DOM?
2. How does the Virtual DOM work?
3. What is the diffing algorithm?
4. Is the Virtual DOM always faster than the real DOM?
5. What is the Shadow DOM?
6. What is the difference between Virtual DOM and Shadow DOM?
7. What are Web Components?
8. What is reconciliation in React?

---

## 2.27 Storage (localStorage, sessionStorage, Cookies)

### ✅ Important Topics

- [ ] localStorage
- [ ] sessionStorage
- [ ] Cookies
- [ ] IndexedDB
- [ ] Storage limits
- [ ] Security considerations
- [ ] Same-origin policy for storage
- [ ] Cookie attributes (HttpOnly, Secure, SameSite, Path, Domain, Expires)

### 📋 Interview Questions

1. What is `localStorage`?
2. What is `sessionStorage`?
3. What is the difference between `localStorage` and `sessionStorage`?
4. What are cookies? How do they work?
5. What is the difference between cookies and `localStorage`?
6. What is the storage limit for `localStorage`, `sessionStorage`, and cookies?
7. Can JavaScript access `HttpOnly` cookies?
8. What is the `SameSite` attribute in cookies?
9. What is `IndexedDB`? When would you use it?
10. How do you store objects in `localStorage`?
11. What happens to `sessionStorage` data when you open a new tab?
12. What is the same-origin policy for web storage?

---

## 2.28 Security in JavaScript

### ✅ Important Topics

- [ ] XSS (Cross-Site Scripting)
- [ ] CSRF (Cross-Site Request Forgery)
- [ ] CORS (Cross-Origin Resource Sharing)
- [ ] Content Security Policy (CSP)
- [ ] SQL Injection
- [ ] Clickjacking
- [ ] eval() dangers
- [ ] Sanitization
- [ ] HttpOnly cookies
- [ ] Secure headers
- [ ] Same-Origin Policy

### 📋 Interview Questions

1. What is XSS? What are the types of XSS?
2. How do you prevent XSS attacks?
3. What is CSRF? How do you prevent it?
4. What is CORS? How does it work?
5. What is the Same-Origin Policy?
6. Why is `eval()` dangerous?
7. What is Content Security Policy (CSP)?
8. What is clickjacking? How do you prevent it?
9. How do you sanitize user input in JavaScript?
10. What is the difference between stored XSS and reflected XSS?
11. What is the role of `HttpOnly` flag in preventing XSS?
12. How does CORS preflight work?

---

## 2.29 Event Delegation

### ✅ Important Topics

- [ ] Event bubbling
- [ ] Event capturing
- [ ] Event delegation pattern
- [ ] Event propagation
- [ ] stopPropagation()
- [ ] stopImmediatePropagation()
- [ ] preventDefault()
- [ ] Event target vs currentTarget
- [ ] Custom events

### 📋 Interview Questions

1. What is event bubbling?
2. What is event capturing?
3. What is event delegation? Why is it useful?
4. What is the difference between `event.target` and `event.currentTarget`?
5. What does `stopPropagation()` do?
6. What is the difference between `stopPropagation()` and `stopImmediatePropagation()`?
7. What does `preventDefault()` do?
8. What is the difference between `addEventListener` and `onclick`?
9. How do you create and dispatch custom events?
10. In what order do event handlers fire: capturing or bubbling?
11. How does event delegation improve performance?

### 💻 Coding Questions

12. Implement event delegation for a dynamic list.
13. Create a click handler for a table using event delegation.
14. Implement a custom event system (pub/sub pattern).

---

## 2.30 Miscellaneous Must-Know JavaScript

### ✅ Important Topics

- [ ] Type coercion (implicit and explicit)
- [ ] == vs ===
- [ ] typeof vs instanceof
- [ ] NaN behavior
- [ ] null vs undefined
- [ ] Truthy and Falsy values
- [ ] IIFE (Immediately Invoked Function Expression)
- [ ] Strict mode
- [ ] Error types (SyntaxError, TypeError, ReferenceError, RangeError)
- [ ] try...catch...finally
- [ ] Custom errors
- [ ] Proxy and Reflect
- [ ] Object.defineProperty
- [ ] Property descriptors (writable, enumerable, configurable)
- [ ] JSON.parse() and JSON.stringify()
- [ ] structuredClone()
- [ ] setTimeout vs setInterval
- [ ] requestAnimationFrame

### 📋 Interview Questions

1. What is type coercion in JavaScript?
2. What is the difference between `==` and `===`?
3. What are truthy and falsy values in JavaScript?
4. What is `NaN`? How do you check for `NaN`?
5. What is the difference between `null` and `undefined`?
6. What is the `typeof` operator? What are its quirks?
7. What is an IIFE? Why is it used?
8. What is strict mode? What changes does it introduce?
9. What is `JSON.stringify()`? What happens with circular references?
10. What is `structuredClone()`? How is it different from `JSON.parse(JSON.stringify())`?
11. What are property descriptors?
12. What is `Object.defineProperty()`?

### 🖥️ Output Based Questions

13. What is the output?

```js
console.log([] == ![]);
console.log([] == false);
console.log("" == false);
console.log(null == undefined);
console.log(null === undefined);
```

14. What is the output?

```js
console.log(typeof null);
console.log(typeof undefined);
console.log(typeof NaN);
console.log(typeof []);
console.log(typeof {});
console.log(typeof function () {});
```

15. What is the output?

```js
console.log(0.1 + 0.2 === 0.3);
console.log(0.1 + 0.2);
```

16. What is the output?

```js
console.log(NaN === NaN);
console.log(isNaN("hello"));
console.log(Number.isNaN("hello"));
```

17. What is the output?

```js
console.log(1 + "2" + 3);
console.log(1 + 2 + "3");
console.log("1" - 1);
console.log("5" * "2");
console.log(true + true);
console.log([] + []);
console.log([] + {});
console.log({} + []);
```

18. What is the output?

```js
console.log(false == "");
console.log(false == "0");
console.log("" == "0");
console.log(false == null);
console.log(false == undefined);
```

19. What is the output?

```js
const a = {};
const b = { key: "b" };
const c = { key: "c" };
a[b] = 123;
a[c] = 456;
console.log(a[b]);
```

20. What is the output?

```js
console.log(+"");
console.log(+true);
console.log(+false);
console.log(+null);
console.log(+undefined);
console.log(+{});
console.log(+[]);
console.log(+[1]);
console.log(+[1, 2]);
```

---

### 🎯 What Interviewer Expects (JavaScript)

- [ ] Deep understanding of closures, prototypes, and `this`
- [ ] Ability to predict output of tricky code snippets
- [ ] Understanding of async JavaScript (Event Loop, Promises, async/await)
- [ ] Knowledge of ES6+ features and when to use them
- [ ] Ability to implement polyfills (map, filter, reduce, bind, call, apply, Promise.all)
- [ ] Understanding of memory management and garbage collection
- [ ] Knowledge of browser APIs and DOM manipulation
- [ ] Security awareness (XSS, CSRF, CORS)

### ❌ Common Mistakes (JavaScript)

- [ ] Confusing `==` with `===`
- [ ] Not understanding `this` in arrow functions vs regular functions
- [ ] Not knowing the difference between `var`, `let`, and `const`
- [ ] Confusing synchronous and asynchronous code execution
- [ ] Not understanding the Event Loop order (microtasks vs macrotasks)
- [ ] Mutation confusion (which methods mutate arrays, shallow vs deep copy)
- [ ] Not handling Promise rejections
- [ ] Using `typeof null === 'object'` without understanding why
- [ ] Forgetting TDZ with `let` and `const`
- [ ] Not knowing the difference between `null` and `undefined`
- [ ] Confusing `slice()` and `splice()`
- [ ] Not understanding prototype chain lookup

---

> **📌 SECTION 2 COMPLETE — JavaScript**

---
