# **JavaScript Basics - Part 1**

## **📌 Overview**
This lecture introduces the fundamentals of JavaScript, including variable declaration, different ways to display output, and data types such as numbers, strings, arrays, and objects. JavaScript is a powerful programming language used for adding interactivity to web pages.

---

## **1️⃣ Introduction to JavaScript**
JavaScript (JS) is a **lightweight, interpreted**, and **dynamic** programming language widely used for web development. It enables interactivity, such as handling user inputs, animations, and API communications.

✅ **Why Use JavaScript?**
- Enhances web interactivity
- Manipulates HTML & CSS dynamically
- Handles events (click, hover, form submission)
- Supports backend development (Node.js)

You can include JavaScript in an HTML file in three ways:
```html
<!-- Inline JavaScript -->
<button onclick="alert('Hello!')">Click Me</button>

<!-- Internal JavaScript -->
<script>
    console.log("Hello, JavaScript!");
</script>

<!-- External JavaScript -->
<script src="script.js"></script>
```

---

## **2️⃣ Variable Declaration**
JavaScript provides three ways to declare variables:

### **🔹 Using `var` (Old Method)**
- Function-scoped
- Can be redeclared and updated
- Can be hoisted
```js
var name = "John";
console.log(name);
```

### **🔹 Using `let` (Recommended for block-scoped variables)**
- Block-scoped
- Can be updated but not redeclared
```js
let age = 25;
age = 26; // ✅ Allowed
```

### **🔹 Using `const` (Recommended for constants)**
- Block-scoped
- Cannot be updated or redeclared
```js
const PI = 3.1416;
// PI = 3.15; ❌ Error: Cannot reassign
```

---

## **3️⃣ Different Ways to Display Output**
### **🔹 `console.log()` (For debugging in browser console)**
```js
console.log("Hello, World!");
```
### **🔹 `alert()` (Displays a popup alert box)**
```js
alert("Welcome to JavaScript!");
```
### **🔹 `document.write()` (Writes content to the webpage)**
```js
document.write("Hello, this is JavaScript!");
```
### **🔹 `innerHTML` (Inserts content into an HTML element)**
```js
document.getElementById("demo").innerHTML = "Hello, JavaScript!";
```

---

## **4️⃣ JavaScript Data Types**
JavaScript has **primitive** and **non-primitive** data types.

### **🔹 1. Number**
Stores numeric values, including integers and decimals.
```js
let num1 = 10;
let num2 = 3.14;
console.log(num1 + num2); // 13.14
```

### **🔹 2. String**
Stores textual data and must be enclosed in quotes (`" "`, `' '`, or \`\`).
```js
let message = "Hello, JavaScript!";
console.log(message.length); // Output: 17
```
#### **String Concatenation**
```js
let firstName = "John";
let lastName = "Doe";
console.log(firstName + " " + lastName); // John Doe
```
#### **Template Literals (Using backticks ``)**
```js
console.log(`My name is ${firstName} ${lastName}`);
```

### **🔹 3. Boolean**
Represents **true** or **false** values.
```js
let isAdult = true;
console.log(isAdult); // Output: true
```

### **🔹 4. Array** (Stores multiple values in a single variable)
```js
let fruits = ["Apple", "Banana", "Mango"];
console.log(fruits[0]); // Apple
```
#### **Array Methods:**
```js
fruits.push("Orange"); // Adds an element
fruits.pop(); // Removes last element
console.log(fruits.length); // Returns array length
```

### **🔹 5. Object** (Stores key-value pairs)
```js
let person = {
    firstName: "John",
    lastName: "Doe",
    age: 25
};
console.log(person.firstName); // Output: John
```
#### **Accessing Object Properties**
```js
console.log(person["lastName"]); // Doe
```

---

## **📌 Summary Table**
| Data Type | Example |
|-----------|---------|
| Number | `let num = 10;` |
| String | `let str = "Hello";` |
| Boolean | `let isTrue = true;` |
| Array | `let arr = [1, 2, 3];` |
| Object | `let obj = {key: "value"};` |

---

## **📌 Next Steps**
Now that you've learned JavaScript basics, move on to:
- JavaScript **Operators and Expressions**
- JavaScript **Functions**
- JavaScript **DOM Manipulation**

Happy Coding! 🚀

