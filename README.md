# Ex.-5-React-Lab-Exercise-Form-Handling-in-React
## Name: TAMIL MARUDHU K
## Roll no: 2305001033
## Department: CSE

## AIM
### To develop a simple Student Registration Form using React and handle form input values using the useState Hook.

## PROGRAM
### i) App.jsx
```py
import { useState } from "react";
import "./App.css";
function App() {
 const [name, setName] = useState("");
 const [registerNo, setRegisterNo] = useState("");
 const [department, setDepartment] = useState("");
 function handleSubmit(event) {
 event.preventDefault();
 alert(
 "Name: " +
 name +
 "\nRegister Number: " +
 registerNo +
 "\nDepartment: " +
 department
 );
 }
 return (
 <div className="container">
 <h1>Student Registration Form</h1>
 <form onSubmit={handleSubmit}>
 <label>Name</label>
 <input
 type="text"
 placeholder="Enter your name"
 value={name}
 onChange={(event) => setName(event.target.value)}
 />
 <label>Register Number</label>
 <input
 type="text"
 placeholder="Enter register number"
 value={registerNo}
 onChange={(event) => setRegisterNo(event.target.value)}
 />
 <label>Department</label>
 <input
 type="text"
 placeholder="Enter department"
 value={department}
 onChange={(event) => setDepartment(event.target.value)}/>
 <button type="submit">Submit</button>
 </form>
 </div>
 );
}
export default App;
```
### ii) App.css
```py
.container {
 width: 400px;
 margin: 50px auto;
 padding: 25px;
 border: 1px solid gray;
 border-radius: 10px;
}
h1 {
 text-align: center;
 color: blue;
}
label {
 display: block;
 margin-top: 15px;
 font-weight: bold;
}
input {
 width: 100%;
 padding: 10px;
 margin-top: 5px;
 box-sizing: border-box;
}
button {
 margin-top: 20px;
 padding: 10px 20px;
 background-color: blue;
 color: white;
 border: none;
 border-radius: 5px;
 cursor: pointer;
}
```
## OUTPUT
<img width="696" height="321" alt="image" src="https://github.com/user-attachments/assets/8791270f-159d-4289-b42a-ccf9cac2b1ec" />
<img width="690" height="360" alt="image" src="https://github.com/user-attachments/assets/d8041203-9db9-43e0-a478-7c9658a84411" />

## RESULT
### Thus, a Student Registration Form was successfully created using React. The form input valueswere managed using the useState() Hook, user input was handled using the onChange event, and form submission was handled using the onSubmit event.
