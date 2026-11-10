# SauceDemoManual-TESTING
# SauceDemo - Manual Testing

Manual test documentation for the [SauceDemo](https://www.saucedemo.com) e-commerce application.

## Objective

Verify that the core user flows of SauceDemo work as expected: login, product browsing and sorting, cart, checkout and logout.

## Scope

**In scope**
- Login and logout
- Product listing, details and sorting
- Add to cart and remove from cart
- Checkout (information, overview, completion)
- Basic UI and cross-browser checks

**Out of scope**
- Performance and load testing
- Security testing
- Payment gateway integration (not available on the demo site)

## Test Environment

| Item | Details |
|---|---|
| Application URL | https://www.saucedemo.com |
| Browsers | Chrome, Firefox, Edge (latest versions) |
| Operating System | Windows 11 |
| Test Data | Standard user: `standard_user` / `secret_sauce` |

## Test Approach

- Functional testing
- Positive and negative testing
- Boundary and validation testing
- Smoke and regression testing
- Exploratory testing

## Test Scenarios

| ID | Module | Scenario | Type |
|---|---|---|---|
| TS_01 | Login | Login with valid credentials | Positive |
| TS_02 | Login | Login with invalid username or password | Negative |
| TS_03 | Login | Login with empty fields | Negative |
| TS_04 | Login | Login with a locked-out user | Negative |
| TS_05 | Products | Verify all products are displayed with name, price and image | Positive |
| TS_06 | Products | Sort by name (A to Z, Z to A) | Positive |
| TS_07 | Products | Sort by price (low to high, high to low) | Positive |
| TS_08 | Cart | Add a single product to the cart | Positive |
| TS_09 | Cart | Add multiple products and verify the cart badge count | Positive |
| TS_10 | Cart | Remove a product from the cart | Positive |
| TS_11 | Checkout | Complete checkout with valid details | Positive |
| TS_12 | Checkout | Checkout with missing first name, last name or postal code | Negative |
| TS_13 | Checkout | Verify item total, tax and total price | Positive |
| TS_14 | Logout | Logout and verify redirect to the login page | Positive |
| TS_15 | Logout | Press the browser back button after logout | Negative |
| TS_16 | End to End | Login, add items, checkout, logout | Positive |

## Sample Test Case

| Field | Details |
|---|---|
| Test Case ID | TC_LOGIN_01 |
| Title | Login with valid credentials |
| Precondition | User is on the login page |
| Test Data | Username: `standard_user`, Password: `secret_sauce` |
| Steps | 1. Open https://www.saucedemo.com<br>2. Enter the username<br>3. Enter the password<br>4. Click Login |
| Expected Result | User is redirected to the Products page |
| Actual Result | (fill in during execution) |
| Status | Pass / Fail |

## Defect Reporting

Each defect should include:
- Defect ID and title
- Environment and browser version
- Steps to reproduce
- Expected vs actual result
- Severity and priority
- Screenshot or video
- Status (New, Open, Fixed, Retested, Closed)

## Entry and Exit Criteria

**Entry**
- Application is deployed and accessible
- Test cases are reviewed and approved
- Test data is ready

**Exit**
- All planned test cases are executed
- All critical and high defects are fixed and retested
- Test summary report is shared

## Deliverables

- Test scenarios and test cases
- Defect log
- Test summary report

## Author

HYFA RASHEED
