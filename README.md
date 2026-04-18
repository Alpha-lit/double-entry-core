# double-entry-core

A compact Django reference project for double-entry accounting primitives.

This repo exists to show serious backend engineering, not flashy demo work. It focuses on domain modeling, validation rules, and testable financial logic in a clean public package.

## Why this repo exists

A lot of strong private systems never become visible in public portfolios.

This project turns one high-signal concept, a double-entry ledger core, into a recruiter-friendly public repo that demonstrates real engineering judgment without exposing private business code.

## What it demonstrates

- double-entry accounting fundamentals
- balanced journal entry validation
- immutable posting workflow
- clean domain boundaries
- service-layer business logic
- test-first financial correctness mindset
- Django structure for business-critical backend systems

## Initial scope

Version 1 stays intentionally tight.

### Core models
- Account
- JournalEntry
- JournalLine

### Core rules
- total debits must equal total credits
- journal entries cannot post without lines
- posted entries become immutable
- account categories drive normal balance behavior
- line amounts must be positive

### Core features
- create draft journal entry
- add debit and credit lines
- validate balance
- post entry
- calculate account balance
- list ledger lines for an account

## What this repo is not

- not a full ERP
- not invoicing software
- not payroll
- not bank integration
- not a clone of any private production codebase

## Suggested stack

- Python 3.12+
- Django 5
- Django REST Framework
- pytest
- PostgreSQL or SQLite for demo use

## Suggested structure

```text
app/
  accounting/
    domain/
    services/
    selectors/
    api/
    tests/
```

## Public portfolio positioning

This repo should communicate one thing clearly:

> I know how to model financial rules and backend business logic in Django.

That is stronger than publishing a half-finished public ERP.

## Roadmap

### v1
- domain model
- posting rules
- balance logic
- test suite
- clean README

### v2
- trial balance endpoint
- account statement endpoint
- reversal entries
- fiscal period guardrails

### v3
- multi-tenant adaptation example
- audit and event hooks
- demo fixtures

## Recruiter outcome

Someone landing here should quickly conclude:
- this developer has built real systems
- this developer understands financial correctness
- this developer can structure backend code cleanly
- this developer can separate domain logic from framework glue

## Next build step

Scaffold the Django project and implement the minimal accounting core with tests before adding extra features.
