//# Student-Registration-form-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Student Registration Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 40px;
        }
        form {
            max-width: 400px;
        }
        label {
            display: block;
            margin-top: 15px;
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            box-sizing: border-box;
        }
        button {
            margin-top: 20px;
            padding: 10px;
            width: 100%;
            background-color: #4CAF50;
            color: white;
            font-size: 16px;
            border: none;
        }
    </style>
</head>
<body>

<h2>Student Registration Form</h2>

<form method="POST" action="/submit-registration">
    <label for="name">Full Name:</label>
    <input 
        type="text" 
        id="name" 
        name="name" 
        placeholder="Enter your full name" 
        required 
    >

    <label for="email">Email Address:</label>
    <input 
        type="email" 
        id="email" 
        name="email" 
        placeholder="Enter your email" 
        required 
    >

    <label for="password">Password:</label>
    <input 
        type="password" 
        id="password" 
        name="password" 
        placeholder="Create a password" 
        required 
        minlength="6"
    >

    <label for="gender">Gender:</label>
    <select id="gender" name="gender" required>
        <option value="" disabled selected>Select your gender</option>
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option>
    </select>

    <label for="age">Age:</label>
    <input 
        type="number" 
        id="age" 
        name="age" 
        placeholder="Enter your age" 
        required 
        min="10" max="100"
    >

    <label for="address">Address:</label>
    <textarea 
        id="address" 
        name="address" 
        placeholder="Enter your address" 
        rows="3" 
        required
    ></textarea>

    <label for="course">Course:</label>
    <select id="course" name="course" required>
        <option value="" disabled selected>Select your course</option>
        <option value="science">ECE</option>
        <option value="commerce">CSE</option>
        <option value="arts">ELCE</option>
    </select>

    <button type="submit">Register</button>
</form>

</body>
</html>
