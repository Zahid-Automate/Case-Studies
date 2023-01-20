# Case-Study on Test Automation 

As applications and systems grow larger and more complex, test automation is moving beyond a luxury and becoming a necessity for them. As technology changes, testing must also change and adapt. So start small, by using different approaches on a small scale to see what works best before attempting to spread further.

Successful test automation needs both ingenuity and perseverance.

What are the main factors that contribute to success in test automation? What common factors most often lead to the failure of an automation effort?

There are no simple universal answers to these questions, but some common elements exist. Two of them are management issues and the testware architecture:

- <b>Management support for automation,</b> such as setting realistic objectives and providing sufficient and appropriate resources to achieve a planned return on investment (ROI).

- <b>A good technical architecture for automated testware,</b> having the right levels of abstraction to give flexibility and adaptability while minimizing costs, not just of testware maintenance, but of all aspects of automation.
Overview


Added value / benefits
- <b>Performing a daily check of the test environments</b> (9 environments, in place for 1 year)

       - manually \~30 minutes/environment

       - automated \~15 minutes/environment
        
- With automated tests, we are <b>able to identify, within minutes, major configuration issues </b>(e.g. deployment problems, services not started).

- We sometimes <b>find bugs that are not found by manual test execution.</b>

- Manual testers have <b>more time for exploratory testing </b> since they don`t have to perform the tests that are already automated.

- <b>Functional</b> (test cases) coverage.

- <b>Number of releases/ year.</b>

- 2013(regression testing done manually) - 4 releases/year

- 2015(regression testing done automatically + manually) - 8 releases/year

<b>=> GAIN:</b> doubled the number of releases in a 2-year time span

## HOW - case ## 
### Introduction ###
- Automation testing is part of the development life cycle (with continuous delivery)

- Independent team, working with Scrum (testers & developers)

- Defined and documented way of working

- Support from Architect for the testing approach & senior developers for technical reviews

### Phases ###

- Pilot - goal: Define Strategy and Approach by trying to automate various parts of the systems

- Phase 1 - goal: Automate first subset of tests, which forms environment morning check [\~30 tests]

- Phase 2 - Goal: Extension of morning check [400+ tests]

- Phase 3 - Goal: Regression test suite

### CI runs ###
- All development environment + Integration + Acceptance

- Team City

- Schedule

### Frontend tests ###
- Are done by clicking links and comparing elements

- All tests are independent

- Can be executed for each browser

- Tests are written based on A-A-A (arrange-act-assert) pattern

- Usually, it's a check if an element exists or if an element contains a certain value.

- Screenshots are made if tests fail

### Backend tests ###
- Tests are written based on A-A-A (arrange-act-assert) pattern

- All tests are independent

- Ping tests check if a call can be made

- Quick scan tests simulate a user using application by calling all calls without frontend
