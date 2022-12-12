# Test Case
- Test case is high level
- Test cases are often *NOT* executable by itself
- Test data will allow for several concrete low level test cases to be designed
- Inputs and expected results

```mermaid

    flowchart LR;
    TB[Test Basis]
    HTC[High Level Test Cases]
    TDATA["Test Data"]
    LTC[Low Level Test Cases]

    TB --> HTC
    HTC --- TDATA --> LTC

```