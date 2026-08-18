---
name: rp-test-plan
description: "Create a simple Republic Polytechnic software-testing test plan from a school template or slide reference. Use for plans such as EcoQuest - User Authentication Test Plan, especially when a plan ID such as ECO-UA-TP-01, scope, objectives, test approach, schedule, environment, entry and exit criteria, risks, and deliverables are required."
argument-hint: "Provide the system or feature, test-plan ID, and template or requirements"
---

# RP Test Plan

Create a clear, school-assignment-ready test plan from the user's template, slides, and requirements. Fill in known details and label unknown details as assumptions or pending confirmation. Do not invent URLs, dates, names, credentials, or unsupported behavior.

## Current Example

- Title: `EcoQuest - User Authentication Test Plan`
- Test Plan ID: `ECO-UA-TP-01`
- Feature: User Authentication / Login

The test-plan ID is not a test-case ID. Manual test cases derive IDs from the project prefix, for example `ECO-UA-FUNC-001`.

## Required Structure

Use these sections in order unless the user's template specifies another order:

1. **Document Control** - title, Test Plan ID, version, date, author, status.
2. **Introduction / Purpose** - system or feature and reason for testing.
3. **Test Objectives** - specific outcomes testing must demonstrate.
4. **Scope** - in-scope and out-of-scope items.
5. **Test Items and Features** - functions covered.
6. **Test Approach / Test Types** - functional, valid, invalid, validation, UI, security, and accessibility when relevant.
7. **Test Data and Environment** - URL, browser/device assumptions, accounts, and other data.
8. **Test Schedule and Activities** - preparation, case design, manual execution, automation, retesting, and review.
9. **Roles and Responsibilities**.
10. **Entry Criteria**.
11. **Exit Criteria**.
12. **Risks, Assumptions, and Mitigations**.
13. **Approval / Sign-off**.

## Procedure

1. Read the template, slides, requirements, and project context if available.
2. Identify the system name, feature, Test Plan ID, scope, required test types, and required headings.
3. Build document control using the exact supplied plan ID, such as `ECO-UA-TP-01`.
4. Define observable objectives, such as successful login, rejection of invalid credentials, empty-field validation, and protection of authentication data.
5. Separate in-scope and out-of-scope behavior. Mark assumptions clearly.
6. Describe each selected test type and what it checks.
7. Add a manual test-case summary only when requested. Use the companion `rp-login-test-case-summary` skill for its three-column format.
8. For automated testing, mention automation in the approach and schedule, but do not create a duplicate manual summary. Scenarios and assertions belong in code.
9. Add environment, data, schedule, responsibilities, entry/exit criteria, and risks.
10. Reserve time for defect investigation and retesting when capacity is known; do not schedule 100% of available time for planned work.

## School-Friendly Defaults

- Entry: requirements are available, the application is accessible, test data is prepared, and the tester can reach the feature.
- Exit: planned high-priority tests are executed, results are recorded, defects are logged, critical defects are closed or accepted, and results are reviewed.
- Status: Not Started, In Progress, Blocked, Complete.
- Risk: High, Medium, Low.

## Validation Checklist

- Title and Test Plan ID are present and consistent.
- Test-plan ID is distinguished from manual test-case IDs.
- All required sections are present.
- Scope includes explicit in-scope and out-of-scope items.
- Each listed test type has a clear purpose.
- No unsupported facts or unresolved placeholders remain where details were supplied.
- Risks include mitigations.
- Schedule includes retesting or unexpected-defect time when capacity is provided.
- Automated tests are not duplicated as manual summary tables.
