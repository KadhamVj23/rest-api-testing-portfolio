# REST API Testing – Test Execution Report

## 1. Execution Summary

| Metric | Result |
|---|---:|
| Total test cases | 12 |
| Test cases executed | 12 |
| Test cases passed | 12 |
| Test cases failed | 0 |
| Execution tool | Postman |

## 2. Test Execution Results

| ID | Test Scenario | Expected HTTP Status | Actual Result |
|---|---|---|---|
| TC01 | Retrieve single post | 200 | PASS |
| TC02 | Retrieve all posts | 200 | PASS |
| TC03 | Create a post | 201 | PASS |
| TC04 | Update a post | 200 | PASS |
| TC05 | Delete a post | 200 | PASS |
| TC06 | Retrieve non-existing post | 404 | PASS |
| TC07 | Access without authentication | 401 | PASS |
| TC08 | Simulated forbidden response | 403 | PASS |
| TC09 | Validate response headers | 200 | PASS |
| TC10 | Validate response schema and data types | 200 | PASS |
| TC11 | Simulated bad request | 400 | PASS |
| TC12 | Validate response time and response structure | 200 | PASS |

## 3. Key Testing Activities

- Executed GET, POST, PUT and DELETE requests.
- Validated HTTP response status codes.
- Tested negative response scenarios.
- Validated JSON fields and data types.
- Checked response headers and content type.
- Implemented JavaScript assertions in Postman.
- Performed basic response-time checks.

## 4. Observations

- JSONPlaceholder returned an empty JSON object for the non-existing resource scenario.
- The unauthenticated Basic Auth request returned HTTP 401 with a plain-text response.
- Postman Echo was used to simulate HTTP 400 and HTTP 403 responses.
- An initial rate-limiting response (429) was encountered during testing with httpbin. An alternative endpoint was used for the 401 test.
- All final configured test assertions passed during execution.

## 5. Limitations

This project uses public API testing services and is intended as a practical demonstration.

- POST, PUT and DELETE operations on JSONPlaceholder are simulated.
- HTTP 400 and 403 status endpoints simulate responses rather than validating actual application business rules.
- The response-time checks are individual-request checks, not load or stress testing.
- Authentication and authorization testing is limited to the demonstrated public endpoints.

## 6. Conclusion

Successfully completed 12 API test scenarios using Postman, demonstrating REST API testing fundamentals, JavaScript assertions, response validation, negative testing and basic performance checks.
