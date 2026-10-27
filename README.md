# Sabhuvi Agents
Telugu–English voice and chat agents for business enquiries, starting with a real-estate demo.

> **Status: planning and starter workspace.** No runnable agent, telephony connection, website widget, CRM integration, or deployment is implemented yet. All sample properties and conversations are fictional.

## First demo
Help a prospective buyer choose Telugu or English, describe a property requirement, explore matching sample listings, and request a human callback or site visit. Support natural language switching while keeping prices, locations, and availability grounded in the demo data.

## Workspace
| Path | Purpose |
| --- | --- |
| [docs/SETUP.md](docs/SETUP.md) | Getting started, including Windows instructions |
| [docs/ENVIRONMENT.md](docs/ENVIRONMENT.md) | Proposed configuration and secret handling |
| [docs/MILESTONE-1.md](docs/MILESTONE-1.md) | First milestone, deliverables, and acceptance checks |
| [docs/DECISIONS.md](docs/DECISIONS.md) | Open implementation decisions |
| [voice-agents/](voice-agents/README.md) | Voice channel scope and integration placeholders |
| [chat-agents/](chat-agents/README.md) | Chat channel scope and integration placeholders |
| [demos/real-estate/](demos/real-estate/README.md) | Bilingual conversation, fictional listings, lead example, and checks |
| [.env.example](.env.example) | Proposed configuration template; no working credentials |

## Start here
1. Follow [setup](docs/SETUP.md); no API key or paid service is needed to review this workspace.
2. Read the [demo brief](demos/real-estate/README.md) and rehearse the sample conversation.
3. Resolve the blocking items in [decisions](docs/DECISIONS.md).
4. Implement and validate [milestone 1](docs/MILESTONE-1.md).

## Planned capabilities
- Telugu and English enquiries, including mixed-language turns.
- Property requirements: location, budget in INR, property type, and bedrooms.
- Answers from approved listing data; explicit uncertainty when information is missing.
- Consent-based callback requests and human handoff.
- Shared business rules across chat and voice.

## Implementation boundaries
Runtime, model provider, speech recognition, speech synthesis, telephony, hosting, and CRM are **TBD**. No vendor's Telugu support is assumed. Verify speech quality with real Telugu samples before choosing a provider. Inbound/outbound calling and live lead delivery are later decisions, not enabled features.

Use synthetic data during development. Keep credentials, real phone numbers, recordings, and customer transcripts out of Git. A visit request is not a confirmed booking, and listing information is not a legal or investment assurance.

## License
TBD — repository owner must choose a license before reuse permissions are advertised.
