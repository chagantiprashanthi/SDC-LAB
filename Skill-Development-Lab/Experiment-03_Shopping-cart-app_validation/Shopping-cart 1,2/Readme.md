 Program 3: Client-Side Validation Using JavaScript


1. Aim
To implement client-side validation using JavaScript for a registration form and a shopping cart page.

2. Requirements
•Software: Google Chrome, VS Code / Any Text Editor
•Technologies: HTML, CSS, JavaScript
![Screenshot (17)](https://github.com/user-attachments/assets/d9f9a0ba-344a-4495-92d1-38941571450a)

![Screenshot (18)](https://github.com/user-attachments/assets/3c611137-c377-4ead-959c-9698694865c1)
![Screenshot (19)](https://github.com/user-attachments/assets/2b121b8e-68dd-49b0-b718-cab8ccacd5c6)
![Screenshot (20)](https://github.com/user-attachments/assets/f3475e38-17ca-437c-8c0a-a39c722131a0)



3. Theory
SDC observation
Client-side validation ensures that form inputs meet the required format before being sent to the server. JavaScript functions are used to check user input dynamically, preventing invalid data from being submitted and improving the user experience.

4. Features

4.1 Registration Form Validation
•Validates user input fields (name, email, and password).
•Ensures all fields are filled.
•Uses a regular expression to validate email format.
•Checks that the password is at least 6 characters long.
•Displays an alert for invalid input.

4.2 Shopping Cart Validation
•Retrieves cart items from localStorage.
•Validates quantity (must be a positive number).
•Displays an alert for incorrect input.
•Dynamically updates the total price.

5. Usage
1.Open the registration form and enter details.
2.Click the submit button to trigger validation.
3.Navigate to the shopping cart and check the quantities.
4.Adjust item quantities, ensuring all inputs are valid.
5.The total price updates dynamically.

6. Implementation
The validation logic is implemented using JavaScript. The registration form ensures valid inputs before submission, while the shopping cart checks item quantities and updates the total price accordingly.

7. License
This project is open-source and free to use.
