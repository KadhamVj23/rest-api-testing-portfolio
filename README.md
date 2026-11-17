# REST API Testing Portfolio – Postman

## Project Overview

This project demonstrates practical REST API testing using Postman. It covers HTTP methods, CRUD operations, negative testing, authentication responses, response headers, schema validation, and basic response-time checks.

The project uses public API testing services to demonstrate API testing concepts and assertion writing.

## Tools & Technologies

- Postman
- REST APIs
- HTTP methods: GET, POST, PUT, DELETE
- JavaScript (Postman test scripts)
- JSON
- GitHub

## Test Scenarios

| Test Case | Scenario | Expected Status |
|---|---|---|
| TC01 | Retrieve a single post | 200 OK |
| TC02 | Retrieve all posts | 200 OK |
| TC03 | Create a post | 201 Created |
| TC04 | Update a post | 200 OK |
| TC05 | Delete a post | 200 OK |
| TC06 | Request a non-existing post | 404 Not Found |
| TC07 | Unauthenticated access | 401 Unauthorized |
| TC08 | Simulated forbidden access | 403 Forbidden |
| TC09 | Response headers validation | 200 OK |
| TC10 | Response schema and data validation | 200 OK |
| TC11 | Simulated bad request | 400 Bad Request |
| TC12 | Response-time and basic performance validation | 200 OK |

## Validations Performed

- HTTP status code validation
- Response-time threshold checks
- JSON response validation
- Required field validation
- Data type validation
- Response header validation
- Empty response and error handling
- Basic API negative testing

## Test Execution

All 12 test cases were executed in Postman. The assertions passed against the responses received during the project runs.

## Important Notes & Limitations

- JSONPlaceholder is a fake REST API. POST, PUT, and DELETE operations simulate changes and do not persist data.
- Postman Echo status endpoints simulate HTTP error responses. They do not validate actual application authorization or input-validation rules.
- The 401 test uses Postman Echo's Basic Auth endpoint without credentials.
- The response-time thresholds are basic checks from individual requests, not load or stress testing.
- This is a learning and demonstration project using public testing services. It does not contain confidential customer or employer data.

## Skills Demonstrated

REST API testing, Postman, HTTP methods, status codes, JSON validation, JavaScript assertions, negative testing, response headers, and basic performance checks.
