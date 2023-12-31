### Software Testing Techniques

#### Overview of Software Testing
Software testing is a critical component of the software development lifecycle. It involves the evaluation of software to detect differences between given input and expected output. Testing is a process that involves the execution of a software component to evaluate one or more properties of interest.

#### Types of Software Testing
- **Component Testing**: 
  - Focuses on individual components within a program.
  - Ensures that each component functions correctly in isolation.
  - Typically the responsibility of the developer who created the component.
  - Example: Testing a login system by verifying username and password handling.

- **Integration Testing**: 
  - Involves testing groups of components as a combined entity.
  - Ensures that multiple components work together as intended.
  - Often conducted by an independent testing team.
  - Based on system specifications to reflect the requester's needs.

#### Defect Testing
- **Goal**: To discover defects within the program.
- **Key Principle**: Testing can show the presence of defects, not their absence.
- **Exhaustive Testing**: Testing every possible input is impractical, thus prioritization is necessary.
- **Prioritization Guidelines**:
  - Test system capabilities over individual components.
  - Focus on typical situations over boundary cases.

#### Test Data and Test Cases
- **Test Data**: Inputs designed to test program functionality.
- **Test Cases**: Combinations of inputs and expected outputs.
- **Test Plan Template**: Includes test case name, description, input data, expected output, and actual output.

#### Defect Testing Process
- Design test cases.
- Prepare test data.
- Run the program with test data.
- Compare results with expected outcomes.
- Generate a test report detailing successes and failures.

#### Black Box Testing
- Treats the system as a 'black box' without knowledge of internal workings.
- Focuses on testing against system specifications.
- Can begin early in the development process.

#### Equivalence Partitioning
- Divides input data and output results into classes that should behave equivalently.
- Test cases are selected from each partition to ensure coverage.

#### Boundary Value Analysis
- Focuses on values at the edge of equivalence partitions.
- Important for detecting errors in boundary conditions.

#### Search Routine Specification
- **Preconditions**: Conditions that must be true before the routine runs.
- **Postconditions**: Conditions that must be true after the routine completes successfully.

#### Input Partitions for Search Routine
- Inputs conforming to preconditions.
- Inputs where preconditions do not hold.
- Inputs where the key element is a member of the array.
- Inputs where the key element is not a member of the array.

#### Structural Testing (White Box Testing)
- Based on knowledge of the program's internal structure.
- Aims to execute all program statements.

#### Path Testing
- Ensures each possible path through the program is executed at least once.
- Utilizes program flow graphs to identify decision points.

#### Cyclomatic Complexity
- Measures the number of linearly independent paths through a program.
- Calculated as the number of edges minus the number of nodes, plus two.
- Indicates the minimum number of tests needed to execute all paths.

#### Key Points
- Test commonly executed parts of the system.
- Use equivalence partitions to create effective test cases.
- Black box testing is based on system specifications.
- White box testing focuses on internal program paths.
