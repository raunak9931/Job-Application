<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Job Application</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #e0f7fa, #80deea);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            background-color: #ffffff;
            padding: 40px;
            box-shadow: 0 15px 25px rgba(0, 0, 0, 0.1);
            border-radius: 12px;
            width: 100%;
            max-width: 500px;
            border: 1px solid #ddd;
            transition: all 0.3s ease-in-out;
        }

        .container:hover {
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }

        h2 {
            text-align: center;
            margin-bottom: 20px;
            color: #00796b;
            font-size: 28px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        label {
            margin-bottom: 8px;
            font-size: 16px;
            color: #333;
            font-weight: bold;
            display: block;
        }

        input, select, button {
            width: 100%;
            padding: 12px;
            margin-bottom: 20px;
            border: 2px solid #80deea;
            border-radius: 8px;
            font-size: 16px;
            background-color: #f5f5f5;
            transition: all 0.3s ease-in-out;
        }

        input:focus, select:focus, button:focus {
            border-color: #00796b;
            outline: none;
            box-shadow: 0 0 8px rgba(0, 121, 107, 0.5);
        }

        button {
            background-color: #00796b;
            color: white;
            cursor: pointer;
            border: none;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #004d40;
        }

        input[type="file"] {
            padding: 10px;
            background-color: #f9f9f9;
            border: 2px solid #ccc;
        }

        .form-footer {
            text-align: center;
            font-size: 14px;
            color: #666;
        }

        .form-footer a {
            color: #00796b;
            text-decoration: none;
            font-weight: bold;
        }

        .form-footer a:hover {
            text-decoration: underline;
        }

        /* Add a smooth animation for inputs */
        input, select, button {
            animation: slideIn 0.5s ease-out;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Job Application</h2>
        <form>
            <label for="name">Full Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="phone">Phone Number:</label>
            <input type="tel" id="phone" name="phone" required>

            <label for="position">Position Applied For:</label>
            <input type="text" id="position" name="position" required>

            <label for="qualification">Highest Qualification:</label>
            <select id="qualification" name="qualification" required>
                <option value="">Select</option>
                <option value="bachelor">Bachelor's Degree</option>
                <option value="master">Master's Degree</option>
                <option value="diploma">Diploma</option>
            </select>

            <label for="resume">Upload Resume:</label>
            <input type="file" id="resume" name="resume" accept=".pdf,.doc,.docx" required>

            <button type="submit">Apply</button>
        </form>
        <div class="form-footer">
            <p>Already have an account? <a href="#">Log In</a></p>
        </div>
    </div>
</body>
</html>
