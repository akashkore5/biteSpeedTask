# API Documentation and Usage Guide

This guide provides information on how to use the BiteSpeed Task API endpoints and run them in Postman.

## BiteSpeed Task API

The BiteSpeed Task API provides an endpoint for identifying contacts based on their email and phone number.

Base URL: https://bitespeedtask-production.up.railway.app/identity
Here only endpoint is accessible with POST method.

## Prerequisites

To run the API endpoints in Postman, make sure you have the following:

- Postman installed on your machine (Download: https://www.postman.com/downloads/)
- Valid API key for authentication

## API Endpoints
https://bitespeedtask-production.up.railway.app/identity

### Identify Contact

This endpoint allows you to identify a contact based on their email and phone number.

- URL: [URL](https://bitespeedtask-production.up.railway.app/identity)
- Method: POST
- Headers: 
    - Key: Content-Type, Value: application/json
    - Key: API-Key, Value: [[Your Endpoint Key]](https://bitespeedtask-production.up.railway.app/identity)
- Body (Example):
    ```
    {
        "email": "example@example.com",
        "phoneNumber": "1234567890"
    }
    ```

### Response

The response will contain the details of the identified contact or a newly created contact if no match is found.

Example Response:
```
{
    "contact": {
        "primaryContactId": 1,
        "emails": ["example@example.com"],
        "phoneNumbers": ["1234567890"],
        "secondaryContactIds": [2]
    }
}
```

## Running the API Endpoints in Postman

To run the API endpoints in Postman, follow these steps:

1. Open Postman on your machine.
2. Set the request URL to the appropriate endpoint URL (e.g., https://bitespeedtask-production.up.railway.app/identity).
3. Set the necessary headers:
   - Key: Content-Type, Value: application/json
   - Key: API-Key, Value: [Your API Key]
4. Add the request body in the JSON format as shown in the example above.
5. Click the "Send" button to make the API request.
6. View the response from the API in the Postman response pane.

## Additional Links

- [Resume]([https://your-resume-link.com](https://drive.google.com/file/d/1L_KCcIBjF8h-AthIZlS-wkB1vuOJffmK/view?usp=drive_link)) - Link to resume.

Feel free to reach out if you have any questions or need further assistance.
