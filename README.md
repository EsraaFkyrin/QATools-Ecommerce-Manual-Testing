# E-Commerce Web Application — Manual QA Testing

## Project Overview

This project demonstrates end-to-end manual QA testing of the **QATools Playground Shop**, a demo e-commerce web application designed for safe testing practice.

The goal was to validate critical customer journeys and common e-commerce functionality, including product discovery, filters, sorting, product details, wishlist, cart behavior, authentication, checkout, payment options, shipping, and order confirmation.

The project includes structured test cases, execution evidence, exploratory observations, and a documented checkout defect.

## Application Under Test

- **Application:** QATools Playground — Shop
- **URL:** https://playground.qatools.dev/products
- **Testing Type:** Manual Functional Testing
- **Test Environment:** Web / Desktop and Mobile Browser
- **Test Data:** Demo and fictional data only

## Tools Used

- Microsoft Excel — test case design and execution tracking
- Browser Dev/Test Environment — manual execution
- GitHub — project documentation and portfolio hosting
- Screenshots — execution evidence

## Test Coverage

The project covers:

- Product search
- Search boundary and negative scenarios
- Category filtering
- Price filtering
- Sorting and cross-page sorting validation
- Stock availability
- Pagination
- Product details
- Wishlist
- Shopping cart
- Quantity and total calculations
- Authentication validation
- Checkout flow
- Shipping methods
- Payment methods
- Required-field validation
- Order review
- Order confirmation
- Post-order cart state
- Exploratory product-variant observations

## Test Execution Summary

| Metric | Result |
| --- | ---: |
| Total Test Cases | 43 |
| Passed | 39 |
| Failed | 2 |
| Blocked | 2 |
| Not Run | 0 |
| Executed Pass Rate | 95.1% |

### Key Successful Flows

- Product search, filtering, sorting, and pagination
- Add/remove wishlist items
- Add/remove cart items
- Quantity increase/decrease with correct subtotal, tax, and total updates
- Login validation and successful demo authentication
- Checkout shipping form validation
- Payment-method switching
- Review step validation
- Successful end-to-end dummy order placement
- Cart cleanup after successful order

## Confirmed Defect

### BUG-001 — Shipping cost and total do not update when shipping method changes

**Severity:** High  
**Priority:** High  
**Status:** Open

The checkout displays **Standard shipping as free**, but the order summary shows a **$5.99 shipping charge**. Switching between Standard, Express, and Overnight shipping does not update the displayed shipping fee or total.

See [`BUG_REPORTS.md`](BUG_REPORTS.md) for full reproduction steps and evidence.

## Additional Observations

Two exploratory product-variant cases remain **Blocked / Needs Clarification** because expected product requirements are not available:

- Product image does not change after selecting a different color.
- Product Specs continue to display the default color after a different color is selected.

These were intentionally **not classified as confirmed bugs** without a clear requirement.

## Repository Structure

```text
QATools-Ecommerce-Manual-Testing/
├── README.md
├── TEST_EXECUTION_REPORT.md
├── BUG_REPORTS.md
├── QATools_Ecommerce_Manual_QA_Test_Cases.xlsx
└── screenshots/
    ├── search_negative.png
    ├── cart_quantity_calculation.jpg
    ├── checkout_shipping_bug.png
    ├── order_placed.png
    └── login_required_validation.png
```

## Test Case Workbook

The Excel workbook includes:

- Dashboard
- Test Cases
- Observation Log
- Bug Reports
- Usage notes

The test cases include fields such as test case ID, module, scenario, title, priority, test type, preconditions, steps, test data, expected result, actual result, status, severity, bug ID, evidence, execution date, and notes.

## Testing Approach

The project used a mix of:

- Positive testing
- Negative testing
- Boundary value testing
- Input validation testing
- Exploratory testing
- UI consistency testing
- End-to-end testing
- Calculation validation
- Post-condition verification

## Key QA Skills Demonstrated

- Manual test case design
- Test execution and evidence collection
- Functional web testing
- Negative and boundary testing
- Defect identification and documentation
- Severity and priority assessment
- Exploratory testing
- Test reporting
- End-to-end e-commerce flow validation

## Notes

This is a demo storefront. No real payment or personal data was used during testing.
