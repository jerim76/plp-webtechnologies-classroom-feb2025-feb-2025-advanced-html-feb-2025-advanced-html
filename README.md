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
- <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Sample HTML page with various elements">
    <title>Sample HTML5 Page</title>
    <style>
        /* Basic styling for better presentation */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
            color: #333;
        }
        h1, h2 {
            color: #2c3e50;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
        form {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 5px;
            margin-top: 20px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        button {
            background-color: #3498db;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #2980b9;
        }
        .radio-group, .checkbox-group {
            margin: 10px 0;
        }
        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 20px 0;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <!-- Main header for the page -->
    <header>
        <h1>Sample HTML5 Page</h1>
    </header>

    <!-- Main content section -->
    <main>
        <!-- Section with ordered list -->
        <section>
            <h2>Steps to Success (Ordered List)</h2>
            <ol type="I">
                <li>Define your goals</li>
                <li>Create a plan</li>
                <li>Take action</li>
                <li>Review progress</li>
                <li>Adjust as needed</li>
            </ol>
        </section>

        <!-- Section with external image from Pexels -->
        <section>
            <h2>Inspirational Image</h2>
            <img src="https://images.pexels.com/photos/3183150/pexels-photo-3183150.jpeg" 
                 alt="Team collaboration meeting" 
                 title="Photo by fauxels from Pexels">
            <p>Image source: <a href="https://www.pexels.com/" target="_blank">Pexels.com</a></p>
        </section>

        <!-- Section with contacts table -->
        <section>
            <h2>Contact Directory</h2>
            <table>
                <thead>
                    <tr>
                        <th>Name</th>
                        <th>Address</th>
                        <th>Mobile</th>
                        <th>Email</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>John Doe</td>
                        <td>123 Main St, Nairobi</td>
                        <td>0712345678</td>
                        <td>john@example.com</td>
                    </tr>
                    <tr>
                        <td>Jane Smith</td>
                        <td>456 Park Ave, Mombasa</td>
                        <td>0723456789</td>
                        <td>jane@example.com</td>
                    </tr>
                    <tr>
                        <td>Robert Johnson</td>
                        <td>789 Hill Rd, Kisumu</td>
                        <td>0734567890</td>
                        <td>robert@example.com</td>
                    </tr>
                    <tr>
                        <td>Sarah Williams</td>
                        <td>321 Valley Dr, Nakuru</td>
                        <td>0745678901</td>
                        <td>sarah@example.com</td>
                    </tr>
                    <tr>
                        <td>Michael Brown</td>
                        <td>654 Lake View, Eldoret</td>
                        <td>0756789012</td>
                        <td>michael@example.com</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <!-- Registration form section -->
        <section>
            <h2>Registration Form</h2>
            <form id="registrationForm" method="post" action="#">
                <!-- Name field -->
                <div class="form-group">
                    <label for="fullName">Full Name:*</label>
                    <input type="text" id="fullName" name="fullName" 
                           placeholder="Enter your full name" 
                           required minlength="3" maxlength="50">
                </div>

                <!-- Email field -->
                <div class="form-group">
                    <label for="email">Email Address:*</label>
                    <input type="email" id="email" name="email" 
                           placeholder="example@domain.com" 
                           required>
                </div>

                <!-- Password field -->
                <div class="form-group">
                    <label for="password">Password:*</label>
                    <input type="password" id="password" name="password" 
                           placeholder="Create a password (min 8 characters)" 
                           required minlength="8">
                </div>

                <!-- Date of birth field -->
                <div class="form-group">
                    <label for="dob">Date of Birth:*</label>
                    <input type="date" id="dob" name="dob" required>
                </div>

                <!-- Dropdown for country selection -->
                <div class="form-group">
                    <label for="country">Country:</label>
                    <select id="country" name="country">
                        <option value="">Select your country</option>
                        <option value="kenya">Kenya</option>
                        <option value="uganda">Uganda</option>
                        <option value="tanzania">Tanzania</option>
                        <option value="rwanda">Rwanda</option>
                        <option value="other">Other</option>
                    </select>
                </div>

                <!-- Radio buttons for gender -->
                <div class="form-group">
                    <label>Gender:</label>
                    <div class="radio-group">
                        <input type="radio" id="male" name="gender" value="male">
                        <label for="male" class="inline-label">Male</label>
                        
                        <input type="radio" id="female" name="gender" value="female">
                        <label for="female" class="inline-label">Female</label>
                        
                        <input type="radio" id="other" name="gender" value="other">
                        <label for="other" class="inline-label">Other</label>
                    </div>
                </div>

                <!-- Checkboxes for interests -->
                <div class="form-group">
                    <label>Interests (Select all that apply):</label>
                    <div class="checkbox-group">
                        <input type="checkbox" id="sports" name="interests" value="sports">
                        <label for="sports" class="inline-label">Sports</label><br>
                        
                        <input type="checkbox" id="music" name="interests" value="music">
                        <label for="music" class="inline-label">Music</label><br>
                        
                        <input type="checkbox" id="reading" name="interests" value="reading">
                        <label for="reading" class="inline-label">Reading</label><br>
                        
                        <input type="checkbox" id="travel" name="interests" value="travel">
                        <label for="travel" class="inline-label">Travel</label>
                    </div>
                </div>

                <!-- Additional comments -->
                <div class="form-group">
                    <label for="comments">Additional Comments:</label>
                    <textarea id="comments" name="comments" 
                              rows="4" 
                              placeholder="Any additional information..."></textarea>
                </div>

                <!-- Terms and conditions checkbox -->
                <div class="form-group">
                    <input type="checkbox" id="terms" name="terms" required>
                    <label for="terms" class="inline-label">I agree to the terms and conditions*</label>
                </div>

                <!-- Form submission buttons -->
                <div class="form-group">
                    <button type="submit">Register</button>
                    <button type="reset">Reset Form</button>
                </div>
            </form>
        </section>
    </main>

    <!-- Page footer -->
    <footer>
        <p>&copy; 2023 Sample HTML Page. All rights reserved.</p>
    </footer>
</body>
</html>
- Ensure semantic correctness.

Happy Coding! 💻✨
