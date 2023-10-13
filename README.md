# Bank API Automation for International Conversions

This project automates API testing to retrieve the average exchange rate of a chosen currency over the last 10 weeks. It utilizes Cypress to ensure that the API endpoints are working correctly and provides accurate historical exchange rate data. The results are presented in a user-friendly HTML report generated using the Cypress HTML Reporter.

## Installation

To start this project, you need to have Cypress and the Cypress HTML Reporter installed on your machine. Follow these steps to set up your environment:

**Prerequisites:**

   - [Node.js](https://nodejs.org/) should be installed on your machine.

## Installation

 
   ```shell
   npm Install 
   npm install cypress --save-dev
   ```

## Running Cypress Tests

  ```
  npx cypress open
  ```

## Running Cypress Mochawesome Reporter

  ```
  npx cypress run --e2e
  ```

After running the command you can find the report on an HTML file in the reports folder

## API Automation Structure

For this automation, all test scenarios are under currency-conversions.cy.js

There are two scenarios under this spec, Conversion rate for currency - Success and Conversion rate for invalid currency - Fail

The first scenario will always run for a 10-week conversion rate, if you want more than 10 weeks you can change the variable numWeeks.

The first scenario also uses an array called currencies where it stores all the currencies the scenario will test. You can add as many currencies as you want on this array, just make sure the currencies are supported by the API.


