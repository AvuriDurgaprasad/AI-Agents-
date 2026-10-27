# Environment variables
All names in [.env.example](../.env.example) are a proposed interface, not an implemented configuration contract.

| Variables | Intended purpose | When needed |
| --- | --- | --- |
| APP_ENV, DEMO_MODE | Environment and synthetic-data mode | First runtime |
| DEFAULT_LANGUAGE, SUPPORTED_LANGUAGES | Telugu (te) and English (en) | Shared conversation |
| PROPERTY_DATA_PATH | Local fictional listing fixture | Offline demo |
| LLM_PROVIDER, LLM_MODEL, LLM_API_KEY | Selected model and server-side credentials | After model decision |
| STT_PROVIDER, STT_API_KEY | Speech recognition | Voice prototype |
| TTS_PROVIDER, TTS_VOICE_TE, TTS_VOICE_EN, TTS_API_KEY | Speech synthesis and tested voice identifiers | Voice prototype |
| TELEPHONY_PROVIDER, TELEPHONY_API_KEY, TELEPHONY_FROM_NUMBER | Calling integration | Later approved calling work |
| PUBLIC_BASE_URL, WEBHOOK_SIGNING_SECRET | Callback URL and webhook authentication | External integration |
| CRM_PROVIDER, CRM_API_KEY, CRM_LEADS_ENDPOINT | Lead destination | After CRM decision |
| ENABLE_OUTBOUND_CALLS | Proposed default false | Future calling gate |
| ENABLE_CALL_RECORDING | Proposed default false | Future recording gate |
| ENABLE_LIVE_LEAD_SUBMISSION | Proposed default false | Future lead-delivery gate |

## Handling secrets
- Keep real values in a local ignored .env or a deployment secret store.
- Never place provider keys in browser code, frontend public variables, screenshots, or commits.
- Keep .env.example free of real keys and personal contact information.
- Verify locally with `git check-ignore .env` before staging files.
- If a credential is committed, revoke/rotate it; deleting the file alone is insufficient.
- Future code must validate required values per enabled feature and fail clearly when missing.
- Disabled integrations must not make external calls. Define and test this behavior when implementing the flags.
- Webhook signatures must be verified server-side before processing provider callbacks.

Provider-specific credentials and variable names may change after decisions. Document additions here and in the example together.
