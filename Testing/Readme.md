# Introduction to software testing

## Test Selection

- Manual testing
- Exception testing
- Boundary testing
- Randomized testing
- Coverage testing
- Requirements testing
- Specification testing
- Safety testing
- Security testing
- Preformance testing

Programmers usually make mistakes at:\
- Boundary conditions
- Complex Boolean Expressions

Thinking like "How can I break this thing"

- Black box testing: examine the requirements
- Write box testing: examine the code

Test cases: test data, expected output

4 parts of a test:

- Set up
- Invocation: execute the software under test
- Assessment: Observing the doftware's behaviour under test, documenting the actions that were taken
- Teardown: such as closing database connections, closing open file handles

For critial systems, much effort is in planning for failure

- Faults: programmer's mistake
- Latent errors: a line of code with a bug in it
- Effective errors: executing the line of code containing a bug, if the system reaches a state where the error can manifest
- Failures: e.g. the program crashes

## Where error usually happens

- Floating-point numbers
- Pointers(C/C++)
- Parallelism: such as deadlock
- Numeric Limits/Boundaries: off by 1
- Interrupts
- Complex Boolean Expressions
- Casts and Conversions between Types


## V model
User requirements ------------------> Validation
  Specification ------------------> Verification
    Architectural decisions ---> System integration testing
      Design -------------> Module testing
        Implementation -> Unit tests
        
Validation:\
- Meet user's satisfaction
- Are we building the right product?

Verification:\
- Are we building the product right?

## Mutation testing
create a new version of the software with a single error injected, and see if all the tests pass.
