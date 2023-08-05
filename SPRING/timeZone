Here are some best practices for date time handling in a Spring app:

1. Use UTC/GMT as the default timezone in the code and database. All timestamps should be stored in UTC. This makes it easy to deal with users from different timezones.

2. Use Java 8 Date and Time API (LocalDateTime, OffsetDateTime, ZonedDateTime) instead of the legacy Date and Calendar classes. They are better designed and easier to use.

3. Expose UTC timestamps from the backend to the UI. Convert to the user's local timezone only in the front-end. This separates concerns and keeps the backend agnostic of user timezones.

4. For the database, store timestamps in UTC and use TIMESTAMP WITH TIME ZONE columns. This allows correct handling of daylight saving time changes.

5. In the UI, use a javascript library like Moment.js to handle date times. It has functions to convert between UTC and local timezones.

6. Define all timezones as strings, not numeric offsets. This is more robust and avoids issues like daylight saving time.

7. Avoid parsing user-inputted date strings. Instead, have the UI give a timestamp and timezone, and do the parsing on the backend. This ensures consistent parsing.

8. Be careful of edge cases like daylight saving time changes, leap years, and time offsets larger than +/-12 hours. Test thoroughly with sample data.

Hope this helps! Let me know if you have any other questions