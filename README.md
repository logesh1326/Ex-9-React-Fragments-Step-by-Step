# Ex. 9 React Fragments — Step by Step

## Exercise Number
Exercise 9

## Subject
AI1067 - Modern Web Application Development (React JS Lab)

## Student Details
- **Name:** LOGESH S
- **Roll No:** 2305001014
- **Department:** B.Tech CSE
- **College:** IST, NMV University

## Objective
React JS Lab Exercise

## Description
Ex. 9 React Fragments — Step by Step 
1. What is a React Fragment? 
A React Fragment allows us to group multiple elements without adding an extra HTML 
element such as <div> to the DOM. 
The syntax is: 
<> 
  <h1>Hello</h1> 
  <p>Welcome to React</p> 
</> 
The <>...</> is called a Fragment shorthand. 
 
2. Why Do We Need Fragments? 
A React component normally needs to return a single parent element. 
This will cause an error: 
function App() { 
  return ( 
    <h1>Hello</h1> 
    <p>Welcome</p> 
  ); 
} 
There are two separate elements at the top level. 
 
3. Solution Using <div> 
We can put them inside a <div>: 
function App() { 
  return ( 
    <div> 
      <h1>Hello</h1> 
      <p>Welcome</p> 
    </div> 
  ); 
} 
This works, but the <div> creates an extra DOM element. 
 
4. Solution Us

## Technologies Used
- React JS
- Vite
- JavaScript (JSX)
- HTML5 / CSS3

## How to Run
```bash
npm create vite@latest my-app -- --template react
cd my-app
npm install
npm run dev
```

## Exercise Content
See `exercise.txt` for complete exercise content and source code.
