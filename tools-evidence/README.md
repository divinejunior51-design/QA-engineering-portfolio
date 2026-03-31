# Tools Hands-On Evidence
## Prepared By: Divine Chukwuemerie — Junior QA Engineer

---

## Jira — Bug Tracking
**Account:** divinechukwuemerie.atlassian.net
**Project:** QA Testing

### Tickets Created
**DEV-5:** Checkout First Name and Last Name fields accept single character input without displaying a validation error.
- Status: Resolved and closed.
- Complete defect lifecycle executed — To Do, In Progress, Done.
- Developer comment added simulating fix notification.

**DEV-6:** Product page red t-shirt image displays a sweatshirt instead of a t-shirt.
- Status: Created and logged in To Do column.

### Skills Demonstrated
Bug report creation, defect lifecycle management, developer comment simulation, board navigation, backlog management.

---

## TestRail — Test Case Management
**Account:** nerieqa.testrail.io
**Project:** Saucedemo QA Portfolio

### Test Cases Created
- C46 — Verify that a registered user can successfully login with valid credentials. Type: Functional. Priority: High.
- C47 — Verify that a locked out user cannot login. Type: Functional. Priority: High.
- C48 — Verify that a user cannot login with a one character username. Type: Functional. Priority: Medium.

### Test Run Created
Test Run 3/26/2026 — Sprint 1 login feature testing for Saucedemo QA Portfolio.

### Execution Results
- T105 — Passed. Actual result recorded. Version: Saucedemo 2026. Elapsed: 2 minutes.
- T106 — Passed. Actual result recorded. Version: Saucedemo 2026. Elapsed: 2 minutes.
- T107 — Passed. Actual result recorded. Version: Saucedemo 2026. Elapsed: 2 minutes.

### Final Results
3 Passed. 0 Failed. 0 Blocked. Pass rate: 100%.

---

## Chrome DevTools — UI and Network Inspection
**Website Tested:** www.saucedemo.com

### Elements Tab Findings
Login button element inspected revealing id="login-button", class="submit-button btn_action", data-test="login-button", value="Login", type="submit". Confirmed button is correctly identified for automation testing via data-test attribute. CSS color temporarily modified to verify style editing capability.

### Console Tab Findings
Two console errors observed on page load before any user interaction.
- Error 1: POST request to backtrace.io returning ERR_INTERNET_DISCONNECTED. Investigation confirmed background error tracking service with no user impact. Not reported as bug.
- Error 2: CORS policy blocking access to backtrace.io. Investigation confirmed third-party service blocked by browser security. No user impact. Not reported as bug.

### Network Tab Findings
Saucedemo identified as Progressive Web App running via Service Worker — operates from local storage without live server API calls. All network requests observed were GET requests returning 200 status codes for static assets.

### Device Toolbar Findings
Tested saucedemo across iPhone SE (375x667), iPad Air, iPhone 14 Pro, Samsung Galaxy S8, and iPad Mini. Layout adapted correctly across all device sizes. Login functionality confirmed working on all simulated devices. No mobile-specific bugs identified.

---

## Postman — API Testing
**API Tested:** JSONPlaceholder (https://jsonplaceholder.typicode.com)

### Requests Executed
- GET /users — 200 ✅ — 10 users returned with complete profile data
- GET /users/1 — 200 ✅ — Single user object returned correctly
- GET /users/999 — 404 ✅ — Non-existent user correctly returned 404
- POST /users — 201 ✅ — New user created with auto-generated ID
- PUT /users/1 — 200 ✅ — Existing user updated successfully
- DELETE /users/1 — 200 ✅ — User deleted successfully

### Skills Demonstrated
GET/POST/PUT/DELETE request execution, JSON body construction, status code validation, response data validation, negative testing with non-existent resources, basic authentication testing using httpbin.org.
