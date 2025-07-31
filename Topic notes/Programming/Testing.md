# Testing

Testing is most commonly used in quality assurance, a fancy way of ‘making sure stuff works’

# Testing ***to find issues***

# Concept testing / MR

Also known as **market research**

- Used to understand the strengths and weaknesses of a concept
- For software, networks & digital system
- Only interested stakeholders are provided with information on the concept
- Stakeholders provide feedback, which is collated & analysed
- Very expensive and time consuming, but saves lots of unnecessary costs in the long term

# Unit testing / WBT

Also known as **white box testing**

- Individual components/units are tested
- Only used for software development (mainly)
- Designed to validate that all modules functions as intended
- Isolated sections of code are tested & verified
    - Sections can be functions, modules, procedures or objects

**Mixed integration**

Also known as sandwiched integration testing

- Top level units are tested, then bottom level units
- They are then tested once integrated
- Effective testing method for **large companies**

# Performance testing

Also known as perf testing

- Used to test the speed, response time, reliability, scalability and resource use
- Designed to ensure issues with performance are found & solved

# System testing

Falls under **black box testing** (People testing don’t have knowledge of the software design)

- Complete system testing with all software fully integrated
- Final test carried out to verify the system meets the specification
- Must meet both functional and non-functional requirements

Types of system testing:

## Usability/Acceptance testing

- Confirms if the end user will have a good experience
- Must meet the requirements of stakeholder(s)
- Evaluates the compliance of the system with the requirements of the business
- Ensures end user criteria have been met

## Load/Stress testing

- Form of **non-functional** testing
- Provides information on how the software/digital system works under various loads
- Similar to performance testing

## Regression testing

- Confirms if any changes to the software/digital system had any adverse effects on existing features

## Functionality testing

- Confirms that the software/digital system functions according to **user specifications**

## Migration testing

- Program/system testing to test the feasibility of moving it to a new digital system
- Checks that data and other dependencies can still be accessed, or if there needs to be a conversion

## 6Compatibility testing

- Checking that software will work on different platforms and environments

## Boundary testing

Form of **black box testing** (also used by developers in **white box testing**)

- Consists of a series of tests using **boundary values**
- Tests aspects of a program with the relevant **boundary values**

## Fuzz testing

- Uses invalid, random and unexpected data as inputs to software to see what the program does

# Automated and functional testing

## Automated testing

- Specialised tools used to control the execution of tests
- Actual results compared with expected results
- An example is **regression testing** which involves repetitive actions, and can be automated
- Where functional and non-functional tests are re-run to ensure that any newly developed code hasn’t added in any more bugs to already working areas of the program
- Testing tools are used to perform regression tests & automated data setup, generation, GUI interaction, defect logging and product installation
- Automation tools are used for functional and non-functional testing

## Functional testing

- Used to confirm functionality of a software system against **functional** requirements (specification)
- Each function of the software is tested by providing an input, then comparing the output against the functional requirements
- Primarily **black box testing** doesn’t deal with application source code
- Checks the UI, Application Programming Interfaces (API), database, security, client server communication etc.
- Can be carried out manually or with automation

There are some things to be considered when selecting a testing tool

- Compatibility with OS’s - Automation tools should support many OS’s
- Versatility - It’s important that whatever tool is used needs to support the testing that is going to be done (Duh)
- Compatibility with various platforms - The testing tool tool must support the range of applications that will be used by the end user, and any possible platform changes
- Test creation - A tool should provide more than one way to complete a task, allowing for quick & efficient test completion, regardless of the skill of the testers
- Maintenance - It can be simplified if the testing tool can generate modular test cases (breaking down large tests into smaller tests)
- Cost - Value for money. Aka, is it worth the money to have the tool? Y/N