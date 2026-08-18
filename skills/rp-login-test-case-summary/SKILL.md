---
name: rp-login-test-case-summary
description: "Create simple Republic Polytechnic software-testing login test case summary tables using Test Case ID, Test Cases, and Type. Use for manual login test cases in school assignments, especially when a test-plan ID such as ECO-UA-TP-01 defines the project prefix. Unit and automated test cases belong in code unless the user explicitly requests a documentation summary."
argument-hint: "Describe the login feature or requirements to summarize"
---

# RP Login Test Case Summary

Create a simple manual login test-case summary suitable for a school report or slide.

## Output Format

Use exactly these columns:

| Test Case ID | Test Cases | Type |
|---|---|---|
| ECO-UA-TC-001 | Validate login succeeds with valid username and password | Valid |

## Procedure

1. Read the user's requirements, examples, or attached reference.
2. Create one row for each distinct login rule. Cover valid credentials, incorrect credentials, empty fields, and case sensitivity when relevant.
3. Derive sequential IDs from the test-plan prefix. For test plan `ECO-UA-TP-01`, use `ECO-UA-TC-001`, `ECO-UA-TC-002`, and so on. Use another suffix only when the user's reference specifies one.
4. Write concise, observable descriptions. Avoid `test login`, `verify it works`, `looks right`, or `everything works`.
5. Use one Type per row from the definitions below.
6. Return only the table unless the user requests an explanation or file.
7. If the source test cases are unit tests or automated script tests, generate a summary only when explicitly requested and state that it documents the code rather than replacing the executable tests.

## Type Definitions

| Type | Meaning | Example |
|---|---|---|
| Valid | Uses correct or acceptable input | Login with valid username and password |
| Invalid | Uses incorrect or unacceptable input | Login with incorrect password |
| Functional | Checks whether a feature works as required | Password masking works correctly |
| Validation | Checks required fields and input rules | Username cannot be left blank |
| UI | Checks visual or interface behaviour | Login button is displayed and clickable |
| Security | Checks authentication or security behaviour | Password is not shown as plain text |

Select the most specific applicable Type and do not combine multiple values unless the user's template allows it.

## Boundaries

- This skill creates manual summary tables only.
- Do not add Priority, Preconditions, Steps, Expected Result, or Test Data by default.
- Unit and automated test code does not need a duplicate summary table by default. Put scenarios, data, actions, and assertions in the code.
- When the user explicitly requests an automated-test summary, provide it as documentation and tell the user that the executable test case remains in code.
- For full manual cases, use the standard anatomy: Title, Preconditions, Steps, Expected Results, and Test Data.
- Do not invent unsupported features such as account lockout, password recovery, or email-format rules.

## Validation

- Header is exactly `Test Case ID | Test Cases | Type`.
- IDs are unique, sequential, and use the project prefix.
- Every description is non-empty and covers one business rule.
- Every Type is `Valid`, `Invalid`, `Functional`, `Validation`, `UI`, or `Security`.
- No vague expected wording is present.
