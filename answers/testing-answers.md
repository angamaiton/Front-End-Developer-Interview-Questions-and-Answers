# Testing Questions

#### What are some advantages/disadvantages to testing your code?

###### Advantages

- Tests can be used as specs/requirements
- Testing provides an easy way to ensure that there are no missing pieces that
  aren't working when code is refactored
- Tests can be shared across a team

###### Disadvantages: there are rarely disadvantages

- It can take more time at the outset to prototype.
- If you have the wrong boss, he may yell at you or fire you if you keep telling
  him that testing is important.

#### What tools would you use to test your code's functionality?

Every language has their own set of tools, but here's a basic idea of what I use
for my tests:

  - **JavaScript**: Jest (React, front-end and back-end), Mocha (back-end), Nightmare (integration)
  - **Ruby**: RSpec (Rails)
  - **Elixir**: ExUnit (Phoenix, universal)
  - **CSS**: Quixote

#### What is the difference between a unit test and a functional/integration test?

Unit tests are, as the name would suggest, for individual (small) units of code. Integration
tests, on the other hand, test how well each unit/piece of code works together.

#### What is the purpose of a code style linting tool?

Linting helps keep source code in a repository consistent and easy for
developers to read and use (as well as pick up, if they're new to a project). It
also helps prevent mistakes and errors -- for a language like Python, which is
whitespace-sensitive, it can be the difference between a method passing and
failing unexpectedly. Linters serve as a kind of static analyzer, and can be
really helpful for keeping code clean and well-structured.
