# Voice agents
**Status: implementation placeholder.**

Planned flow: microphone/voice transport → speech recognition → shared real-estate conversation logic → speech synthesis → user.

## Intended responsibilities
- Ask the preferred language and support Telugu/English switching.
- Handle silence, interruptions, unclear speech, and retries.
- Confirm budget and contact details instead of trusting uncertain transcription.
- Offer a human callback when unable to understand or answer.
- Use the same approved listing facts and lead fields as chat.

## Future areas (not yet implemented)
- `adapters/`: selected speech and transport providers.
- `sessions/`: turn handling and interruption logic.
- `tests/`: bilingual audio and recovery tests.

Start with [the demo](../demos/real-estate/README.md). Providers, voice IDs, runtime, latency targets, and calling setup remain TBD. Do not assume Telugu quality from a vendor label alone. No outbound calls or recordings are enabled.
