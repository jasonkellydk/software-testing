# Blackbox - specification based
+ Focus on specifications
+ Technique derived from specs or some model(=test basis)
+ Important to separate definition of what it is **(specs)** from how it should work **(design)**
+ Allows the two specialist groups **(testers and designers)** to work independently

## The Five techniques
- <a href="/#/blackbox/README?id=equivalence-partitioning">Equivalence partitioning</a>
- <a href="/#/blackbox/README?id=boundary-value-analysis">Boundary value analysis</a>
- <a href="/#/blackbox/README?id=decision-table-testing">Decision table testing</a>
- <a href="/#/blackbox/README?id=state-transition-testing">State transition testing</a>
- <a href="/#/blackbox/README?id=use-case-testing">Use case testing</a>

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

<img src="assets/equivalence.png" width="500" />

## Boundary value analysis
Boundary value analysis is a software testing technique in which tests are designed to include representatives of boundary values in a range

<img src="assets/boundary-value-analysis.png" width="500" />

***as seen in this example the boundary value tests accepted the range of values***

## Decision table testing
Decision tables are a concise visual representation for specifying which actions to perform depending on given conditions.

<img src="assets/decision.png" width="1000"/>

***example of decision table***


</br>
</br>

<img src="assets/decision-table-2.png" />

***another example of decision table***

## State transition testing
State Transition testing, a black box testing technique, in which outputs are triggered by changes to the input conditions or changes to 'state' of the system. In other words, tests are designed to execute valid and invalid state transitions.

### When to use?
* When we have sequence of events that occur and associated conditions that apply to those events
* When the proper handling of a particular event depends on the events and conditions that have occurred in the past
* It is used for real time systems with various states and transitions involved

### Deriving Test cases
* Understand the various state and transition and mark each valid and invalid state
* Defining a sequence of an event that leads to an allowed test ending state
* Each one of those visited state and traversed transition should be noted down
* Steps 2 and 3 should be repeated until all states have been visited and all transitions traversed
* For test cases to have a good coverage, actual input values and the actual output values have to be generated

### Advantages
* Allows testers to familiarise with the software design and enables them to design tests effectively.
* It also enables testers to cover the unplanned or invalid states.

### Examples
A System's transition is represented as shown in the below diagram:

<img src="assets/state_transition_1.jpg" />

***table representation below***

|Tests|Test 1|Test 2|Test 3|
|--- |--- |--- |--- |
|Start State|Off|On|On|
|Input|Switch ON|Switch Off|Switch off|
|Output|Light ON|Light Off|Fault|
|Finish State|ON|OFF|On|


#### Other examples

<img src="assets/state-transition.png" />

<img src="assets/state-transition-example.png" />

<img src="assets/state-transition-example-2.png" />


## Use case testing