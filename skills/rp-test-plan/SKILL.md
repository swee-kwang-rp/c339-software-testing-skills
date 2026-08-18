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

## Title Naming Rules

- Order the title from broadest to narrowest, ending with the artifact type.
- Keep the product or system name first, then the feature or component, and finish with the document type.
- Best practice format: `[Product] – [Feature/Component] [Artifact Type]`.
- Example: `EcoQuest – User Authentication Test Plan`.
- Use the same logic for other artifacts when relevant, such as `EcoQuest – User Authentication Test Cases`.

## ID Naming Rules

- A test plan ID should be a unique code that identifies the plan and follows the same broad-to-narrow structure as the title.
- The ID is derived from the product, feature, artifact type, and running sequence number.
- Format: `XX-XX-XX-##`.
- Each section is ordered from broadest to narrowest: product/system, feature/component, artifact type, running sequence.
- Example: `ECO-UA-TP-01`.
- Breakdown: `ECO` = EcoQuest, `UA` = User Authentication, `TP` = Test Plan, `01` = sequence number.
- Keep the parts consistent with the title so each section can be clearly distinguished and matched to the artifact.

## Versioning Rules

- Version tracks changes to the document and should use semantic versioning (SemVer).
- Use the same versioning scheme as software: `MAJOR.MINOR.PATCH`.
- Increase the version when changes affect the document significantly, the content is revised, or a new approved draft is issued.
- Example: `Version 3.2.14`.
- Keep the version consistent with the document revision history and change log.

## Executive Summary Rules

- Executive Summary provides a brief overview of the system and its intended purpose.
- Product Name is the name of the application, system, or product being tested. It is normally the same as the test plan title.
- Product Description is a short explanation of what the product does, who it is for, and its main functions or features.
- Test Objective states what the testing aims to verify, such as whether key functions work correctly, requirements are met, and important defects are identified before release.
- The test objective should list the main goals of testing, such as verifying functionality, performance, usability, and security where relevant.
- Keep the summary brief, clear, and aligned with the actual feature or system being tested.

## Test Phases Rules

- Test Phases outline the stages of testing, such as preparation, execution, and closure, and describe what activities happen in each phase.
- For most software applications, the standard test plan can include three phases: Test Implementation, Test Execution, and Test Completion.
- Test Implementation covers preparing test data, confirming the setup, reviewing requirements, and finalising the planned test activities.
- Test Execution covers running the tests, recording outcomes, identifying defects, and checking whether the expected results are achieved.
- Test Completion covers reviewing results, confirming exit conditions, logging defects or follow-up actions, and closing the test activity.
- Use these phase names unless the reference template specifies different labels.

## Environment Setup Rules

- Environment Setup describes the setup and resources required before testing can begin.
- It ensures that testers use the correct environment so that test results are consistent, reliable, and repeatable.
- The environment can include hardware, software, platforms, application files, runtimes, databases, test accounts, and evidence-recording methods.
- Hardware examples may include laptop or workstation specifications, such as memory or processing requirements.
- Application examples may include frontend and backend source files or deployment builds.
- Runtime examples may include frameworks or tools such as Node.js, Java, or other required runtime versions.
- Database examples may include MySQL, PostgreSQL, SQLite, or other supported database types and versions.
- Test Accounts includes valid credentials, roles, or login scenarios required for testing.
- Evidence and Recording should explain how defects or failed test cases are captured, such as screenshots, notes, recorded logs, or issue tracking evidence.
- Include only the setup items that are relevant to the actual project; do not force a fixed list when the project needs a different environment.

## Schedule Rules

- Schedule is a timeline showing when each phase or activity will occur.
- Day refers to the planned day when the testing activity will be carried out, such as Day 1, Day 2, or a specific date.
- Period refers to the time slot or session within that day, such as Period 1, Period 2, or another class/session label.
- A schedule may include multiple periods in one day, such as Day 1 – Period 1 and Day 1 – Period 2.
- Topics/Activity refers to the testing phase or specific work to be performed, such as Test Implementation, Test Execution, or Test Completion.
- Keep the schedule aligned with the actual project timeline and test phases, using the reference format only when required.

## Entry and Exit Criteria Rules

- Entry Criteria defines the conditions that must be met before testing can start.
- Exit Criteria defines the conditions that must be met before testing can end.
- Entry Criteria ensures the system or feature is ready for testing and that the required setup, requirements, and test data are available.
- Exit Criteria ensures testing is sufficiently completed and that the planned activities have been carried out to an acceptable level.
- Typical entry conditions may include requirements being available, the application being accessible, test data being ready, and the tester being able to reach the target feature.
- Typical exit conditions may include the planned high-priority tests being executed, defects being logged, critical defects being resolved or accepted, and results being reviewed.
- Keep the criteria observable, realistic, and specific to the project.

## Test Case Summary Table Rules

- Test Case Summary Table provides a quick overview of all test cases planned for testing.
- Test Case ID is a unique code used to identify each test case and should be derived from the test plan ID.
- The format follows the plan structure, with the artifact type changed from `TP` for Test Plan to `TC` for Test Case.
- Example: if the Test Plan ID is `ECO-UA-TP-01`, the first test case should start as `ECO-UA-TC-001`.
- Test Case is a short description of what is being tested, written as a concise scenario or validation point.
- Type identifies the category of testing and must use one of the approved values only: `Valid`, `Invalid`, `Functional`, `Validation`, `UI`, or `Security`.
- Do not invent other type names. Use the most specific matching category for each test case.
- Include only the relevant cases for the feature and keep the summary brief, readable, and aligned with the project requirements.
- If the companion test-case skill is available, follow that format and naming pattern for consistency.

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
