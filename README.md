<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Job Application</title>
</head>
<body>
    <h2 style="text-align: center;">Job Application</h2>
    <form style="max-width: 400px; margin: auto; display: flex; flex-direction: column; gap: 10px;">
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
        
        <button type="submit" style="background-color: #28a745; color: white; padding: 10px; border: none; cursor: pointer;">Apply</button>
    </form>
</body>
</html>
