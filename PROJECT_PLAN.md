# double-entry-core Project Plan

## Goal
Create a compact public repository that turns private finance-system experience into visible backend engineering proof.

## Design principles
1. small enough to finish
2. domain-serious, not tutorial-like
3. high test coverage on core financial rules
4. clean naming and folder structure
5. safe abstraction from private codebases

## v1 deliverable
A working Django project with:
- account model
- journal entry model
- journal line model
- posting service
- balance calculation
- API endpoints or management demo flow
- tests covering balance and immutability rules

## Architecture shape
- models hold durable state
- services enforce posting rules
- selectors handle read/query logic
- API layer stays thin

## Naming guidance
Use neutral, reusable names.
Do not import private business vocabulary from Bulaal, Tusmo, or Nagaad.

## Suggested milestones
1. scaffold repo
2. define domain model
3. implement posting workflow
4. implement balance queries
5
 add tests
6. polish README with examples
7. publish publicly

## Avoid
- dashboards before core rules
- frontend distraction
- too many apps
- fake enterprise buzzwords
- overgrown scope
