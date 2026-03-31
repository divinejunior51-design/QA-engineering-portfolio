# Exploratory Testing Session — Saucedemo
## Prepared By: Divine Chukwuemerie — Junior QA Engineer
## Date: March 2026
## Session Duration: 15 minutes
## Mission: Explore the product listing and checkout pages and find anything unexpected or potentially buggy.

---

## Session Summary
Four confirmed bugs were found during this exploratory testing session. Two bugs were found in the checkout feature and two were found on the products page. No critical or high severity bugs were identified.

---

## Finding 1 — Confirmed Bug
**Area:** Checkout — Zip Code Field
**Observation:** The zip code field accepts alphabetical characters without displaying any validation error.
**Expected Behavior:** The field should only accept numerical digits and display a validation error for alphabetical input.
**Severity:** Medium
**Logged As:** SAUCE-003

---

## Finding 2 — Confirmed Bug
**Area:** Checkout — Name Fields
**Observation:** The First Name and Last Name fields accept a single character input without validation.
**Expected Behavior:** The fields should require more than one character and display a validation error for single character input.
**Severity:** Medium
**Logged As:** SAUCE-001

---

## Finding 3 — Confirmed Bug
**Area:** Products Page — Red T-Shirt
**Observation:** The red t-shirt product image displays a sweatshirt instead of a t-shirt.
**Expected Behavior:** The product image should match the product name and description accurately.
**Severity:** Low
**Logged As:** SAUCE-002

---

## Finding 4 — Confirmed Bug
**Area:** Products Page — Black T-Shirt
**Observation:** The plain black t-shirt description mentions "heather gray with red bolt" but the image shows a plain black shirt.
**Expected Behavior:** The product description should accurately match the product image.
**Severity:** Low
**Logged As:** SAUCE-004

---

## Finding 5 — False Positive (Not a Bug)
**Area:** Console Tab — Chrome DevTools
**Observation:** CORS policy error blocking access to backtrace.io error tracking service.
**Investigation Result:** This is a background third-party error tracking service with no impact on user experience. Not reported as a bug.

---

## Finding 6 — By Design
**Area:** Cart Feature
**Observation:** Cannot add the same item twice to the cart.
**Investigation Result:** This is intentional behavior for the saucedemo demo application. On a real e-commerce site this would be investigated against requirements before making a determination.

---

## Tools Used
- Chrome DevTools — Elements Tab, Console Tab, Network Tab
- Bug Magnet Chrome Extension for edge case input generation
- Saucedemo credentials — standard_user / secret_sauce
