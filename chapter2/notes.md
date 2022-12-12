## Development and Testing Lifecycles
- Testing Lifecycle should pair up to development lifecycle

## Test Levels
  - Unit/component/module
  - Integration
  - System 
  - Acceptance
### Provided for each test level
- **Test Basis**
  - Used to dervive test cases
- **Objectives of testing**
- **Test Object**
  - Something to test
- **Techniques and tools applicable to that level**
## Sequential Models
- Linear flow of testing activities
- **Waterfall**
  - Testing occurs *after* development
- **V-Model**
  - Testing occurs with development in each stage
- Process takes months to years to produce results for stakeholders

## Iterative Models
- Working software is produced in every iteration
- **Agile**
  - *kanban*
  - *Scurm*

## Unit/component/module Testing
- ***Usual Objectives***
  - Create confidence in unit/module quality
  - Verify that functional and non-functional requirements are met
  - Find defects and prevent them from affecting higher levels of the program
- ***Test Basis***
  - Data models
    - UML diagrams
    - Schemas
  - Source Code
- ***Test Objects***
  - Source Code
    - Functions
    - Classes
    - Objects/data structures
  - Software packages
- ***Typical Defects***
  - Flow control failures
  - Improper logic
- **Approach**
  - Often performed by the developer
  - TDD
  - Testing framework
- **Test Environment**
  - Local computer with testing tools
- **Test Type Examples**
  - **Functional**
    - A Test that verifies that a function can convert kilometers to miles correctly
  - **Non Functional**
    - A Test that measures how much CPU usage is used for a large converion of kilometers to miles
  - **White Box**
    - Tests measure all branching logic of the code being covered
      - Every switch case is tested
      - Every if-else is executed in a test
  - **Change Related**
    - A Test framework executes tests each time a developer commits a code change

## Integration Testing
- ***Usual Objectives***
  - Create confidence in the **interfaces** of the application
    - The join point that other programs will interact with
  - Find defects and prevent them from escaping into higher levels
- ***Test Basis***
  - Software design diagram
  - Use Cases
  - Workflow diagrams
- ***Test Objects***
  - Databases
  - APIs
  - Interfaces
- ***Typical Defects***
  - Incorrect data input/output
    - Missing fields
    - encoded differently
  - Unhandled communication errors
  - Failed security 
- **Approach**
  - Focus on testing the connection. Not the component
  - **Component Integration Testing**
    - Seeing if two or mor module work together
      - Often performed by the developer
  - **System Integration Testing**
    - Seeing if two or more standalone systems work together
      - Start with the most critical used systems first
    - Strive for continuous integration
      - Doing an integration test of many components becomes very difficult
- **Test Environment**
  - Local computer with testing tools
  - Could involve multiple running applications and mock setups
- **Test Type Examples**
  - **Functional**
    - Data from a web form is able to be handled by the backend
  - **Non Functional**
    - URL parameter poulltion is checked to prevent a security break
  - **White Box**
    - JSONs from the frontend are correcly parsed into Java Objects
  - **Change Related**
    - Tests that the updated API endpoints do not break existing features

## System Testing
- ***Usual Objectives***
  - Verify that functional and non-functional requirements are met
  - Find defects and prevent them from affecting higher levels 
  - Create confidence in the system as a whole
- ***Test Basis***
  - User stories and epics
  - state diagrams
  - Risk Analysis reports
  - SRS functional and non-functional
- ***Test Objects***
  - Applications
  - Systems Under Test (SUT)
- ***Typical Defects***
  - Incorrect or unexpected functional behavior
  - System does not conform to specifications
  - Inability to complete all parts of end-to-end tasks 
- **Approach**
  - Done by testers
- **Test Environment**
  - Resembles the environment of the deployed application
- **Test Type Examples**
  - **Functional**
    - A user can create a new account
  - **Non Functional**
    - A test that confirms Every web page loads in less that 5 seconds
  - **White Box**
    - All navigation links go to the correct pages in a web app
  - **Change Related**
    - A change in anypart of the system causes selenium script to run all test cases fulfilling critical user stories

## Acceptance Testing
- ***Usual Objectives***
  - Verify that functional and non-functional requirements are met
  - Create confidence in the system as a whole
  - Verify application is in a state to be released to users
  - *not* concerned with finding defects
    - Finding many defects likely means the application has substantial foundational issues
  - **Types of Acceptance Testing**
    - User Acceptance Testing
      - The application handles all requirements needed by the end user
    - Operational Acceptance Testing
      - Internal administrative tasks can be handled sucessulffy
        - Data is appropriately backed up
        - Logs are generated correctly
        - Installing/uninstalling work correctly
      - Security vulnerabilty
      - Performance testing
    - Contractural and Regulatory Acceptance Testing
      - Ensuring the application meets legal/contract requirements
      - Often done in association with an authority witnessing the testing
        - An auditor from the SEC might verify financial records cannot be edited
    - Alpha Testing
      - Interal testing/developers test an application to see if it works as intended
    - Beta Testing
      - People outside the test/dev teams who are sample end users use the application
      - Spot any issues related to end user expectations
- ***Test Basis***
  - User stories and epics
  - Legal Requirements
  - System or user documentation
  - SRS functional and non-functional
- ***Test Objects***
  - System Under Test (SUT)
  - Application
- ***Typical Defects***
  - Business rules not implemented or interpreted correctly
  - Does not mean contract or regulatory requirements
  - Poor perfomance and non-functional failures
- **Approach**
  - Done by stakeholders, end users and testers
- **Test Environment**
  - Resembles the environment of the deployed application
- **Test Type Examples**
  - **Functional**
    - A new user can create an account
  - **Non Functional**
    - Testing Someone with disabilities is able to use the website 
  - **White Box**
    - All files created when saving a picture are tested to be correct
  - **Change Related**
    - The application is sent to beta testers after the values of some enemy's health is recalibrated


# Test Types

## Functional Testing
- The software works as intended
- Should be performed at all test levels
- Throroughness is mesaured through test coverage
  - elements tested/ total elements
  - 40/47 user stories
  - 6/6 functions
  - Should create a meaningful %

## Non-Functional Testing
- Perforamnce/efficieny, usability, security

## White Box
- Tests derived from 
  - Source code
  - Architecture
  - Data Flows

## Change Related Testing
- Tests conducted after the system being tested funciality has changed
  - Code udpated
  - Configuration updated
- **Confirmation Testing**
  - Tests conducted after a defect has been fixed to *confirm* it is fixed
  - Should include any previously failing tests
  - Can include additional tests
- **Regression Testing**
  - Tests conducted after a change to a system to detect *side effects*
    - A change in one feature broke a different feature/component

## Maintenence Testing
- Testing conducted after the application has been deployed
  - When Maintenence testing might start
    - New Feature released
    - Bug(s) detected and fixed
    - Migration
      - System is moved to a new hosting environment
      - Data is being exported/imported from the system
  - **Impact Analysis**
    - Estimating the changes on the system when a maintenence update on a system occurs
    - 