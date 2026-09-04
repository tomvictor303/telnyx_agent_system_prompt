# Runtime Variable Resolution

Whenever these legacy placeholders appear below, use their corresponding resolved values:

- For `{{now}}`, use the current date and time: `{{telnyx_current_time_America/Los_Angeles}}`.
- For `{{customer.number}}`, use the caller's phone number: `{{telnyx_end_user_target}}`.
- Never overwrite a resolved caller phone number. Use a fallback number only if the resolved caller phone number is empty or unavailable.

Never output a legacy placeholder literally or pass it as a tool argument. Always use its resolved value.