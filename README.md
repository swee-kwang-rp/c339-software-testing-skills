# c339-software-testing-skills
# RP QA Skills

Reusable Republic Polytechnic software-testing skills for student.

## Included Skills

- `rp-test-plan` - Creates structured test plans such as `EcoQuest - User Authentication Test Plan`.
- `rp-login-test-case-summary` - Creates simple manual login test-case summary tables.

## Install from GitHub

After publishing this folder as a GitHub repository:

```bash
npx skills add <your-github-username>/rp-qa-skills
```

Install only one skill:

```bash
npx skills add <your-github-username>/rp-qa-skills rp-login-test-case-summary
npx skills add <your-github-username>/rp-qa-skills rp-test-plan
```

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
