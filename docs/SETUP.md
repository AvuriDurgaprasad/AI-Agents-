# Setup guide
## What works today
This repository contains documentation and fictional demo fixtures. It has no server, package manifest, install command, or launch command yet. Reading the files requires no paid subscription.

## Get the workspace
Install Git if needed, then run in a terminal:
```sh
git clone https://github.com/AvuriDurgaprasad/AI-Agents-.git
cd AI-Agents-
```
Alternatively, use GitHub **Code → Download ZIP**, extract it, and open the folder in your editor.

## Optional local configuration
Only when starting implementation, copy the example:
- Windows PowerShell: `Copy-Item .env.example .env`
- macOS/Linux: `cp .env.example .env`

Leave provider values empty until providers are selected. The proposed flags do not enforce behavior until application code implements them. See [environment guidance](ENVIRONMENT.md).

## Rehearse the demo without services
1. Open [the demo](../demos/real-estate/README.md).
2. Read the fictional listings and bilingual conversation.
3. Play the customer and agent roles; use only supplied listing facts.
4. Walk through [acceptance scenarios](../demos/real-estate/acceptance-scenarios.md).
5. Record unresolved choices in [DECISIONS.md](DECISIONS.md).

తెలుగులో: ప్రస్తుతం ఇది ప్రారంభ workspace మాత్రమే. ముందుగా demo conversation చూడండి. Provider ఎంపిక పూర్తయ్యాక మాత్రమే API keys జోడించండి.

## After choosing the stack
Add real dependency manifests, supported runtime versions, install/start commands, configuration validation, and meaningful tests. Update this guide with commands verified against the implementation. Do not invent commands before code exists.
