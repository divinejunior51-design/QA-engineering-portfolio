# Test Summary Report — Saucedemo
## Report ID: TSR_SAUCEDEMO_001
## Prepared By: Divine Chukwuemerie — Junior QA Engineer
## Sprint: Sprint 1 — March 2026
## Reporting Date: March 19 2026

---

## Traffic Light Status: 🟡 AMBER

---

## Executive Summary
Exploratory testing of the Saucedemo webpage was completed across a 2 day sprint. A total of 10 test cases were executed achieving 100% test case execution with a 60% pass rate. Four bugs were identified and remain unresolved. The feature is recommended for release with conditions — all open bugs are Medium and Low severity, documented as known issues with product manager approval required before release. A follow-up fix sprint is recommended to resolve all four open bugs.

---

## Test Scope Summary
**In Scope:** Exploratory testing of the Saucedemo webpage, verification of login feature, validation of the checkout process, and inspection of the products page.
**Out of Scope:** Security strength testing, Saucedemo backend system.
All in-scope items were tested. None were left untested.

---

## Test Execution Summary
- Total test cases planned: 10
- Total executed: 10
- Passed: 6
- Failed: 4
- Blocked: 0
- Pass rate: 60%

---

## Defect Summary
- Total bugs found: 4
- Critical: 0
- High: 0
- Medium: 2 — not fixed yet
- Low: 2 — not fixed yet
- Open bugs at release: 0 critical, 0 high, 2 medium, 2 low.

---

## Test Environment Details
- Browser: Chrome Version 122
- Operating System: Windows 11
- Device: Desktop
- Application Version: Saucedemo 2026
- Test Environment URL: www.saucedemo.com

---

## Risks and Observations
Two of the four bugs found were concentrated in the checkout feature. The remaining two were found on the products page as data integrity issues. The concentration of bugs in the checkout feature suggests the checkout validation logic may benefit from a developer code review before the next sprint.

---

## Recommendations
The Saucedemo application is recommended for release with conditions. All four open bugs are Medium and Low severity. All open bugs must be documented as known issues with explicit product manager approval before release. A follow-up fix sprint is strongly recommended to resolve all four open bugs.

---

## Sign-off
- QA Engineer: Divine Chukwuemerie — Approved
- QA Lead: Pending Approval
- Product Manager: Pending Approval

---

# Release Readiness Report — QuickPay
## Report ID: TSR_QUICKPAY_001
## Project: QuickPay Lagos Fintech
## Feature: Bill Payment
## Prepared By: Divine Chukwuemerie — Junior QA Engineer

---

## Traffic Light Status: 🟡 AMBER

The Bill Payment feature has achieved an 89.5% pass rate with all critical and high severity defects fully resolved and verified. However three open defects remain deferred to the next sprint and two test cases were not executed, which prevents a full green classification.

---

## Executive Summary
The QuickPay team completed a full round of quality checks on the new Bill Payment feature, testing nearly everything on the plan and passing the vast majority of scenarios. The most serious problems found — including one that could have significantly disrupted customers — were all fixed and confirmed before this report was written. Three smaller issues were intentionally set aside with the Product Manager's approval, as they do not affect the core bill payment flow. Overall the feature is in a healthy state and the team is confident it can go live with a short list of known follow-up items to address in the next cycle.

---

## Open Items Summary
- Item 1 — Severity: Medium. Status: Open, Deferred with PM approval. Business Impact: May cause minor friction in edge-case payment scenarios.
- Item 2 — Severity: Medium. Status: Open, Deferred with PM approval. Business Impact: Same risk profile as Item 1.
- Item 3 — Severity: Low. Status: Open, Deferred with PM approval. Business Impact: Negligible immediate business risk.

---

## Release Recommendation
RECOMMENDED WITH CONDITIONS. All critical and high severity bugs have been fixed and verified. Three deferred items carry PM-level approval. Production monitoring should be configured for the payment flow. All deferred items must be resolved in the next sprint.

---

## Sign-off
- QA Engineer: Divine Chukwuemerie — Approved
- QA Lead: Pending Approval
- Product Manager: Pending Approval
