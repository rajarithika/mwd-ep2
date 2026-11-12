# Exp 02 – React Lab Exercise: Using Props

## **NAME : Raja Rithika**

## **REG NO: 2305001029**

---

## Aim

To create a React application that demonstrates passing data from a parent component to a child component using props.

## Objectives

- To create a React project using Vite.
- To create a reusable Employee component.
- To pass employee details such as name, ID, department, and designation using props.
- To display multiple employees using the same component.
- To understand props destructuring and one-way data flow in React.

## Program

### Step 1: Create a React Project

Execute the following commands:

```bash
npm create vite@latest props-demo -- --template react
cd props-demo
npm install
npm run dev
```

### Step 2: Create Employee.jsx

Create `Employee.jsx` inside the `src` folder.

```jsx
function Employee({ name, id, department, designation }) {
  return (
    <div>
      <h2>Employee Details</h2>
      <p>Name: {name}</p>
      <p>ID: {id}</p>
      <p>Department: {department}</p>
      <p>Designation: {designation}</p>
      <hr />
    </div>
  )
}

export default Employee
```

### Step 3: Write App.jsx

Open `src/App.jsx` and add:

```jsx
import Employee from './Employee'

function App() {
  return (
    <div>
      <h1>Employee Information</h1>

      <Employee
        name="Raja Rithika"
        id="2305001029"
        department="CSE"
        designation="Software Developer"
      />

      <Employee
        name="user123"
        id="102"
        department="IT"
        designation="Web Developer"
      />

      <Employee
        name="user456"
        id="103"
        department="AIDS"
        designation="Data Analyst"
      />
    </div>
  )
}

export default App
```

### Step 4: Run the Application

Execute:

```bash
npm run dev
```

Open the localhost URL displayed in the terminal.

## Output

<img width="1199" height="1312" alt="image" src="https://github.com/user-attachments/assets/c67f457d-5925-4aa7-8f3c-5f04f4ce0547" />

## Result

Thus, a React application was successfully created and executed to demonstrate passing employee information from a parent component to a child component using props.
