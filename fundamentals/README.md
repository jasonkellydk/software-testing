
## Fundamentals
- Exhaustive testing of complex systems is not possible
  - A test approach in which all possible data combinations are use.
- Do the right sort of testing instead of trying to test everything. 
- 50% developing and 50% testing	
- Resource Triangle
  - Time
  - Money
  - Quality			
- Deciding when enough is enough
  - Most important thing is prioritisation
  - Setting criteria to when it is safe to stop testing
  - No unlimited time
  - Resources: materials, humans = salaries, overhead, budget
  - Deadlines
- Testing and Debugging
  - Debugging is the process of developers fixing bugs and defects.
  - Testing does not include correcting of bugs or defects. That is passed on to the developer. Testing ensure that changes are checked for their effect on other parts of the component or system.
- Static testing and dynamic testing
  - Static testing is the term used for testing where the code is not exercised. Usually using tools to examine the code while the developer is typing it. Failures often begin with human error and it is therefore important to start testing as early as possible before the issues become failures.
  - Dynamic testing is using the program under test with test data.

# Early Testing
  - Work-products are created throughout the software development life cycle (SDLC). As soon as these are ready, we can test them. As soon as these are ready, we can test them.
  - Cost escalation model
  - The earlier a problem (defect) is found, the less it costs to fix.
  - Many problems in software systems can be traced back to missing or incorrect require- ments.
  - Requirement documents are the basis for acceptance tests. Testing can begin as soon as those are available.
  - Many problems in software systems can be traced back to missing or incorrect requirements.

## Test coverage

A standard measure of a test suite’s comprehensiveness is coverage

some examples:

* **method coverage**
* **branch coverage**
* **path coverage**

**method coverage:** does the test suite make sure that every method (including function, procedure, constructor, property, indexer, action listener) gets executed at least once? statement coverage: does the test suite make sure that every statement of every method gets executed at least once?

**branch coverage:** does the test suite make sure that every transfer of control gets exe- cuted at least once?

**path coverage:** does the test suite make sure that every execution path through the program gets executed at least once?
