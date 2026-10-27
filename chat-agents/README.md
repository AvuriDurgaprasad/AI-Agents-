# Chat agents
**Status: implementation placeholder.**

Planned flow: chat UI → server-side conversation handler → approved property data → reply and optional draft lead.

## Intended responsibilities
- Offer Telugu and English and allow a mid-conversation switch.
- Ask one requirement at a time and confirm the interpreted budget.
- Match only fictional fixture listings during milestone 1.
- Say when no match or verified answer is available.
- Obtain consent before creating a callback request.
- Show a draft request summary without claiming it was delivered.

## Future areas (not yet implemented)
- `ui/`: web chat interface.
- `handlers/`: server-side turns and session handling.
- `tests/`: grounding, language switching, and lead consent checks.

Framework, model, session storage, website embedding, and CRM adapter remain TBD. API secrets must stay server-side. See [milestone 1](../docs/MILESTONE-1.md).
