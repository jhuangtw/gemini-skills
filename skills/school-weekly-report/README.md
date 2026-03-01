# School Weekly Report Skill

Summarizes recent school emails into **Upcoming Evvent**  tables **Action Item** for your child.

This directory contains a Gemini CLI **agent skill** packaged for reuse and customization.

## Prerequisites

- **Gemini CLI** installed and authenticated
- Access to email from Gemini CLI, I use the [Google Workspace Extension](https://github.com/gemini-cli-extensions/workspace):
  - `gemini extensions install https://github.com/gemini-cli-extensions/workspace`

## Installing the skill

```bash
gemini skills install https://github.com/jhuangtw/gemini-skills.git --path skills/school-weekly-report
```

This installs the `school-weekly-report` skill into your local Gemini CLI.

## Configuring for your child

Open `SKILL.md`:

- **Email patterns**: Update sender addresses, domains, or search terms to match your school.
- **Grades filter**: Set the grades/levels that apply to your student(s) so the tables only include relevant rows.

## Using the skill

Once installed and enabled in Gemini CLI:

1. Make sure your agent has access to your email inbox where school email are received (via MCP etc).
2. Ask the agent to `generate weekly school report` using the `school-weekly-report` skill.
