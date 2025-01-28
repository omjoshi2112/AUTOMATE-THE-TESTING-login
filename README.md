# task 02

COMPANY NAME: CODTECH IT SOLUTION PVT.LTD

NAME: OM JOSHI

INTER ID: CT6WKCL.

DOMAIN: SOFTWARE TESTING.

BATCH DURATION: January 5th,2025 to February 20TH,2025.

MENTOR NAME: NEELA SANTHOSH

DESCRIPTION : TEST RESTFUL APIS USING POSTMAN FOR FUNCTIONALITIES LIKE AUTHENTICATION AND DATA RETRIEVAL.

Install Postman:
Download and install from Postman’s website.

Set Up Authentication:
Open Postman, create a request, and add the API URL.

Go to the Authorization tab:
Choose Bearer Token, Basic Auth, or the required method.
Enter the token, username/password, or other credentials.

Test Authentication:
Send the request to the login/auth endpoint (e.g., POST /auth/login).
Verify the response status (200 for success) and save tokens if provided.
Test Data Retrieval:

Create a GET request for a data endpoint (e.g., /users).
Add the required headers (e.g., Authorization: Bearer <token>).
Send the request and verify the response data.

Validate Responses:
Check the status code (e.g., 200 for success).
Inspect the response body for expected data.

Save and Organize:
Save requests into a Postman Collection for reusability.

Optional: Write Tests:
Add scripts in the Tests tab to automate validation:

pm.test("Status code is 200", () =>
{
    pm.response.to.have.status(200);
}
);

pm.test("Response contains data", () => {
    const jsonData = pm.response.json();
    pm.expect (jsonData).to.have.property("id");
});

-------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------
DESCRIPTION: DELIVERABLE A POSTMAN COLLECTION AND DOCUMENTATION OF TEST RESULTS.

Postman Collection
Create and organize API requests for authentication and data retrieval.
Save headers, parameters, and request bodies in Postman.
Export the collection:
Go to Collections → Click three dots → Export → Save as a JSON file.
Test Results Documentation

Run the collection using Collection Runner in Postman.
Export results:
After running tests, click Export Results and save as a CSV or JSON file.
Document key observations like:
Status codes (e.g., 200, 401).
Response times and data validation.
