# Swag Labs UI Automation

This project aims to built an automation testing framework for [Swag Labs](https://www.saucedemo.com/) website
using Playwright with JavaScript.

- Project URL: https://www.saucedemo.com/

- Packages used: playwright, playwright-core. Jest, chai, allure-playwright, allure-commandline.



## Authors

- [@Kaiseremon](https://github.com/Kaiseremon)



## Objective:

The objective of this project is to perform automated UI and functionality testing, cross-browser execution, screenshot/video capture, and test reporting on Swag Labs website based on the following scenarios:

1. **Test Suite-1-Q1:** Try login with *‘locked_out_user’* and verify the error message.

2. **Test Suite-2-Q2:** Log in with *‘standard_user’*. Then, from the hamburger menu, *reset the App State. Add any three items to the cart. Navigate to the final checkout page, verify the product name and total price. Finish the purchase and verify the successful order message. Then, reset the App State again and log out.

3. **Test Suite-3-Q3:** Login with *‘performance_glitch_user’* and reset the App State. Then filter by name (Z to A) and select the first product into the cart. Then navigate up to the final checkout page and verify all the products' names and the total price. Then finish the purchase journey and verify the successful order message. Then, reset the App State again and log out.



## Prerequisites:

If you have not installed already, the following tools are required to install in order to run this project flawlessly:

- [Node.js and npm](https://nodejs.org/) package manager to run Playwright using JavaScript.  

- [Java JDK 11/17](https://www.oracle.com/java/technologies/downloads/) to run allure-commanline. 

- [VS Code](https://code.visualstudio.com/) as the open-source code editor.

- [Git CLI](https://git-scm.com/install/) to sync with GitHub.



## Documentation

In this project, the UI and feature functionality of the SwagLabs website have been analysed. Based on the analysis, a detailed test case scenarios have been written on the above mentioned test suites to perform automated testing.

This is a page object model (**POM**) based automation framework.

Where **Playwright** is used as the automation tools and **Jest** is used to create the framework.

The framework structure follows Test Driven Development (**TDD**) approach. The detailed test case scenarios can be found in the *'TestScenario.txt'* file inside the *'documents'* folder.
 
Besides, **Allure reporter** is used to get the report after completing the test execution. This helps to generate report and take screenshot when a step become failed.



## Run Locally

In order to run this automation testing framework locally, please refer the following sections carefully:


### 1. Clone the project:

To get the project in your local machine, open a terminal and run the following git command:

```bash
  git clone https://github.com/hridoydas/nopCommerce-automation.git
```

Then Go to the project directory and select the branch swagLabs-automation.

```bash
  cd swagLabs-automation
```


### 2. Install Project Dependencies

Install the necessary project dependencies as defined in the 'package.json' file using npm:

```bash
  npm install
```

To install the Playwright browser binaries (Chromium, Firefox, and Webkit), run the following command:

```bash
  npx playwright install
```

test configuration is available inside: playwright.config.js


===========================================



Run test for Feature-1: Nopcommerce registration feature Test

```bash
  npm run registration
```

Run test for Feature-2: Nopcommerce login feature Test

NOTE: Create a user with Email: hridoy@yopmail.com and Password: Test@@00

```bash
  npm run login
```

Run test for Feature-3: Nopcommerce place order feature Test

```bash
  npm run placeOrder
```

Run the all the features as suite

```bash
  npm run nopCommerce
```

Run all the feature parallely

```bash
  npm run test
```

Get report

```bash
  npm run getReport
```



## Demo

Feature-1: Nopcommerce registration feature Test.

URL: https://drive.google.com/file/d/15dcSjE1mj1hRvMjWboz4zqjbr8PPwhQE/view?usp=sharing

Feature-2: Nopcommerce login feature Test.

URL: https://drive.google.com/file/d/1DWLhmH4fDDFzo_HoQkGCq2b4OWsKyQif/view?usp=drive_link

Feature-3: Nopcommerce place order feature Test.

URL: https://drive.google.com/file/d/1QnDthsfU-xZ2Gu9aoDE75Q33TOmMOY7r/view?usp=sharing

Full suite journey and get allure report.

URL: https://drive.google.com/file/d/1RaTPeka7LPpXMHGQoj6a2vzeJ6e1H2dC/view?usp=sharing


