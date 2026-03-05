# Playwright Testing Demo

This repository demonstrates automated testing using Playwright,
including several key testing features such as assertions, mocking, and
CI/CD integration.

The project uses the demo site SauceDemo and the public API ReqRes to
showcase testing techniques.

------------------------------------------------------------------------

# Project Features

This project demonstrates the following Playwright features:

-   Assertions for validating UI elements
-   Mocking API responses
-   Automated test execution
-   Cross-browser testing (Chromium, Firefox, WebKit)
-   CI/CD pipeline integration with GitHub Actions

------------------------------------------------------------------------

# Project Structure

    Playwright-demo
    │
    ├── tests
    │   ├── assertion.spec.js
    │   ├── fixturetest.spec.js
    |   ├── mockingtest.spec.js
    │
    ├── playwright.config.js
    ├── package.json
    └── .github/workflows/playwright.yml

**tests/**\
Contains Playwright test files demonstrating different testing features.

------------------------------------------------------------------------

# Installation

Clone the repository:

``` bash
git clone https://github.com/zero3nine/Playwright-demo.git
cd Playwright-demo
```

Install dependencies:

``` bash
npm install
```

Install Playwright browsers:

``` bash
npx playwright install
```

------------------------------------------------------------------------

# Running Tests

Run all tests:

``` bash
npx playwright test
```

Run tests with the UI runner:

``` bash
npx playwright test --ui
```

View the test report:

``` bash
npx playwright show-report
```

------------------------------------------------------------------------

# CI/CD Integration

This project uses GitHub Actions to automatically run tests whenever
code is pushed to the repository or a pull request is created.

Workflow file:

    .github/workflows/playwright.yml

The pipeline performs the following steps:

1.  Checks out the repository
2.  Installs Node.js
3.  Installs project dependencies
4.  Installs Playwright browsers
5.  Runs automated tests
6.  Uploads the Playwright test report as an artifact

This ensures tests run automatically without requiring manual execution.

------------------------------------------------------------------------

# Tools Used

-   Playwright -- End-to-end testing framework
-   Node.js -- Runtime environment
-   GitHub Actions -- CI/CD automation
-   SauceDemo -- Demo website for UI testing
-   ReqRes API -- Public API used for mocking tests

------------------------------------------------------------------------