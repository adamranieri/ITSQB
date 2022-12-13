
#### Tester Independence
- Testing and development teams can operate together or be independent
- Often the level of independece depends on the organizaion or project
- Low Independence
  - Developers write their own tests
  - Testers are part of the dev team and might write code
    - pros
      - Testers can give quick feedback
      - Testers do not feel like an outside *adversary*
      - Testers get greater experence with the test object
- High Independence
  - Testers are a seperate team to development
  - Testers might be a 3rd party to the deveolopment team
    - pros
      - Less political pressure to have good results
      - Eliminate possible coginize bias that comes from familiarity with the project

#### Tester Roles
- **Test Manager**
  - Creates Test Policy, Test Strategy and Test Plan
  - Coordiante between Testing and other teams
  - Create test progress and test summary reports
  - Set up a defect management system
  - Select the tools to be used in testing
  - Develop the skills of the testing team
- **Tester**
  - Analyze and review user stories, business requirements and acceptance criteria
  - Design and implement test cases
  - Create traceability between the test cases, requirements and test basis
  - Execute Tests
  - Evalute Non-functional characteristics

## Test Plan
- The Test Plan is a living document
  - it is *supposed* to be created and alterted as the project and tested evolves
- There might be a master test plan
  - There could be a test plan for each level
- Things included in a test plan
  - Test Objectives
  - *Approach of testing*/ *Test Strategy* 
  - How to integrate testing into the software development lifecycle
  - What to test 
  - How to test
  - Who is doing the test
  - Testing schedule
  - Metrics for monitoring test progress
  - Providing templates to be used for reporting, constructing tests, reporting tests etc...
## Test Strategy ##
A generalized style of testing. The test strategy for any testing is an amalgam of styles suited for the the particualr testing.
- Analytical
  - Some factor like requirements or risk is used to approach tests
      - Risk-based testing.
        - Tests are created with the task of testing the biggest risks in an application
- Model-Based
  - Tests are designed based on some model or aspect of the application.
      - For example tests are organized by feature in the application or by software package
- Methodical
  - Running down a checklist of common failures in an application
      - Could also include important features like "every page is handicap accesible"
- Process Compliant
  - Creating tests that show the application is compliant with rules from another agency.
      - The system meets all requirements for HIPAA as an example
- Directed/consultative
  - Tests are guided by a stakeholder or client
- Regression-averse
  - Try to avoid regression testing as much as possible
      - Make heavy use of automated testing and previous testware
- Reactive
  - The tests are not planned beforehand and are designed and executed on the spot

**Test Approach** is the a test strategy applied to a specific project. For instance setting up weekly stakeholder meetings to see what to test next is an implementation of a Directed stratgey.

### Entry/Exit Criteria
- As part of a test plan the level of testing and type of testing to be done should be clarified.
- For each level and type of testing you should include
  - **Entry Criteria**
    - What needs to be completed for the testing to begin
    - Examples
      - Documenation like user stories or SRS are completed
      - Test environment has been set up
      - Test data has been created
  - **Exit Criteria**
    - What needs to finished and reported for the testing to be considered thoroughly done.
    - Examples
      - All tests have been exeucted and reported in the proper places
      - There are no remaining defects
      - A metric like 90% of code has been covered is achieved

## Test Effort 
How difficult somthing is to test
- Increases Difficulty
  - Complex domain
    - Accounting software will be harder to test than a pizza delivery app.
    - More likely a user story is misinterpreted
  - Poor test basis
    - Old documents and user stories
    - Unable to access the codebase
  - Size
    - The large the application the difficulty increases
  - Level of Detail in test reporting
  - Legal or regulatory compliance
- Decreases Difficulty
  - Well established long running applications
  - Good testware and test reporting tools
  - Skilled testers
  - Minimal defects discovered

## Test Monitoring and control
- Test Monitoring
  - How the status of tests activities are tracked
  - **Test Metrics** 
    - Examples
      - % of test cases created
      - the amount of test cases exeucted, passed and failed
      - % of requirements covered
      - 
- Test Control
  - How the test schedule is changed in response to events
    - Someone is sick
    - Test Environment is down

- **Test Report**
  - A document describing how testing is going for a test activity
  - Test Activity could be all unit tests for instance
  - Should include 
    - test metrics
    - Any blockers in testing
    - Progress made related to test plan
     - Summary of tests peformed
    - Comments about the quality of the test object
    - Any deviations from the test plan
  - Should be written with an audience in mind
    - Stakeholder
    - Development team
    - Test Manager
- *Test Progress Report*
  - Report made during testingtesting activity
- *Test Summary Report*
  - Report made at end of testing activity

- **Test Configuration**
  - The logistics of traking all test items
    - Each test case is uniqued ID or named
    - Every document is follows a certain naming convention
    - Any testware is in version control

## Risk
- The likelyhood of an event with negative consequences in the future
- Product risk
  - Feature or functionality is broken
  - Poor User Experience
  - A computation is incorrect
- Project Risk
  - Inaccurate budgeting 
  - Insufficient skills/training by team
  - Poor team communication
  - Test basis not well defined
  - Test environment/tools not ready
  - A 3rd party might not supply the software for integration on time

## Defect Management
- Defects should be tracked by test level
- Defects will be handled by all organziations and proejct differently
  - From very informal to very formal
- A defect report usually contains
  - A Unique ID
  - Title
  - Short summary
  - Date of disovery 
  - Who Discovered it
  - The Test Object it occured on
  - Steps to reproduce
  - Possing suggestions on how to fix it
  - Supporting evidence
    - Screenshots
    - Stacktraces
  - Priority
  - Severity
  - Expected Behavior vs Actual Behavior
  - State of defect
    - Open
    - Deferred
    - Closed
    - re-opended
    - Waiting to be fixed
    - etc...
  - It's connection to test cases
    - What Test cases it causes to fail
    - What Test case discovered it
- 