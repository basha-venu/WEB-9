# Exp 9 – React Lab Exercise: React Fragments

## NAME:  BASHA VENU
## REG NO: 2305001005

## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: BASHA VENU</h3>

      <p>Register Number: 2305001005</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: BASHA VENU</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### Fragment Shorthand Syntax

<img width="1376" height="715" alt="image" src="https://github.com/user-attachments/assets/9f0e0a81-a4fa-4d49-8697-246d1b726170" />


### Explicit Fragment Syntax

<img width="1383" height="716" alt="image" src="https://github.com/user-attachments/assets/591aef65-352c-40c8-97e1-dea2904a3409" />


## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
