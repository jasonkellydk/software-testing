# White Box - Structure based

## Syntax errors, semantic errors, and logic errors

A program in Java, or C# or any other language, may contain several kinds of errors:

* **syntax errors**
* **semantic errors**
* **logical errors**

**syntax errors** the program may be syntactically ill-formed (e.g. contain while x {}, where there are no parentheses around x), so that strictly speaking it is not a Java program at all;

**semantic errors** the program may be syntactically well-formed, but attempt to access non-existing local variables or non-existing fields of an object, or apply operators to the wrong type of arguments (as in true * 2, which attempts to multiply a logical value by a number);

**logical errors** the program may be syntactically well-formed and type-correct, but compute the wrong answer anyway.

##	Quality assurance and different kinds of testing

Testing fits into the more general context of software quality assurance.
But what is software quality?

**ISO Standard 25010** distinguishes six quality characteristics of software:

* identifying software and system requirements;
* validating the comprehensiveness of a requirements definition;
* identifying software and system design objectives;
* identifying software and system testing objectives;
* identifying quality control criteria as part of quality assurance;
* identifying acceptance criteria for a software product and/or software-intensive computer system;
* establishing measures of quality characteristics in support of these activities.

## Debugging versus functionality testing

The purpose of testing is very different from that of debugging. It is tempting to confuse the two, especially if one mistakenly believes that the purpose of debugging is to remove the last bug from the program. In reality, debugging rarely achieves this.
The real purpose of debugging is diagnosis.

## Profiling versus performance testing

The distinction between functionality testing and debugging has a parallel in the distinction between performance testing and profiling.

**The purpose of profiling is diagnosis.** After we have observed that the program is too slow or uses too much memory, we use profiling to answer the question: why is this program so slow

**The purpose of performance is efficiency strengthening** so testing our belief that the pro- gram is efficient enough.

## White-box testing versus black-box testing

White-box testing and black-box testing are complementary approaches

### White-box testing (structural testing or internal testing)
* focuses on the text of the program
* The tester constructs a test suite
* Tests program’s choice and loop constructs — if, while, switch, try-catch-finally

### Black-box testing (sometimes called external testing)
* focuses on the problem that the pro- gram is supposed to solve
* the problem statement or specification for the program.
* The tester constructs a test data set (inputs and corresponding expected outputs)

