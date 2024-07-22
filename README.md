EXPLANATION OF THE CODE
    Database Configuration: The database connection setup ($host, $db, $user, $pass) remains unchanged assuming it correctly connects to your MySQL database.

    HTML and PHP Integration: All HTML forms and PHP scripts are now correctly integrated within index.php. Each form handles its respective data submission (POST method) and redirects back to index.php after processing.

    Form Handling: Added checks (isset) for form data before calling corresponding add functions to prevent undefined index errors.

    Fetching and Displaying Data: Functions (getStudents(), getTeachers(), getClasses(), getGrades()) fetch data from the database and populate the HTML lists (ul) accordingly.

    Error Handling: Database connection errors are handled within the try-catch block, ensuring graceful termination with an error message if connection fails.

Additional Notes:

    Security: Ensure to validate and sanitize user inputs (especially before database operations) to prevent SQL injection attacks.
    Redirects: After processing form submissions (POST requests), using header("Location: index.php") ensures the page refreshes with updated data, preventing duplicate form submissions.

This code structure should now function correctly for adding students, teachers, classes, and grades in your School Management System (SMS) while displaying lists of existing data.
