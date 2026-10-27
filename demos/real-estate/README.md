# Telugu–English real-estate demo
**Status: specification and fictional fixtures; not a running application.**

## Scenario
A prospective buyer asks Sabhuvi Agents about a home near Rajamahendravaram. The agent identifies language, location, budget, property type, and bedrooms, then offers matching fictional options or a human follow-up.

## Files
- [sample-properties.json](sample-properties.json): invented listings, INR prices, and explicitly unverified availability.
- [conversation.md](conversation.md): shared behavior and sample bilingual turns.
- [sample-lead.json](sample-lead.json): synthetic, unsent callback request.
- [acceptance-scenarios.md](acceptance-scenarios.md): manual checks to turn into tests when implemented.

## Conversation sequence
1. Identify as an AI demo and ask language preference.
2. Collect location, property type, budget, and bedrooms, one question at a time.
3. Confirm interpretation, especially lakh amounts and ambiguous locations.
4. Match fixture facts; explain when none match.
5. Answer only supported questions; escalate unknown availability, approvals, legal status, or negotiations.
6. Ask whether the user wants a human callback or site-visit request.
7. Ask permission before collecting contact details; summarize the draft.
8. Clearly state that the request is unsent and a visit is not confirmed.

## Demo limits
All prices, addresses, and properties are fictional. No real phone numbers, bookings, calls, CRM writes, or payments. Telugu prompts are a starting draft and require native-speaker validation before a customer pilot.
