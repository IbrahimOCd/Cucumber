# Cucumber POM Framework

A test automation framework built using Cucumber with Page Object Model (POM) design pattern.

## Project Structure

```
CucumberPOM/
├── src/
│   └── main/
│       └── java/
│           ├── com.cucumber.features/
│           │   └── Application.feature
│           ├── com.cucumber.stepdefinitions/
│           │   ├── ContactsSteps.java
│           │   ├── HomePageSteps.java
│           │   └── LoginSteps.java
│           ├── com.cucumber.pom.base/
│           │   └── BaseTest.java
│           ├── com.cucumber.pom.config/
│           │   └── config.properties
│           ├── com.cucumber.pom.pages/
│           │   ├── ContactsPage.java
│           │   ├── HomePage.java
│           │   └── LoginPage.java
│           ├── com.cucumber.pom.runner/
│           │   └── TestRunner.java
│           └── com.cucumber.pom.utils/
│               └── Constants.java
├── resources/
│   └── chromedriver.exe
├── test-output/
├── target/
├── pom.xml
└── README.md
```

## Technologies Used

- Java
- Selenium WebDriver
- Cucumber
- TestNG/JUnit
- Maven

## Key Features

- Page Object Model (POM) design pattern
- BDD framework using Cucumber
- Config file for test settings
- Base test class for common functionalities
- Separate pages package for web elements and actions
- Utility class for constants and common methods
- Chrome WebDriver included

## Prerequisites

- Java JDK 8 or higher
- Maven
- IDE (Eclipse/IntelliJ)
- Chrome browser

## Setup Instructions

1. Clone the repository
2. Import as Maven project in your IDE
3. Update config.properties file if needed
4. Update Chrome driver version if required

## Running Tests

To run the tests:
1. Through TestRunner.java
   - Right-click on TestRunner.java
   - Run as JUnit Test

2. Through Maven
   ```bash
   mvn clean test
   ```

## Configuration

Check `config.properties` file in `com.cucumber.pom.config` package for:
- Browser configurations
- URL configurations
- Other test settings

## Reports

Test reports can be found in:
- test-output folder
- target folder (Cucumber reports)

## Best Practices

1. Follow Page Object Model
2. Use Base class for common methods
3. Maintain test data in feature files
4. Keep step definitions clean and simple
5. Use constants from Constants.java

## Notes

- Make sure to have the correct version of chromedriver.exe matching your Chrome browser version
- Update pom.xml dependencies if needed
