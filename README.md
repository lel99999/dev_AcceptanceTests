# dev_AcceptanceTests
Development of Acceptance Tests w/Python

#### BDD Life-Cycle

![https://github.com/lel99999/dev_AcceptanceTests/blob/main/bdd-cycle.jpg](https://github.com/lel99999/dev_AcceptanceTests/blob/main/bdd-cycle.jpg)

The process can be defined as:
- Write a failing acceptance test
- Write a failing unit test
- Make the unit test pass
- Refactor
- Make the acceptance test pass

Rinse and repeat for every feature, as is necessary. <br/>

#### Gherkin Syntex
Acceptance tests usually make use of the Gherkin Syntax, introduced by the Cucumber Framework, written for Ruby. The syntax is quite easy to understand, and, in the Lettuce Python package, makes use of the following eight keywords to define your features and tests: <br/>

- Given
- When
- Then
- And
- Feature:
- Background:
- Scenario:
- Scenario Outline:

```
Here is a sample Gherkin document:

Feature: Account Holder withdraws cash
 
  Scenario: Account has sufficient funds
    Given the account balance is $100
      And the card is valid
      And the machine contains enough money
    When the Account Holder requests $20
    Then the ATM should dispense $20
      And the account balance should be $80
      And the card should be returned
```

#### BDD Frameworks
- robot [https://pypi.org/project/robotframework/](https://pypi.org/project/robotframework/)  is a generic open source automation framework for acceptance testing, acceptance test driven development (ATDD), and robotic process automation (RPA). It has simple plain text syntax and it can be extended easily with libraries implemented using Python or Java.
- pytest-bdd [https://pytest-bdd.readthedocs.io/en/latest/](https://pytest-bdd.readthedocs.io/en/latest/) is a plugin for pytest that lets users write tests as Gherkin feature files rather than test functions. Because it integrates with pytest, it can work with any other pytest plugins, such as pytest-html for pretty reports and pytest-xdist for parallel testing. It also uses pytest fixtures for dependency injection.
- radish [https://pypi.org/project/radish-bdd/](https://pypi.org/project/radish-bdd/) is a BDD framework with a twist: it adds new syntax to the Gherkin language. Language features like scenario loops, scenario preconditions, and constants make radish‘s Gherkin variant more programmatic for test cases.
