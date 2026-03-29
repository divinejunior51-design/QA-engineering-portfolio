# API Test Suite
## Prepared By: Divine Chukwuemerie — Junior QA Engineer

---

## User Registration API Test Cases
### Base URL: /api/register

---

### API_REG_001 — Happy Path
**Title:** Verify successful user registration with valid credentials
**Method:** POST
**URL:** /api/register
**Request Body:**
```json
{
  "name": "Legacy",
  "email": "legacy@test.com",
  "password": "Password123"
}
```
**Expected Status Code:** 201
**Expected Response:** Response body contains the new user's ID, name, and email. Password is not returned in the response for security reasons.

---

### API_REG_002 — Missing Email
**Title:** Verify that user registration fails when email field is empty
**Method:** POST
**URL:** /api/register
**Request Body:**
```json
{
  "name": "Legacy",
  "email": "",
  "password": "Password123"
}
```
**Expected Status Code:** 400
**Expected Response:** Response body contains an error message stating "email field is required" or similar. No user account is created.

---

### API_REG_003 — Invalid Email Format
**Title:** Verify that user registration fails when email format is invalid
**Method:** POST
**URL:** /api/register
**Request Body:**
```json
{
  "name": "Legacy",
  "email": "legacyATtest.com",
  "password": "Password123"
}
```
**Expected Status Code:** 400
**Expected Response:** Response body contains an error message stating "email field is invalid" or similar. No user account is created.

---

### API_REG_004 — Password Too Short
**Title:** Verify that user registration fails when password is below minimum length
**Method:** POST
**URL:** /api/register
**Request Body:**
```json
{
  "name": "Legacy",
  "email": "legacy@test.com",
  "password": "Pass"
}
```
**Expected Status Code:** 400
**Expected Response:** Response body contains an error message stating "password is too short" or similar. No user account is created.

---

## JSONPlaceholder API Test Results
### Base URL: https://jsonplaceholder.typicode.com

---

### GET All Users
**Method:** GET
**URL:** /users
**Expected Status Code:** 200
**Actual Status Code:** 200 ✅
**Response:** 10 users returned with complete profile data including id, name, username, email, address, phone, website, and company fields.

---

### GET Single User
**Method:** GET
**URL:** /users/1
**Expected Status Code:** 200
**Actual Status Code:** 200 ✅
**Response:** Single user object returned for user ID 1 — Leanne Graham.

---

### GET Non-Existent User
**Method:** GET
**URL:** /users/999
**Expected Status Code:** 404
**Actual Status Code:** 404 ✅
**Response:** Empty response confirming user 999 does not exist.

---

### POST Create New User
**Method:** POST
**URL:** /users
**Request Body:**
```json
{
  "name": "Divine",
  "username": "divine_qa",
  "email": "divine@test.com"
}
```
**Expected Status Code:** 201
**Actual Status Code:** 201 ✅
**Response:** New user created with auto-generated ID 11.

---

### PUT Update User
**Method:** PUT
**URL:** /users/1
**Request Body:**
```json
{
  "name": "Divine Updated",
  "email": "divine_updated@test.com"
}
```
**Expected Status Code:** 200
**Actual Status Code:** 200 ✅
**Response:** Updated user object returned with ID 1 confirming correct record was updated.

---

### DELETE User
**Method:** DELETE
**URL:** /users/1
**Expected Status Code:** 200
**Actual Status Code:** 200 ✅
**Response:** Empty response confirming successful deletion.
