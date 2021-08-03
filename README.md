# dev_AcceptanceTests
Development of Acceptance Tests w/Python

#### Gherkin
Keywords: <br/>
- Feature
- Scenario
- Given, When, Then, And, But (Steps)
- Background
- Scenario Outline
- Examples


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
- pytest-bdd is a plugin for pytest that lets users write tests as Gherkin feature files rather than test functions. Because it integrates with pytest, it can work with any other pytest plugins, such as pytest-html for pretty reports and pytest-xdist for parallel testing. It also uses pytest fixtures for dependency injection.
- radish is a BDD framework with a twist: it adds new syntax to the Gherkin language. Language features like scenario loops, scenario preconditions, and constants make radish‘s Gherkin variant more programmatic for test cases.
