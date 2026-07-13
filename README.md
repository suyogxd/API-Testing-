# REST API Testing Portfolio

A manual API testing project performed on publicly available REST APIs using Postman and Swagger. This project demonstrates test case design, API validation, CRUD operation testing, status code verification, response validation, positive testing, negative testing, and defect identification.

**JSON Placeholder Test Case:** https://docs.google.com/spreadsheets/d/1VP0phg78CnZvuRJhYW7mGTvEl4WGrMd_PLhN_k6hu1o?gid=0#gid=0
**FakeRest API Test Case:** https://docs.google.com/spreadsheets/d/1VP0phg78CnZvuRJhYW7mGTvEl4WGrMd_PLhN_k6hu1o?gid=1551511402#gid=1551511402
**Swagger Petstore API:** https://docs.google.com/spreadsheets/d/1VP0phg78CnZvuRJhYW7mGTvEl4WGrMd_PLhN_k6hu1o?gid=1354569764#gid=1354569764

---

## Project Objective

The objective of this project is to validate the functionality, reliability, and response behavior of REST APIs by executing comprehensive test scenarios covering:

- GET Operations
- POST Operations
- PUT Operations
- PATCH Operations
- DELETE Operations
- Positive Testing
- Negative Testing
- Boundary Testing
- Request Validation
- Response Validation
- Status Code Validation

---

# APIs Tested

## 1. JSONPlaceholder

API URL: https://jsonplaceholder.typicode.com

### Modules Tested

- Posts
- Comments

### Operations Tested

- GET
- POST
- PUT
- PATCH
- DELETE

### Test Coverage

- Fetch all records
- Fetch single record
- Fetch invalid records
- Create records
- Update complete records
- Update partial records
- Delete records
- Validate invalid IDs
- Validate empty requests

### Defects Identified

- Invalid Post ID comments return empty array instead of 404.
- Invalid query parameters return 200 instead of error response.
- Deleting non-existing records returns 200 instead of 404.

---

## 2. FakeRestAPI

API URL: https://fakerestapi.azurewebsites.net

### Modules Tested

#### Activities

- GET
- POST
- PUT
- DELETE

#### Authors

- GET
- POST
- PUT
- DELETE

#### Books

- GET
- POST
- PUT
- DELETE

### Test Coverage

- Fetch valid records
- Fetch invalid records
- Create records
- Create incomplete records
- Create empty records
- Update records
- Delete records
- Boundary testing
- Input validation testing

### Defects Identified

- POST requests return 200 instead of expected 201 Created.
- Custom fields are ignored during record creation.
- Invalid DELETE requests return success instead of 404.
- Invalid book and author references return 200 responses with empty arrays.

---

## 3. Swagger Petstore

API URL: https://petstore.swagger.io

### Module Tested

- Pet

### Operations Tested

- GET
- POST
- PUT

### Test Coverage

- Create pet
- Update pet
- Search pet by ID
- Search pet by status
- Validate invalid IDs
- Form-data update testing
- Boundary testing

### Defects Identified

- Additional custom fields are ignored during pet creation.
- Some error scenarios return HTTP 200 with error messages in the response body.

---

# Test Execution Summary

## JSONPlaceholder

| Result | Count |
|----------|----------|
| Passed | 20 |
| Failed | 5 |

---

## FakeRestAPI

| Module | Passed | Failed |
|----------|----------|----------|
| Activities | 12 | 2 |
| Authors | 15 | 3 |
| Books | 10 | 2 |

---

## Swagger Petstore

| Result | Count |
|----------|----------|
| Passed | 15 |
| Failed | 1 |

---

# Tools Used

- Postman
- Swagger UI
- Google Sheets

---

# Test Documentation

Google Sheets documentation:

- JSONPlaceholder Test Cases
- FakeRestAPI Test Cases
- Swagger Petstore Test Cases

---

# Skills Demonstrated

- REST API Testing
- Manual Testing
- CRUD Validation
- Positive Testing
- Negative Testing
- Boundary Value Analysis
- Defect Reporting
- API Response Validation
- Postman
- Test Case Design
- Test Execution
- Bug Documentation

---

# Author

**Suyog Sharma**

Manual QA / API Testing Portfolio Project
