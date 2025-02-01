# **Redux Basics**

## **📌 Overview**
In this lecture, we explore the fundamentals of **Redux**, including its core principles, architecture, and how it manages state efficiently in React applications. Redux is a predictable state container that helps manage complex application states.

---

## **1️⃣ What is Redux?**
- **Redux** is a state management library for JavaScript applications.
- It helps manage the global state in a predictable manner.
- Works well with **React**, but can also be used with other frameworks.
- Uses a **unidirectional data flow** and a central store for managing state.

---

## **2️⃣ Core Principles of Redux**
Redux follows three fundamental principles:

1. **Single Source of Truth**
   - The entire state of the application is stored in a **single store**.
2. **State is Read-Only**
   - The only way to change the state is by **dispatching actions**.
3. **Changes are Made with Pure Functions**
   - Reducers are **pure functions** that determine how state changes.

---

## **3️⃣ Redux Architecture**
The Redux architecture consists of the following components:

### **🔹 Store**
- The central repository that holds the application's state.
```js
import { createStore } from 'redux';
const store = createStore(reducer);
```

### **🔹 Actions**
- Plain JavaScript objects describing what should change in the state.
```js
const incrementAction = {
  type: 'INCREMENT',
};
```

### **🔹 Reducers**
- Functions that specify how the application's state changes.
```js
const counterReducer = (state = { count: 0 }, action) => {
  switch (action.type) {
    case 'INCREMENT':
      return { count: state.count + 1 };
    case 'DECREMENT':
      return { count: state.count - 1 };
    default:
      return state;
  }
};
```

### **🔹 Dispatch**
- Sends actions to the reducer to update the state.
```js
store.dispatch({ type: 'INCREMENT' });
```

### **🔹 Subscribe**
- Listens for state changes.
```js
store.subscribe(() => {
  console.log(store.getState());
});
```

---

## **4️⃣ Setting Up Redux in a React App**
To use Redux in a React application, follow these steps:

### **🔹 Install Redux and React-Redux**
```bash
npm install redux react-redux
```

### **🔹 Create a Redux Store**
```js
import { createStore } from 'redux';
import counterReducer from './reducers/counterReducer';
const store = createStore(counterReducer);
```

### **🔹 Provide Store to React**
```js
import { Provider } from 'react-redux';
import App from './App';
import store from './store';

const Root = () => (
  <Provider store={store}>
    <App />
  </Provider>
);
```

### **🔹 Connect Redux to Components**
```js
import { useSelector, useDispatch } from 'react-redux';

function Counter() {
  const count = useSelector(state => state.count);
  const dispatch = useDispatch();

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => dispatch({ type: 'INCREMENT' })}>+</button>
      <button onClick={() => dispatch({ type: 'DECREMENT' })}>-</button>
    </div>
  );
}
```

---

## **📌 Summary Table**
| Concept | Description | Example |
|---------|-------------|---------|
| Store | Centralized state container | `createStore(reducer)` |
| Action | Describes state changes | `{ type: 'INCREMENT' }` |
| Reducer | Pure function handling state updates | `switch(action.type)` |
| Dispatch | Sends actions to reducer | `dispatch({ type: 'INCREMENT' })` |
| useSelector | Retrieves state from store | `useSelector(state => state.count)` |
| useDispatch | Dispatches actions from component | `useDispatch()` |

---

🚀 **Happy Coding with Redux!**


