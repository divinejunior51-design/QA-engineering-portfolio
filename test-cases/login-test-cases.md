# Login Feature Test Cases
## Project: Saucedemo 
## Prepared By: Divine Chukwuemerie — Junior QA Engineer

---

### TC_LOGIN_001 — Positive Test Case
**Title:** Verify that a registered user can successfully login with valid credentials.
**Preconditions:** User credentials with username "standard_user" and password "secret_sauce" exist in the system. Tester is on the login page at www.saucedemo.com. No previous login sessions are active.
**Test Steps:**
1. Type "standard_user" into the username field.
2. Type "secret_sauce" into the password field.
3. Click the "Login" button.
**Expected Result:** The user is redirected to the products page at www.saucedemo.com/inventory.html. A list of products is displayed. The page title reads "Products."
**Actual Result:** As expected.
**Status:** Pass.

---

### TC_LOGIN_002 — Negative Test Case
**Title:** Verify that a locked out user cannot login.
**Preconditions:** User credentials with username "locked_out_user" and password "secret_sauce" exist in the system but the account is locked. Tester is on the login page at www.saucedemo.com. No previous login sessions are active.
**Test Steps:**
1. Type "locked_out_user" into the username field.
2. Type "secret_sauce" into the password field.
3. Click the "Login" button.
**Expected Result:** The user remains on the login page. An error message reading "Epic sadface :( Sorry, this user has been locked out." is displayed. The user is unable to login.
**Actual Result:** As expected.
**Status:** Pass.

---

### TC_LOGIN_003 — Edge Case
**Title:** Verify that a user cannot login with a one character username.
**Preconditions:** Tester is on the login page at www.saucedemo.com. No previous login sessions are active.
**Test Steps:**
1. Type "a" into the username field.
2. Type "secret_sauce" into the password field.
3. Click the "Login" button.
**Expected Result:** The user remains on the login page. An error message is displayed stating the username and password do not match any user in the service. The user is unable to login.
**Actual Result:** As expected.
**Status:** Pass.

---

### TC_PURCHASE_001 — Positive Test Case
**Title:** Verify that a registered user can successfully purchase airtime with a valid amount.
**Preconditions:** User is logged in to the app using valid credentials.
**Test Steps:**
1. Type "08087647305" into the phone number field.
2. App detects correct network.
3. Type "₦2000" in the amount field.
4. Click on the "Proceed" button.
5. Input correct PIN in the PIN field.
**Expected Result:** The transaction is completed and the user receives a confirmation notification within 30 seconds of a successful purchase.
**Actual Result:** Not yet executed.
**Status:** Not yet executed.

---

### TC_PURCHASE_002 — Negative Test Case
**Title:** Verify that airtime purchase fails when amount is below minimum threshold of ₦50.
**Preconditions:** Same as TC_PURCHASE_001.
**Test Steps:**
1. Type "08087647305" into the phone number field.
2. App detects correct network.
3. Type "₦49" in the amount field.
4. Click on the "Proceed" button.
5. Input correct PIN in the PIN field.
**Expected Result:** The airtime purchase fails and an error message reading "invalid amount" or similar is displayed within 10 seconds.
**Actual Result:** Not yet executed.
**Status:** Not yet executed.

---

### TC_PURCHASE_003 — Edge Case
**Title:** Verify that airtime purchase fails when alphabetical characters are entered in the amount field.
**Preconditions:** Same as TC_PURCHASE_001.
**Test Steps:**
1. Type "08087647305" into the phone number field.
2. App detects correct network.
3. Type "AB" in the amount field.
4. Click on the "Proceed" button.
5. Input correct PIN in the PIN field.
**Expected Result:** The airtime purchase fails and an error message reading "invalid amount" or similar is displayed within 10 seconds.
**Actual Result:** Not yet executed.
**Status:** Not yet executed.
