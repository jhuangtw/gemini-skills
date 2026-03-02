# School Weekly Report Skill

Summarizes recent school emails into **Upcoming Evvent**  tables **Action Item** for your child.

This directory contains a Gemini CLI **agent skill** packaged for reuse and customization.

## Prerequisites

- [**Gemini CLI**](https://geminicli.com/) installed and authenticated
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

### Example Output

> #### Upcoming Events
>
> | Date  | Time               | Grades  | Event                                        | Location                             | Email                                              |
> |-------|--------------------|---------|----------------------------------------------|--------------------------------------|----------------------------------------------------|
> | 03/05 | 10:00 AM – 2:30 PM | Level 1 | Nature Day                                   | Filoli Gardens                       | Synapse/ Riekes Nature Day for Level 1             |
> | 03/13 | TBD                | All     | Interactive Lab                              | Synapse School                       | Synapse Narwhal News: Lab & Benefit Details, He... |
> | 03/19 | 10:00 AM – 2:30 PM | Level 1 | Nature Day                                   | Filoli Gardens                       | Synapse/ Riekes Nature Day for Level 1             |
> | 03/19 | TBD                | Adults  | San Mateo County Planning Commission Meeting | San Mateo County Planning Commission | Update on Last Night’s North Fair Oaks Council ... |
> | 03/26 | 10:00 AM – 2:30 PM | Level 1 | Nature Day                                   | Filoli Gardens                       | Synapse/ Riekes Nature Day for Level 1             |
> | 04/16 | 10:00 AM – 2:30 PM | Level 1 | Nature Day                                   | Filoli Gardens                       | Synapse/ Riekes Nature Day for Level 1             |
>
> #### Action Items
>
> | Due Date | Grades  | Action Item                                              | Email                                              |
> |----------|---------|----------------------------------------------------------|----------------------------------------------------|
> | 03/01    | Parents | Automatic payment of $165.00 scheduled for debit         | Automatic Payment Reminder for Synapse School      |
> | 03/02    | Level 1 | Complete Nature Day Program Form and Waiver \[1]         | Reminder: Level 1_2025-26 Nature Day Program Fo... |
> | 03/05    | Level 1 | Bring-Your-Own-Lunch (no Choice Lunch) for Nature Day    | Synapse/ Riekes Nature Day for Level 1             |
> | TBD      | Level 1 | Review Nature Day Orientation Slides \[2]                | Banana Slugs Class Notes - 2/27                    |
> | TBD      | All     | Review Burton Lab Resource Board for Interactive Lab \[3] | Banana Slugs Class Notes - 2/27                    |
>
> #### Important Links
> 1. Blackbaud (Nature Day Form/Waiver): https://_link.to.form_
> 2. Nature Day Orientation Slides: https://_link.to.file_
> 3. Burton Lab Resource Board: https://_link.to.info_
