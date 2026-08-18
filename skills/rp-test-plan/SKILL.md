---
name: rp-test-plan
description: "Guide a student in creating a simple Republic Polytechnic software-testing test plan using the user's school template or solution reference as a guide. Use for plans such as EcoQuest - User Authentication Test Plan, especially when a plan ID such as ECO-UA-TP-01, executive summary, scope, test phases, environment setup, schedule, entry and exit criteria, test case summary, and change log are required."
argument-hint: "Provide the system or feature, test-plan ID, and template or requirements"
---

# RP Test Plan

Guide the user through a clear, school-assignment-ready test plan using the user's template or solution reference as a model. Learn the reference's headings, order, labels, table style, level of detail, and testing decisions, then apply those conventions to the user's own system and requirements. The reference is guidance, not content to copy: replace its project-specific details with supported details from the user's project. Fill in known details and label unknown details as assumptions or pending confirmation. Do not invent URLs, dates, names, credentials, or unsupported behavior.

## Use the Reference as a Guide

- Treat an attached template, completed solution, or slide as the guide for expected school format and depth.
- Extract the reference's structure and explain how each section applies to the user's system before drafting when the request is ambiguous.
- Reuse its section names and order when they are supplied, but do not copy project-specific names, IDs, dates, URLs, accounts, requirements, or test results.
- Use the reference's testing choices as prompts. Include a test type only when it is relevant to the user's feature or explicitly required.
- Keep the plan simple and readable for a school assignment. Use short paragraphs, bullets, and tables only where the reference uses them or where they make the information easier to scan.
- Preserve the reference's distinction between the test-plan document and individual test cases.
- If no reference is supplied, use the output structure below and mark missing project details as assumptions or pending confirmation.

When guiding the user, point out missing decisions such as the feature boundary, test data, environment, responsibilities, schedule, entry criteria, exit criteria, and risk mitigations. Ask for confirmation when a missing detail changes the plan; otherwise use a clearly labelled assumption.

## Current Example

- Title: `EcoQuest - User Authentication Test Plan`
- Test Plan ID: `ECO-UA-TP-01`
- Feature: User Authentication / Login

The test-plan ID is not a test-case ID. Manual test cases derive IDs from the project prefix, for example `ECO-UA-TC-001`.

## Output Structure

Use these sections in this order only when the user's template does not specify another order:

1. **Test Plan Header** - title, Test Plan ID, and version.
2. **Executive Summary** - product name, product description, and test objective.
3. **Scope** - what the test covers and what is excluded.
4. **Test Phases** - Test Implementation, Test Execution, and Test Completion, adapted to the project.
5. **Environment Setup** - browser, application URL, test accounts/data, and evidence or recording method.
6. **Schedule** - day, period, and topics/activities.
7. **Entry and Exit Criteria** - conditions for starting and completing testing.
8. **Test Case Summary Table** - manual cases with Test Case ID, Test Cases, and Type when requested.
9. **Test Change Log** - date, change description, author, and version.

### Scope Guidance

Always include Scope. Separate it into:

- **In scope:** features, rules, and user flows that will be tested.
- **Out of scope:** features, integrations, roles, platforms, or non-functional areas not covered by this plan.

For the EcoQuest login example, in-scope items may include valid login, invalid credentials, empty required fields, case sensitivity, password masking, and user feedback. Out-of-scope items may include registration, password recovery, dashboard functions, account administration, and performance testing unless the requirements explicitly include them. Adapt these examples to the user's actual system; do not assume they apply.

For the opening document-control area, use fields such as:

| Field | Value |
|---|---|
| Test Plan Title | `[system or feature] Test Plan` |
| Test Plan ID | `[supplied ID]` |
| Version | `1.0` or the supplied version |
| Date | supplied date, or `Pending confirmation` |
| Author | supplied author, or `Pending confirmation` |

## Procedure

1. Read the template, completed solution, slides, requirements, and project context if available.
2. Extract the reference's expected structure, level of detail, and testing decisions as guidance.
3. Map the user's system, feature, Test Plan ID, scope, requirements, and test types to that guidance.
4. Confirm or clearly label missing decisions before drafting.
5. Build the header using the exact supplied plan ID and version, such as `ECO-UA-TP-01` and `1.0.0`.
6. Write an Executive Summary with product name, product description, and observable test objective.
7. Define explicit in-scope and out-of-scope items before listing test phases.
8. Describe Test Implementation, Test Execution, and Test Completion activities, adapting the phase names only when the reference requires it.
9. Add the environment setup and schedule tables in the reference's style.
10. Add entry and exit criteria that are observable and specific to the feature.
11. Add a manual test-case summary only when requested. Use the companion `rp-login-test-case-summary` skill for its three-column format.
12. For unit tests or automated tests executed by a script, treat the test case as code: scenarios, test data, actions, and assertions belong in the test script, so do not create a duplicate summary by default.
13. If the user explicitly asks for a summary of unit or automated test cases, generate it, but state that it is a documentation summary only and that the executable test case remains in code.
14. Finish with a Test Change Log using supplied date, author, version, and change description, or label missing values as pending confirmation.

## School-Friendly Defaults

- Entry: requirements are available, the application is accessible, test data is prepared, and the tester can reach the feature.
- Exit: planned high-priority tests are executed, results are recorded, defects are logged, critical defects are closed or accepted, and results are reviewed.
- Status: Not Started, In Progress, Blocked, Complete.
- Risk: High, Medium, Low.

## Validation Checklist

- Title and Test Plan ID are present and consistent.
- Test-plan ID is distinguished from manual test-case IDs.
- All required sections are present.
- Scope is present and explicitly separates in-scope and out-of-scope items.
- Executive Summary includes product name, product description, and test objective.
- Test Phases cover implementation, execution, and completion when the reference uses those phases.
- Environment Setup includes browser, application, test data/accounts, and evidence recording where relevant.
- Schedule includes day, period, and activity where the reference uses that table.
- Test Change Log includes date, change description, author, and version where required.
- Each listed test type has a clear purpose.
- No unsupported facts or unresolved placeholders remain where details were supplied.
- Risks include mitigations.
- Schedule includes retesting or unexpected-defect time when capacity is provided.
- Unit and automated test cases are written in code and are not duplicated as summary tables by default.
- If an automated-test summary was explicitly requested, it is labelled as documentation only and the user is told that the executable test remains in code.
- The plan uses the supplied reference's headings, order, labels, and level of detail without copying unsupported project-specific content.
- Each included section and test type is connected to the user's system or requirements.
