# School Upcoming Events

## Data Extraction Logic
1.  **Find Emails:** use emails passed in from context.
2.  **Identify Events:**
   -   Example events:
        -   field trips, day off, holidays and breaks, meetings, school-wide events. Be very thorough with recurring events.
    -   Pay special attention to "Calendar of Events" section of emails and analyze the events listed carefully.
    -   Look for dates, times, and locations
    -   If multiple dates are mentioned for the same event, list each date in a separate row.
3.  **Table Structure:**
    -   **Date** Date formatted MM/DD. List multiple dates in separate rows if an event repeats.
    -   **Time** Start/End times (e.g., 10:00 AM – 2:30 PM).
    -   **Grades** Specify which grade level (e.g., Level 1, All. If unsure, use All).
    -   **Event** Concise name of the event.
    -   **Location** Specific location (e.g., Filoli Gardens, SportsHouse).
    -   **Email** Subject truncated to 50 chars with ellipsis if needed.