
## Static Testing
- Tests done on **work products** that does ***not*** involve running software
- Typically done early in testing
- Benefits
  - Detect bugs before more difficult and time consuming dynamic testing
  - Find bugs not found in dynamic testing
    - Misunderstood user stories
  - Promotes good code quality
  - Early reviews promote team cohesion
- Examples of products that can be statically tested
  - User Stories
  - System Requirements Specifications
  - Web pages
  - User Manuals
  - Code
    - *Not running the code*
    - Static Code analysis
  - Contracts and schedules
  - User diagrams
- Static testing reveals defects directly
  - Dynamic testing reveals defects that were dormant and activated while the code was running
- Common defects found via static testing
  - Requirement Defects
    - user story/ business rule is ambigous or contradictory
  - Design Defects/Coding Defects/ Coding Standards
    - Poor coding patterns
    - Unused variables
    - inconsistent naming conventions
    - cyclomatic complexity
  - Interface Specification Mismatch
    - The fields on a JSON might differ
    - The data type might be different
  - Gaps in Test coverage
    - Traceability matrix cannot be filled out

### Static Testing Review Workflow
1. **Planning**
   1. Scope and prupose of review
   2. entry and exit criteria
   3. Effort and time
2. **Initiate Review**
   1. Handing out the tasks to individuals
3. **Individual Review**
   1. Note defects, reccomendations and questions
4. **Communication and analysis**
   1. Discuss defects and assign ownership of defects
   2. Assign a status to a defect
      1. Reject
      2. Accept
      3. Accept with minor changes
      4. etc...
5. **Fixing and Reporting**
   1. Create defect reports
   2. Communciate defects to appropriate teams

## Roles
- Author
  - Creator of the work product
  - Typically fixes defects
- Manager(s)
  - Manage budget/ schedule and times
- Facilitator
  - Hosts and organizes meeting
- Review Leader
  - Decides who will do what reviews
- Reviewers
  - Do the review
  - Might be specialized based on knowledge
- Scribe
  - Responsible for keeping all documents
  - Making notes as necessary

## Review Techniques
- Ad Hoc
  - Just review the work products with no real organization or order
- Checklist-based
  - Reviewers are given a checklist of questions to review
  - Examples
    - Can the user reset their passowrd?
    - Can the managaer approve the request if his credentials are expired?
- Perspective-based
  - Reviewers model themselves after an end user
  - Attempt to use the product under review

#### Success Factors
- Clear objectives
- Reviews are written in small chunks
- People are open to criticism
- Criticism is constructive
- 
  

