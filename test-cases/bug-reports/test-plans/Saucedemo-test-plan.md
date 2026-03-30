# Test Plan — Saucedemo
## Test Plan ID: TP_SAUCEDEMO_001
## Prepared By: Divine Chukwuemerie — Junior QA Engineer

---

## Introduction
This test plan covers the functional testing of Saucedemo 2026. Specifically the login page, products page, cart feature, and checkout process. The goal is to verify that all acceptance criteria are met before the planned release date.

---

## Test Scope
**In Scope:**
- Login page — valid credentials, invalid credentials, locked out user, empty field validation
- Products page — product display, sorting, and filtering
- Cart feature — adding items, removing items, and cart count updates
- Checkout process — form validation, order summary, and confirmation

**Out of Scope:**
- About page verification
- Security penetration testing
- Performance testing under load

---

## Test Approach
Manual functional testing using equivalence partitioning and boundary value analysis for all input field validation. API testing using Postman for backend endpoints. Cross-device testing using Chrome DevTools Device Toolbar. Cross-browser testing on Chrome, Firefox, and Safari.

---

## Test Objectives
- Achieve 100% test case execution for all in-scope features within the 5 day test schedule.
- Zero critical or high severity or priority bugs at release.
- All acceptance criteria verified and documented.

---

## Entry Criteria
- Build successfully deployed to staging environment.
- New build has successfully passed smoke test.
- All test cases written and reviewed.
- Test credentials confirmed working — standard_user, locked_out_user, problem_user.

---

## Exit Criteria
- All test cases executed.
- No open critical or high severity or priority bugs.
- All medium and low bugs acknowledged and verified with documented resolution plans.
- Final smoke test passed on release candidate build.

---

## Test Schedule
- Day 1 — Smoke test and test case writing.
- Days 2 and 3 — Test execution across all in-scope features.
- Day 4 — Regression testing and bug verification.
- Day 5 — Final smoke test and release sign-off.

---

## Resource Requirements
- One QA engineer.
- Tools — TestRail for test case management, Jira for bug tracking, Postman for API testing, Chrome DevTools for UI and network inspection.
- Environment — Staging environment with saucedemo test credentials.

---

## Risk Assessment
- Development delay risk — impact is reduced testing window. Mitigation — risk-based testing prioritization ensuring highest-risk features tested first.
- Environment instability risk — impact is inability to execute test cases. Mitigation — daily environment health checks at start of each testing day.
- Browser-specific error risk — impact is bugs missed on non-Chrome browsers. Mitigation — cross-browser testing on Chrome, Firefox, and Safari.
- Test data availability risk — impact is inability to execute credential-specific test cases. Mitigation — verify all test credentials at the start of each testing day.
