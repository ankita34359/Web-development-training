# **JavaScript Basics - Part 2**

## **📌 Overview**
In this lecture, we will cover key JavaScript concepts such as **operators, conditional statements, loops, functions, arrow functions, the DOM, and events**. Mastering these concepts will help you build interactive and dynamic web applications.

---

## **1️⃣ JavaScript Operators**
Operators allow us to perform operations on variables and values.

### **🔹 Arithmetic Operators** (Perform mathematical operations)
```js
let a = 10, b = 5;
console.log(a + b); // Addition → 15
console.log(a - b); // Subtraction → 5
console.log(a * b); // Multiplication → 50
console.log(a / b); // Division → 2
console.log(a % b); // Modulus (remainder) → 0
console.log(a ** b); // Exponentiation (a^b) → 100000
```

### **🔹 Comparison Operators** (Compare values and return a boolean)
```js
console.log(10 == "10"); // true (checks value only)
console.log(10 === "10"); // false (checks value & type)
console.log(10 != 5); // true
console.log(10 > 5); // true
console.log(10 < 5); // false
```

### **🔹 Logical Operators** (Used in conditions)
```js
console.log(true && false); // false (AND)
console.log(true || false); // true (OR)
console.log(!true); // false (NOT)
```

---

## **2️⃣ Conditional Statements**
Conditional statements execute different code blocks based on conditions.

### **🔹 if-else Statement**
```js
let age = 18;
if (age >= 18) {
    console.log("You are an adult.");
} else {
    console.log("You are a minor.");
}
```

### **🔹 else-if Ladder**
```js
let score = 85;
if (score >= 90) {
    console.log("Grade: A");
} else if (score >= 75) {
    console.log("Grade: B");
} else {
    console.log("Grade: C");
}
```

### **🔹 Switch Case**
```js
let day = "Monday";
switch (day) {
    case "Monday":
        console.log("Start of the week!");
        break;
    case "Friday":
        console.log("Weekend is near!");
        break;
    default:
        console.log("Just another day!");
}
```

---

## **3️⃣ Loops in JavaScript**
Loops help in executing a block of code multiple times.

### **🔹 for Loop**
```js
for (let i = 1; i <= 5; i++) {
    console.log("Iteration: " + i);
}
```

### **🔹 while Loop**
```js
let count = 1;
while (count <= 5) {
    console.log("Count: " + count);
    count++;
}
```

### **🔹 do-while Loop**
```js
let num = 1;
do {
    console.log("Number: " + num);
    num++;
} while (num <= 5);
```

---

## **4️⃣ Functions in JavaScript**
Functions are reusable blocks of code that perform specific tasks.

### **🔹 Regular Function**
```js
function greet(name) {
    return "Hello, " + name;
}
console.log(greet("John"));
```

### **🔹 Arrow Function (ES6)**
A shorter syntax for functions.
```js
const add = (a, b) => a + b;
console.log(add(3, 4)); // Output: 7
```

---

## **5️⃣ Document Object Model (DOM)**
DOM allows JavaScript to manipulate HTML elements dynamically.

### **🔹 Accessing Elements**
```js
let heading = document.getElementById("title");
console.log(heading.innerText);
```
```js
let items = document.getElementsByClassName("list-item");
console.log(items[0].innerText);
```

### **🔹 Changing Content**
```js
document.getElementById("title").innerText = "Welcome to JavaScript!";
```

### **🔹 Changing Styles**
```js
document.getElementById("title").style.color = "blue";
```

### **🔹 Creating & Appending Elements**
```js
let para = document.createElement("p");
para.innerText = "This is a new paragraph!";
document.body.appendChild(para);
```

---

## **6️⃣ JavaScript Events**
Events are user interactions like clicks, key presses, etc.

### **🔹 onclick Event**
```js
function showMessage() {
    alert("Button Clicked!");
}
```
```html
<button onclick="showMessage()">Click Me</button>
```

### **🔹 addEventListener() Method**
```js
document.getElementById("myBtn").addEventListener("click", function() {
    alert("Button Clicked!");
});
```

### **🔹 Mouse Events**
```js
document.getElementById("box").onmouseover = function() {
    console.log("Mouse is over the box!");
};
```

### **🔹 Keyboard Events**
```js
document.addEventListener("keydown", function(event) {
    console.log("Key Pressed: " + event.key);
});
```

---

## **📌 Summary Table**
| Concept | Description | Example |
|---------|-------------|---------|
| Operators | Perform operations on values | `a + b`, `a == b` |
| Conditional Statements | Execute different blocks based on conditions | `if-else`, `switch` |
| Loops | Repeat execution | `for`, `while`, `do-while` |
| Functions | Reusable blocks of code | `function greet() {}` |
| Arrow Functions | Shorter function syntax | `const add = (a, b) => a + b;` |
| DOM Manipulation | Interact with HTML elements | `document.getElementById("title").innerText = "Hello";` |
| Events | Handle user interactions | `onclick`, `addEventListener()` |

---

🚀 Happy Coding! 😊


