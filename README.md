# React Lab Exercise 9: React Fragments
## Name: LOGESH S
## Roll no: 2305001014
## Department: CSE

## AIM
### To understand and implement React Fragments to group multiple JSX elements without creating unnecessary DOM elements.

## PROGRAM

### i) App.jsx
```jsx
import { Fragment } from "react";
import "./App.css";

function Student() {
  return (
    <>
      <h2>Student Details</h2>
      <p>Name: Ajith</p>
      <p>Department: CSE</p>
      <p>Year: III Year</p>
    </>
  );
}

function App() {
  const students = [
    { id: 1, name: "Ajith" },
    { id: 2, name: "Ravi" },
    { id: 3, name: "Divya" },
  ];

  return (
    <div className="container">
      <h1>College Information</h1>
      <Student />
      <hr />
      <h2>Student List</h2>
      {students.map((student) => (
        <Fragment key={student.id}>
          <h3>{student.name}</h3>
          <p>Department: Computer Science</p>
          <hr />
        </Fragment>
      ))}
    </div>
  );
}

export default App;
```

## OUTPUT
<img width="1125" height="473" alt="image" src="https://github.com/user-attachments/assets/f8468b80-64bb-40da-98a7-0f3ed460b73a" />
<img width="1125" height="509" alt="image" src="https://github.com/user-attachments/assets/cd02aaae-b9b7-48af-ad30-d12a290b3d59" />

## RESULT
### Thus, React Fragments were successfully implemented using both shorthand syntax (<> </>) and explicit Fragment syntax. Multiple JSX elements were grouped without adding extra wrapper elements to the DOM.
