---
name: rp-manual-test-case
description: "Create a Republic Polytechnic manual test case using the school template for teaching and assessment. Use for cases that require a Test ID, Test Case title, Description, Preconditions, numbered Test Steps, Expected Results, and a pass/fail observation summary. Keep the format aligned to the provided teaching template and do not invent unsupported project details."
argument-hint: "Provide the feature, scenario, requirements, or example context"
---

# RP Manual Test Case

Create a manual test case using the school's teaching template. Follow the exact structure and wording style, and fill in only supported project details. If details are missing, label them as assumptions or pending confirmation instead of inventing facts.

## Template Structure

Use this structure exactly when the user has not supplied a different template:

**Test Case**

**Test ID**

`ECO-UA-TC-001`

**Test Case**

`Validate login succeeds with valid username and password`

**Description**

`Verify that a user can successfully log in when a valid registered username and correct password are entered.`

**Preconditions**

1. Login page is accessible.
2. A valid user account exists.
3. User is not currently logged in.

**Test Steps**

Provide detailed, sequential, and atomic steps that testers can follow without ambiguity. Each step should focus on a single action.

**Expected Results**

State the specific and measurable outcome of each action, and compare it directly with the observed result.

**SN | Pass | Fail | Observation**

| SN | Pass | Fail | Observation |
|---|---|---|---|
| 1 |  |  |  |
| 2 |  |  |  |
| 3 |  |  |  |

Then write the numbered scenario and sub-step format similar to the school example:

1. **Open the EcoQuest login page**
   1.1 Enter `https://c339-l3-bug-hunting.vercel.app/login` in the browser.

   **Expected result:**
   - The login page is displayed with the required fields and button.

2. **Enter a valid email address**
   2.1 Enter a valid registered email address in the Email Address field.

   **Expected result:**
   - The email is displayed correctly in the field.

3. **Enter the correct password**
   3.1 Enter the password associated with the registered email address in the Password field.

   **Expected result:**
   - The password is entered and displayed as masked characters.

4. **Submit the login credentials**
   4.1 Click the Login button.

   **Expected result:**
   - The credentials are submitted for authentication.

5. **Verify successful login**
   5.1 Observe the page displayed after clicking Login.

   **Expected result:**
   - The user is successfully logged in and redirected to the appropriate page.

## Procedure

1. Read the user's feature, requirement, or attached reference.
2. Identify the real scenario to be tested and write a clear test title.
3. Derive a unique Test ID from the project or test-plan prefix, following the broad-to-narrow naming pattern.
4. Write a concise Description that explains the purpose of the test.
5. List the Preconditions as numbered items that must be true before testing starts.
6. Write the Test Steps in a numbered sequence, using sub-steps such as `1.1`, `2.1`, and `3.1` when needed.
7. After each step, include an Expected Result that is specific and measurable.
8. Include a pass/fail observation table with the headings `SN`, `Pass`, `Fail`, and `Observation`.
9. Keep the wording simple, direct, and school-appropriate.
10. Do not invent details such as URLs, credentials, dates, statuses, or unsupported behaviors.
11. If a detail is missing, label it as `Pending confirmation` or `Assumption`.

## ID Rules

- Use a unique ID that helps reference the test case.
- For a test plan such as `ECO-UA-TP-01`, the test case IDs should start from `ECO-UA-TC-001`.
- Follow the pattern: `Project/System abbreviation - Feature/Component abbreviation - Test Case abbreviation - Sequence number`.
- Example: `ECO-UA-TC-001`.

## Test Case Writing Rules

- Test Case should be a short scenario title that describes the situation being tested.
- Description should explain the purpose of the test and what it validates.
- Preconditions should list the required conditions before testing can begin.
- Test Steps should be sequential, atomic, and easy to follow.
- Expected Results should be explicit and measurable.
- Each numbered test step should clearly show the action and the expected output.

## Pass / Fail / Observation Table Rules

- Use the column headings exactly as: `SN`, `Pass`, `Fail`, and `Observation`.
- Add one row per scenario or test condition.
- Use the `Pass` and `Fail` columns to show whether the outcome matched expectations.
- Use `Observation` to record what the tester actually saw.
- Keep the table simple and readable for a school report or slide.

## Boundaries

- This skill creates manual test cases.
- Do not transform it into a test plan or summary table unless the user explicitly asks for that format.
- Do not add extra columns unless the template requires them.
- Do not invent unsupported features, requirements, or credentials.
- If the user wants a summary table only, use the separate `rp-test-case-summary` skill instead.

## Validation Checklist

- The output uses the required structure and headings.
- Test ID is unique and follows the project naming pattern.
- Test Case title is clear and scenario-based.
- Description explains the test purpose.
- Preconditions are listed and realistic.
- Test Steps are sequential and specific.
- Expected Results are explicit and measurable.
- Pass/Fail/Observation table is included with the correct headings.
- No unsupported facts or invented placeholders are included.
