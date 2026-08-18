---
name: rp-test-plan
description: "Guide a student in creating a simple Republic Polytechnic software-testing test plan using the user's school template or solution reference as a guide. Use for plans such as EcoQuest - User Authentication Test Plan, especially when a plan ID such as ECO-UA-TP-01, executive summary, test phases, environment setup, schedule, entry and exit criteria, test case summary, and change log are required."
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
3. **Test Phases** - Test Implementation, Test Execution, and Test Completion, adapted to the project.
4. **Environment Setup** - the hardware, software, platform, tool, test data, and setup details needed for the specific project.
5. **Schedule** - day, period, and topics/activities.
6. **Entry and Exit Criteria** - conditions for starting and completing testing.
7. **Test Case Summary Table** - manual cases with Test Case ID, Test Cases, and Type when requested.
8. **Test Change Log** - date, change description, author, and version.

For the opening document-control area, use fields such as:

| Field | Value |
|---|---|
| Test Plan Title | `[system or feature] Test Plan` |
| Test Plan ID | `[supplied ID]` |
| Version | `1.0.0` or the supplied version |
| Date | supplied date, or `Pending confirmation` |
| Author | supplied author, or `Pending confirmation` |

## Procedure

1. Gather the user's available requirements, system or feature details, project context, template, and any reference material before drafting.
2. Extract the reference's expected structure, level of detail, and testing decisions as guidance, but do not copy unsupported project-specific content.
3. Map the user's feature, Test Plan ID, requirements, and test types to that guidance.
4. Confirm or clearly label missing decisions as assumptions or pending confirmation before drafting.
5. Draft or complete the test plan using the supplied information and the reference format, filling in the content with what is supported by the project.
6. Build the document-control header using the exact supplied plan ID and version, such as `ECO-UA-TP-01` and `1.0.0`.
7. Write an Executive Summary with product name, product description, and observable test objective.
8. Describe Test Implementation, Test Execution, and Test Completion activities, adapting the phase names only when the reference requires it.
9. Add the environment setup and schedule details in the reference's style, using project-specific setup rather than a fixed browser-centric template.
10. Add entry and exit criteria that are observable and specific to the feature.
11. Add a manual test-case summary only when requested. Use the companion `rp-login-test-case-summary` skill for its three-column format.
12. For unit tests or automated tests executed by a script, treat the test case as code: scenarios, test data, actions, and assertions belong in the test script, so do not create a duplicate summary by default.
13. If the user explicitly asks for a summary of unit or automated test cases, generate it, but state that it is a documentation summary only and that the executable test case remains in code.
14. Finish with a Test Change Log using supplied date, author, version, and change description, or label missing values as pending confirmation.

## Validation Checklist

- Title and Test Plan ID are present and consistent.
- Test-plan ID is distinguished from manual test-case IDs.
- All required sections are present.
- Executive Summary includes product name, product description, and test objective.
- Test Phases cover implementation, execution, and completion when the reference uses those phases.
- Environment Setup includes the relevant project-specific setup details, such as platform, tool, environment, data, or access requirements.
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
