# DummyAPITesting
How to run it on postman?
1-Open Postman:
Launch the Postman application on your computer. If you haven't installed Postman yet, you can download it from the Postman website.
2-Import into Postman:
Open Postman and click on the "Import" button located in the top-left corner. Select the exported collection file (.json) from your local system and import it into Postman.

3-Review and Organize:
Once imported, review your collection to ensure that all requests, descriptions, and variables are correctly represented. Organize your collections and requests as needed for easier navigation.

4-Set Environment Variables:
If you have environment variables, you can set them in Postman by clicking on the gear icon in the top-right corner, selecting "Manage Environments", and adding/editing variables as necessary.

5-Test Your API:
With your API documentation imported and environment variables set, you can now test your API endpoints directly within Postman. Send requests and verify that you receive the expected responses.

And 
 Here’s a brief explanation 
1.	Get All Employees: This test sends a GET request to the /api/v1/employees endpoint to retrieve all employee data. The test checks for a successful response and then stores the ID of the first employee in an environment variable for use in future requests.


2.	Get Single Employee: This test sends a GET request to the /api/v1/employee/{id} endpoint to retrieve data for a single employee. The test checks for a successful response and the correct response code.

3.	Create Employee: This test sends a POST request to the /api/v1/create endpoint to create a new employee record. The request body includes the employee’s name, salary, and age, which are stored in environment variables to allow for dynamic data. The test checks for a successful response and the correct response code.


4.	Update Employee: This test sends a PUT request to the /api/v1/update/{id} endpoint to update an existing employee record. The request body includes the updated name, salary, and age, which are stored in environment variables to allow for dynamic data. The test checks for a successful response, a ‘success’ message in the response body, and verifies that the updated data is correctly reflected in the response.

5.	Delete Employee: This test sends a DELETE request to the /api/v1/delete/{id} endpoint to delete an existing employee record. The test checks that the deleted employee no longer exists in the list of employees.
In all these tests, environment variables are used to store and manipulate data. This allows for dynamic data in the requests and helps check the correctness of the responses. The tests are designed to ensure that the API is functioning correctly and that it handles data as expected.
