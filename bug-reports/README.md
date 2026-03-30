# Bug Reports
## Project: Saucedemo
## Prepared By: Divine Chukwuemerie — Junior QA Engineer

---

### SAUCE-001
**Title:** Checkout First Name and Last Name fields accept single character input without displaying a validation error.
**Environment:** Chrome Version 122, Windows 11, Desktop, www.saucedemo.com
**Preconditions:** User is logged in as standard_user. At least one item has been added to the cart. User has clicked the checkout button and is on the checkout information page.
**Steps to Reproduce:**
1. Type "A" into the First Name field.
2. Type "A" into the Last Name field.
3. Type "10001" into the Zip Code field.
4. Click the Continue button.
**Expected Result:** The system displays a validation error message stating "Please enter more than one character for first name and last name" or similar. The form does not proceed to the next step.
**Actual Result:** The system accepts "A" as a valid first name and "A" as a valid last name without displaying any validation error and proceeds to the checkout overview page.
**Severity:** Medium
**Priority:** High
**Attachments:** Screenshot showing "A" accepted in both fields with the system proceeding to the checkout overview page.

---

### SAUCE-002
**Title:** Product page red t-shirt image displays a sweatshirt instead of a t-shirt.
**Environment:** Chrome Version 122, Windows 11, Desktop, www.saucedemo.com
**Preconditions:** User is logged in as standard_user and is on the products page.
**Steps to Reproduce:**
1. Log in as standard_user.
2. Navigate to the products page.
3. Locate the product named "Sauce Labs Bolt T-Shirt."
4. Observe the product image displayed.
**Expected Result:** The product image shows a red t-shirt matching the product name and description.
**Actual Result:** The product image displays a red sweatshirt instead of a t-shirt, creating a data integrity mismatch.
**Severity:** Low
**Priority:** Medium
**Attachments:** Screenshot showing the mismatched product image.

---

### SAUCE-003
**Title:** Checkout zip code field accepts alphabetical characters without displaying a validation error.
**Environment:** Chrome Version 122, Windows 11, Desktop, www.saucedemo.com
**Preconditions:** User is logged in as standard_user. At least one item has been added to the cart. User is on the checkout information page.
**Steps to Reproduce:**
1. Type "John" into the First Name field.
2. Type "Doe" into the Last Name field.
3. Type "ABCDE" into the Zip Code field.
4. Click the Continue button.
**Expected Result:** The system displays a validation error message stating "Please enter a valid zip code" or similar. The form does not proceed to the next step.
**Actual Result:** The system accepts "ABCDE" as a valid zip code without displaying any validation error and proceeds to the checkout overview page.
**Severity:** Medium
**Priority:** High
**Attachments:** Screenshot showing "ABCDE" accepted in the zip code field.

---

### SAUCE-004
**Title:** Black t-shirt product description does not match its image.
**Environment:** Chrome Version 122, Windows 11, Desktop, www.saucedemo.com
**Preconditions:** User is logged in as standard_user and is on the products page.
**Steps to Reproduce:**
1. Log in as standard_user.
2. Navigate to the products page.
3. Locate the plain black t-shirt product.
4. Compare the product description against the product image.
**Expected Result:** The product image matches the product description accurately.
**Actual Result:** The description mentions "heather gray with red bolt" but the image shows a plain black t-shirt — a clear data integrity mismatch.
**Severity:** Low
**Priority:** Medium
**Attachments:** Screenshot showing the description and image mismatch.

---

### PAYFAST-BUG-001
**Title:** App freezes for 45 seconds before showing success message when exactly ₦50,000 airtime is purchased.
**Environment:** Chrome Version 122, Windows 11, Desktop, PayFast version 1.0.0, Staging environment.
**Preconditions:** User is logged in using valid credentials. A valid phone number has been entered. Network has been detected correctly.
**Steps to Reproduce:**
1. Type "08087647305" into the phone number field.
2. App detects correct network.
3. Type "₦50,000" in the amount field.
4. Click on the "Proceed" button.
5. Input correct PIN in the PIN field.
**Expected Result:** The transaction is completed and the user receives a confirmation notification within 30 seconds as per acceptance criteria.
**Actual Result:** The app freezes for 45 seconds before displaying a success message — exceeding the required 30 second confirmation window by 15 seconds.
**Severity:** High
**Priority:** High
**Attachments:** Screen recording showing the 45 second freeze and delayed success message.
