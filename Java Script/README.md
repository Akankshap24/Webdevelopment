# Day 1
# What is JavaScript ?

JavaScript is a `lightweight`, `interpreted`, and `just-in-time (JIT) compiled` programming language.



## ✅ Key Concepts

| Concept         | Meaning                                                                 |
|----------------|-------------------------------------------------------------------------|
| **Lightweight**| Uses less memory and resources. Easy to embed and quick to load         |
| **Interpreted**| Code is executed **line by line** at runtime                            |
| **Compiled**   | Code is translated to machine code before or during execution           |



## ⚙️ Types of Compilation in JavaScript

| Type      | Full Form           | When It Happens                         | How It Works                                                             | Example                    |
|-----------|---------------------|-----------------------------------------|---------------------------------------------------------------------------|----------------------------|
| **JIT**   | Just-in-Time        | **During runtime** (after user request) | Code is compiled **in the browser**, just before it's executed            | Chrome's **V8 Engine**     |
| **AOT**   | Ahead-of-Time       | **Before runtime** (during build)       | Code is compiled **before deployment**, at the **application level**     | **Angular** with AOT build |


## 📝 Example Use

- Browsers like Chrome, Firefox → `JIT Compilation`
- Frameworks like Angular → `AOT Compilation` for faster initial load.

## ⚙️ JavaScript Engines & Compilers

JavaScript can run using different `engines` and `compilers` across environments:

| Tool     | Description                                           |
|----------|-------------------------------------------------------|
| **Ivy**  | Angular's next-gen compilation and rendering engine   |
| **Babel**| JavaScript compiler that converts ES6+ to ES5         |
| **Node** | Runtime for executing JS on the server (built on V8) |
| **V8**   | Google Chrome's powerful JavaScript engine            |

---

## 🧠 JavaScript Programming Paradigms

JavaScript supports `multiple programming paradigms`:

| Paradigm               | Description                                                       |
|------------------------|-------------------------------------------------------------------|
| **Structural**         | Code is organized using functions and blocks                      |
| **Functional**         | Emphasizes pure functions, immutability, and function composition |
| **Imperative**         | Code describes **how** things should happen (step-by-step)        |
| **Object-Oriented**    | Uses objects and inheritance (but **not fully OOP**)              |

---

> 🔎 **Note:** JavaScript is *not a purely OOP language*, but it supports some OOP concepts like objects, classes, and inheritance (via prototypes).
---

## 🧩 JavaScript Usage in Full-Stack Projects

JavaScript is used at **various layers** of development:

| Layer          | Tool / Tech                                | Role                                 |
|----------------|---------------------------------------------|--------------------------------------|
| **Client Side**| HTML + JavaScript                          | Dynamic frontend interaction         |
| **Server Side**| Node.js                                     | Backend logic and APIs               |
| **Database**   | MongoDB (with JS-based queries)             | Data storage using JS-like syntax    |
| **Animation**  | Tools like Flash, 3DS Max (older usage)     | Motion graphics, UI effects          |

---

## ❓ FAQ: What are the Issues with JavaScript?

JavaScript, despite being powerful and widely used, has a few key limitations:

### 1️⃣ Not Strongly Typed
JavaScript allows a variable to hold different types of data without restriction:

```js
let a = 10;        // number
a = "sachin";      // string
a = false;         // boolean
a = 13.5;          // number
```
🔸JavaScript is `not strongly typed` — no fixed datatype on a variable.

### 2️⃣ Not Strictly Typed
JavaScript allows you to use undeclared variables unless in strict mode:

```js
"use strict";
a = 10;  // ❌ Error: 'a' is not declared
```

🔸JavaScript is `not strictly typed` — variables can be used without declaring.

### 3️⃣ No Uniform Data Control
JavaScript doesn't enforce a uniform object structure:

```js
[
  { Name: "Samsung", price: 45000 },
  { Product: "LG", cost: 55000 }
]
```

⚠️ Different property names `(Name, Product, price, cost)` make data processing difficult.

### 4️⃣ Security Concerns
JavaScript can be misused or blocked by browsers due to security risks.

### 🔐 Security Concerns in JavaScript

| Example       | Type     | Description                                                                           |
|---------------|----------|---------------------------------------------------------------------------------------|
| **Trojan**    | ❌ Bad   | A virus installed to secretly control a device without consent — malicious approach.  |
| **TeamViewer**| ✅ Good  | A legitimate tool installed with user permission to control a device — safe approach. |

🔐 JavaScript is `not inherently secure` and is often restricted by modern browsers.


# Day 2

## 🌐 JavaScript – Client Side

JavaScript plays a vital role on the **client side** by reducing the load on the server and improving the overall performance of web applications.

---

### ✅ Purpose

- To **avoid burden** on the server.
- To **enhance performance** by handling interactions in the browser.

---

### 🧠 Key Client-Side Interactions

#### 1. 📄 DOM Manipulations

- Add elements to the page
- Remove elements from the page
- Update content inside elements
- Apply dynamic styles to elements
- Attach events dynamically to elements

#### 2. ✔️ Validations

- Verify and validate **user input** before sending it to the server

#### 3. 💾 Client-Side Management

| Area                  | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| *Client Memory*         | Store temporary data like username/password in browser cache                |
| *Client Devices*        | Example: Ticket booking — print ticket without internet                     |
| *User Location*         | Websites request location access to provide location-specific experiences   |
| *Data Sharing*          | Share data between apps on the client device                                |





