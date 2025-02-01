# **React Basics - Lecture 7**

## **📌 Overview**
In this lecture, we explore the fundamentals of **React.js**, including its core concepts like **components, props, state, JSX, and event handling**. React is a powerful JavaScript library for building interactive and dynamic user interfaces efficiently.

---

## **1️⃣ What is React?**
- **React.js** is an open-source JavaScript library used for building user interfaces.
- It follows a **component-based architecture**, making UI development modular and reusable.
- Developed and maintained by **Facebook (Meta)**.
- Utilizes **Virtual DOM** for efficient updates and rendering.

---

## **2️⃣ Setting Up a React Project**
To create a new React project, use **Create React App**:
```bash
npx create-react-app my-app
cd my-app
npm start
```
This sets up a development server and opens the app in the browser.

---

## **3️⃣ JSX (JavaScript XML)**
JSX allows writing HTML-like syntax inside JavaScript.
```jsx
const element = <h1>Hello, React!</h1>;
```
JSX expressions must be wrapped in a single parent element and use `{}` for embedding JavaScript.

Example:
```jsx
function Welcome() {
  return <h1>Welcome to React</h1>;
}
```

---

## **4️⃣ Components in React**
### **🔹 Functional Components** (Stateless)
A simple function returning JSX:
```jsx
function Greeting() {
  return <h1>Hello, User!</h1>;
}
export default Greeting;
```

### **🔹 Class Components** (Stateful)
Used when managing state:
```jsx
import React, { Component } from 'react';
class Greeting extends Component {
  render() {
    return <h1>Hello, User!</h1>;
  }
}
export default Greeting;
```

---

## **5️⃣ Props in React**
Props allow data to be passed between components.
```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}!</h1>;
}
```
Usage:
```jsx
<Welcome name="John" />
```

---

## **6️⃣ State in React**
State allows components to manage dynamic data.
```jsx
import React, { useState } from 'react';
function Counter() {
  const [count, setCount] = useState(0);
  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}
export default Counter;
```

---

## **7️⃣ Event Handling in React**
React uses camelCase for event handlers.
```jsx
function ClickHandler() {
  function handleClick() {
    alert("Button clicked!");
  }
  return <button onClick={handleClick}>Click Me</button>;
}
```

---

## **📌 Summary Table**
| Concept | Description | Example |
|---------|-------------|---------|
| JSX | JavaScript + XML for UI structure | `<h1>Hello</h1>` |
| Functional Component | Stateless component | `function App() {}` |
| Class Component | Stateful component | `class App extends Component {}` |
| Props | Pass data between components | `<Component propName={value} />` |
| State | Internal component data management | `useState(0)` |
| Events | Handle user interactions | `onClick={handleClick}` |

---

🚀 **Happy Coding with React!**


