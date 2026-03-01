---
name: school-weekly-report
description: Summarizes recent school emails into action item and event tables.
---

# School Weekly Updates

This skill streamlines the process of extracting, summarizing, and presenting upcoming school events and action items from school emails.

## Configuration
1. School email patterns to look for:
   - specific addresses: noreply@synapseschoolorg.myenotice.com, synapseschool@myschoolapp.com
   - from email sender with domain @synapseschool.org
   - general search terms: "Synapse School"
2. Grades filter: Level 1, L1, All, Adults, Parents

## Workflow
To generate a weekly summary:

1.  **Email Search & Content Retrieval**
    -   Find all emails following email patterns specified from configuration section, sent in the last 2 weeks
    -   Retrieve the full content of each relevant message. If the email payload is in html, first convert it to markdown or plain text to be able to extract relevant information. Be specific about grades applicable to each piece of information.
2.  **Table Generation:**
    -   IMPORTANT: follow table presentation rules set below
    -   Follow extraction & table schema in **[upcoming-events.md](references/upcoming-events.md)** to display Upcoming Events table
    -   Follow extraction & table schema in **[action-items.md](references/action-items.md)** to display Action Items table
    -   present Action Items at the very end

## Table presentation rules
- IMPORTANT: do not change column name or ordering
- IMPORTANT: update each table to only include rows from grades specified in configuration section
- sort chronologically
- Display table in a clean, well-spaced Markdown.
- Include a numbered link suffix `[n]` for action item / event with important links (RSVP, form, payment, log-in link etc).
- Add an "Important Links" legend below the table with the numbered URLs. Sort from most important to least important

## Validation
-   there should be no row in any table presented that does not apply to the grades specified in configuration section

## Reference Material
-   [Upcoming Events Extraction Guide](references/upcoming-events.md)
-   [Action Items Extraction Guide](references/action-items.md)

## Future Ideas
-   sync to calendar (if not already there) and google