# Milestone 1 — private bilingual real-estate prototype
**Current state:** starter documents and fixtures complete; runtime work has not started.
**Outcome:** a locally runnable or private prototype demonstrating a grounded Telugu–English enquiry and an unsent synthetic lead draft.

## Work plan
| Step | Deliverable | Completion evidence |
| --- | --- | --- |
| 1. Resolve stack | Runtime, model, and speech evaluation choices in DECISIONS.md | Decisions with reasons and cost assumptions |
| 2. Implement shared logic | Fixture lookup, requirements, language preference, and draft lead validation | Correct matches, no-match and consent checks |
| 3. Build text demo | Simple chat UI and server-side handler | Telugu, English, and language-switch walkthroughs |
| 4. Evaluate voice | Browser microphone proof of concept with selected STT/TTS | Native Telugu review and recorded test results without private customer data |
| 5. Verify and document | Repeatable install/start instructions, configuration errors, acceptance results | Fresh setup and reviewed scenarios |

## Definition of done
- [ ] A fresh checkout runs using documented, verified commands.
- [ ] Telugu and English flows use only fixture facts.
- [ ] All applicable [acceptance scenarios](../demos/real-estate/acceptance-scenarios.md) pass with evidence.
- [ ] A synthetic callback request remains unsent; no confirmed booking is claimed.
- [ ] Secrets remain server-side and ignored locally.
- [ ] Disabled integrations make no external calls or recordings.
- [ ] Voice works with native-speaker validation, or is explicitly marked blocked with evidence and a revised milestone scope accepted by the owner.
- [ ] Provider usage/cost observations, known limitations, and next actions are documented.

## Out of scope
Production hosting, outbound campaigns, live telephone numbers, real customer data, WhatsApp integration, CRM delivery, payments, and real bookings.

## Follow-up milestone (TBD)
After reviewing the prototype, choose one real integration, approve source listings, define consent and retention behavior, and plan a limited human-supervised pilot. Timeline and budget remain TBD until the stack is selected.
