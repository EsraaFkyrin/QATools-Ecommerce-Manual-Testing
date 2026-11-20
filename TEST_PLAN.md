# Test Plan

## Project

**E-Commerce Web Application — Manual QA Testing**

## Objective

Validate the critical customer journeys of the QATools Playground Shop and identify functional, validation, calculation, and usability issues that could affect the shopping and checkout experience.

## In Scope

- Product search
- Category and price filters
- Sorting
- Stock availability
- Pagination
- Product details
- Wishlist
- Cart operations
- Quantity and totals
- Authentication
- Checkout shipping information
- Shipping methods
- Payment methods
- Order review
- Order confirmation
- Post-order cart state

## Out of Scope

- Real payment processing
- Real email delivery
- Production security testing
- Performance/load testing
- Backend/API validation
- Accessibility audit
- Cross-browser matrix beyond the manually used browsers/devices

## Test Types

- Positive testing
- Negative testing
- Boundary value testing
- Exploratory testing
- Input validation testing
- UI consistency testing
- End-to-end testing
- Calculation validation

## Entry Criteria

- Demo shop is accessible.
- Product catalog loads successfully.
- Demo authentication credentials are available where required.
- Test data can be created without real transactions.

## Exit Criteria

- All planned test cases are executed or formally blocked.
- Critical checkout flows are validated.
- Confirmed defects are documented with reproduction steps and evidence.
- Execution summary is completed.

## Test Data

Only dummy/demo data was used, including the application's provided demo account and fictional shipping information.

## Risks

- Demo application behavior may intentionally include training defects.
- Product requirements are not fully documented, so some exploratory observations require clarification before being classified as confirmed bugs.
- Dynamic demo data or application resets may affect repeatability.

## Deliverables

- Test case workbook
- Test execution report
- Bug report
- Selected screenshots/evidence
- README documentation
