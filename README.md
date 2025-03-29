# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced HTML5 Implementation</title>
</head>
<body>
    <header>
        <h1>Welcome to Advanced HTML5</h1>
    </header>
    
    <section>
        <h2>Ordered List with Roman Numerals</h2>
        <ol type="I">
            <li>HTML Basics</li>
            <li>CSS Styling</li>
            <li>JavaScript Fundamentals</li>
            <li>Responsive Design</li>
            <li>Multimedia Integration</li>
        </ol>
    </section>
    
    <section>
        <h2>External Image</h2>
        <img src="https://www.pexels.com/photo/sample-image.jpg" alt="Sample Image from Pexels" width="600">
    </section>
    
    <section>
        <h2>Contact Table</h2>
        <table border="1">
            <tr>
                <th>Name</th>
                <th>Address</th>
                <th>Mobile</th>
                <th>Email</th>
            </tr>
            <tr>
                <td>John Doe</td>
                <td>123 Street, City</td>
                <td>+123456789</td>
                <td>johndoe@example.com</td>
            </tr>
            <tr>
                <td>Jane Smith</td>
                <td>456 Avenue, City</td>
                <td>+987654321</td>
                <td>janesmith@example.com</td>
            </tr>
            <tr>
                <td>Michael Johnson</td>
                <td>789 Boulevard, City</td>
                <td>+1122334455</td>
                <td>michaelj@example.com</td>
            </tr>
            <tr>
                <td>Emily White</td>
                <td>159 Drive, City</td>
                <td>+2233445566</td>
                <td>emilyw@example.com</td>
            </tr>
            <tr>
                <td>David Brown</td>
                <td>357 Lane, City</td>
                <td>+3344556677</td>
                <td>davidb@example.com</td>
            </tr>
        </table>
    </section>
    
    <section>
        <h2>Registration Form</h2>
        <form action="#" method="post">
            <label for="name">Full Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your full name" required><br>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required><br>
            
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" placeholder="Enter a password" required><br>
            
            <label for="dob">Date of Birth:</label>
            <input type="date" id="dob" name="dob" required><br>
            
            <label>Gender:</label>
            <input type="radio" name="gender" value="male" required> Male
            <input type="radio" name="gender" value="female" required> Female
            <input type="radio" name="gender" value="other" required> Other<br>
            
            <label for="country">Country:</label>
            <select id="country" name="country" required>
                <option value="">Select Country</option>
                <option value="usa">USA</option>
                <option value="uk">UK</option>
                <option value="canada">Canada</option>
            </select><br>
            
            <label>Interests:</label>
            <input type="checkbox" name="interests" value="coding"> Coding
            <input type="checkbox" name="interests" value="design"> Design
            <input type="checkbox" name="interests" value="music"> Music<br>
            
            <button type="submit">Register</button>
        </form>
    </section>
    
    <footer>
        <p>&copy; 2025 Advanced HTML5 Classroom</p>
    </footer>
</body>
</html>

