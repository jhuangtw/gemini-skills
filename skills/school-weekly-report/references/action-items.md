# School Action Items

## Data Extraction Logic
1.  **Find Emails:** use emails passed in from context.
2.  **Analyze Content:** Look for:
    -   Call to action and links (e.g., school-specific app like Blackbaud, Google Forms, ordering or payment/ordering links, enrollment agreement, etc).
        -   links are extremely important, keep track of and prioritize them
    -   Specific call out for time of arrival or dismissal for events.
    -   Events to RSVP for.
    -   Items to bring to school or pack (e.g., lunches, gear).
    -   Special clothing, shoes, or gear requirements (e.g., field trips, sports).
    -   Important deadlines.
    -   include action items due in the last week
3.  **Table Structure:**
    -   **Due Date** Date formatted MM/DD.
    -   **Grades** Specify which grade level (e.g., Level 1, All. If unsure, use All).
    -   **Action Item** Concise description. If associated with an event, include the event name (e.g., "Pack lunch for Nature Day")
    -   **Email** Subject truncated to 50 chars with ellipsis if needed.
