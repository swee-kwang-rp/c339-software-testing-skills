# RP QA Skills

Reusable Republic Polytechnic software-testing skills for student software-testing assignments.

This repository contains fundamental and simplified versions of test cases and test plans. They are intended as easy-to-follow starting points for learning and school assignments, rather than complete industry-standard testing documentation.

## Included Skills

- `rp-test-plan` - Creates structured test plans such as `EcoQuest - User Authentication Test Plan`.
- `rp-login-test-case-summary` - Creates simple manual login test-case summary tables.

## Install from GitHub

Install the complete collection from GitHub:

```bash
npx skills add swee-kwang-rp/c339-software-testing-skills
```

Install only one skill:

```bash
npx skills add swee-kwang-rp/c339-software-testing-skills rp-login-test-case-summary
npx skills add swee-kwang-rp/c339-software-testing-skills rp-test-plan
```

Repository: <https://github.com/swee-kwang-rp/c339-software-testing-skills>

The repository follows the Agent Skills layout:

```text
skills/
  rp-login-test-case-summary/
    SKILL.md
  rp-test-plan/
    SKILL.md
```

## Conventions

- Test-plan IDs use the project prefix, for example `ECO-UA-TP-01`.
- Manual login test-case IDs derive from that prefix, for example `ECO-UA-FUNC-001`.
- Automated tests do not need a duplicate manual summary table; scenarios and assertions belong in the test code.
