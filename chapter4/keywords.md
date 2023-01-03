# Chapter 4

- black-box test
  - also called "behavioral testing", are based on analysis of the appropriate test basis (formal req. documents, spec sheets, user stories, etc.) Can be applied to functional and non-functional tests, and focuses on the inputs and outputs of a test rather than internal structure.

- technique,
  - The specific method applied to evaluate a system or component (ex. black-box, unit, integration, etc.)

- boundary value analysis,
  - testing values at the boundaries of an equivalence partition. E.g. in a partition that can be descried as having a valid range of 1-10 inclusive, the boundary values would be 1 and 10 for the valid partition, and 0 and 11 for the invalid partition.

- checklist-based testing,
  - testers deign, implement, and execute tests to cover test conditions found in a pre-determined checklist, usually created during analysis.

- coverage,
  - how much of the test object is actually being tested. Typically described as a percentage.  

- decision coverage,
  - how many possible decisions within a system are covered by tests. the standard is to have at least one test case for every possible combination of decisions.

- decision table testing,
  - tester identifies conditions (based on inputs) and resulting actions (outputs) of a system, often based on business rules. A table is created to map all possible decisions the system could arrive at.

- error guessing,
  - an experience based technique that aims to anticipate errors, defects and failures based on the tester's prior knowledge.

- equivalence partitioning,
  - dividing data into separate units or partitions known as "equivalence cases" in a way that all members of a given partition are expected to be processed in the same way. Can be divided into sub-partitions.

- experience-based test technique,
  - techniques that leverage the experience of developers, testers, and users to design/implement/execute tests. Can be used with black and white box techniques.

- exploratory testing,
  - using informal tests that are created on the fly during testing. used to create formal tests for areas identified as needing more testing.

- state transition testing,
  - testing done to test how the test object performs as events change it's internal state.

- statement coverage,
  - how many code statements within the test object are covered by tests. measured as the number of tested statements divided by the total number of executable statements; expressed as a percentage.

- test technique,
  - different ways of designing and implementing tests for different areas of a test object.

- use case testing,
  - tests derived from specific ways that users interact with the software.

- white-box test technique
  - also called "structural testing", based on analysis of internal structure or code of the test object. Focuses on the processing and structure within the test object rather than behavior (inputs and outputs.)
