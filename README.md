# TestAutomation-Healthcare-Website

## Overview
The One Health Website Automation framework is designed to ensure the reliability and functionality of the website through automated testing. Built using Selenium WebDriver and TestNG, the framework allows for efficient and scalable testing of all website pages, including user interactions, form submissions, and data validations. The code is organized using the Page Object Model (POM) design pattern, which enhances readability and maintainability. This automation setup supports cross-browser testing, data-driven testing, and integrates seamlessly with CI/CD pipelines, making it a robust solution for continuous testing and quality assurance.

## Key Features
- Configures WebDriver (ChromeDriver) and opens One Health website.
- Maximizes browser window for test consistency.
- Simulates smooth scrolling on the home page via JavaScript and keyboard actions.
- Fills and submits the registration form, verifies success message.
- Generates alert messages when necessary.
- Navigates and performs operations on About, Doctors, and Blog pages.
- Handles forms efficiently.
- Interacts with Google Map on Contact page: zoom in/out, landscape view.
- Implements data-driven TestLogin with DataProvider for multiple credentials.



## Prerequisites
- **Java Development Kit (JDK):** Version 8 or higher.
- **Maven:** For managing dependencies and running tests.
- **IDE:** IntelliJ IDEA, Eclipse, or any other Java IDE.
- **Web Browser:** Chrome, Firefox, etc., with respective WebDriver binaries.

## Setup and Installation 

Clone the repository: 

```bash
  https://github.com/Wisteriaa9/TestAutomation-Healthcare-Website.git
```

Install dependencies: 
```bash
  mvn clean install
```
Configure Webdriver: 

- Place the WebDriver binaries (e.g., chromedriver, geckodriver) in a location accessible to your system.
- Update the WebDriver path in the config/WebDriverConfig.java file.


## Test Structure

- **Page Object Model (POM):** pages/: Contains Java classes representing each page of the One Health Website. Each class includes web elements identified using Selenium and methods to interact with those elements. 
- **Test Cases:** tests/: Contains the actual test cases, organized by page. Each test class corresponds to a particular page and includes tests for all functionalities on that page.
- **Test Data:** testdata/: Stores external data used in test cases, such as Excel files or JSON files for parameterized testing.
- **Utilities:** utils/: Contains reusable utility methods such as reading from configuration files, handling waits, and capturing screenshots.
- **Explicit Waits:** Ensures robust and reliable tests by using explicit waits for elements to load, reducing flakiness.

## Reporting
- **TestNG Reports:** After running the tests, reports are generated under the test-output/ directory. Open the index.html file in a browser to view detailed results.









