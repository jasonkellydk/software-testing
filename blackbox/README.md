# Blackbox - specification based
+ Focus on specifications
+ Technique derived from specs or some model(=test basis)
+ Important to separate definition of what it is (specs) from how it should work (design)
+ Allows the two specialist groups (testers and designers) to work independently

## Five techniques
- Equivalence partitioning
- Boundary value analysis
- Decision table testing
- State transition testing
- Use case testing

## Equivalence partitioning
    - Input partitions
    - Very simple idea: inputs can be put in groups of similar kind. Could be integers. Should reject anything else, like positive and negative integers and zero. 
    - Every value in the partition is exactly the same for the program
    - Reduces the number of test cases we need to write. Only needs one test from each partition. For example, partitions -10000 to -1 or 0 or 1 to 10000
    - Often select a value in the middle range 
        - -5000
        - 0
        - 5000
    - Valid equivalence partitions: collections of valid inputs
    - Non-valid equivalence partitions are important to test. For example, inputs less than -10000 and greater than 10000, real numbers like 3.17
    - Tip: Testing is trying to check that the system does everything it should do - nothing else.
    - Generally there are far more ways of incorrect input than correct.

    - Output partitions
        - You can make partitions for expected output. For example, 3%, 5% and 7% interest rate based on credit amount.
        - Can be alternative to input partitions
 <img src="assets/output-partitions.png"/>
  
    - Other partitions

<img src="assets/equivalence.png" width="500" height="300" />

## Boundary value analysis
<img src="assets/equivalence-boundary.png" width="500" height="300" />


## Decision table testing
<img src="assets/decision.png" width="1000"/>
<img src="assets/decision-table-2.png" />

## State transition testing
<img src="assets/state-transition.png" />

<img src="assets/state-transition-example.png" />

<img src="assets/state-transition-example-2.png" />

## Use case testing