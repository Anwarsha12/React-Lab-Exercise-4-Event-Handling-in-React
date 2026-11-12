# React Lab Exercise 4: Event Handling in React
## Name: Anwarsha E.M
## Roll no: 2305001002
## Department: CSE

## AIM
### To understand and implement event handling in React using events such as onClick, onChange, and onSubmit. 

## PROGRAM
### App.jsx  
### i) onClick Event function
```py
App() {   function handleClick() {     alert("Button was clicked!"); 
  }   return ( 
    <div> 
      <h1>React Event Handling</h1> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} export default App;
```
 
### ii) onClick with State
```py
import { useState } from "react"; function App() {   const [count, setCount] = useState(0);   function handleClick() {     setCount(count + 1); 
  }   return ( 
    <div> 
      <h1>Click Counter</h1> 
      <h2>Button clicked: {count} times</h2> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} export default App; 
 ```
### iii) onChange Event 
```py
import { useState } from "react"; function App() {   const [name, setName] = useState("");   function handleChange(event) {     setName(event.target.value); 
  }   return ( 
    <div> 
      <h1>Student Name</h1> 
      <input 
        type="text" 
        placeholder="Enter your name"         onChange={handleChange} 
      /> 
      <h2>Hello, {name}</h2> 
    </div> 
  ); 
} export default App; 
```
## OUTPUT
<img width="917" height="229" alt="Screenshot 2026-11-13 005305" src="https://github.com/user-attachments/assets/68ccd145-0033-4b7d-9cf1-0a8f7a167b36" />
<img width="920" height="157" alt="Screenshot 2026-11-13 005320" src="https://github.com/user-attachments/assets/4aeb9f09-de89-4f8a-99f5-3238c3049daf" />
<img width="915" height="152" alt="Screenshot 2026-11-13 005337" src="https://github.com/user-attachments/assets/b58849d6-cece-4476-ba12-12a1dfb91b01" />


## RESULT
### Thus, React event handling was successfully implemented using the onClick and onChange events. The application responded to button clicks, maintained a click counter using useState, and displayed the student's name dynamically based on user input. 
