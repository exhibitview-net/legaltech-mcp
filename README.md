# ExhibitView Legaltech Intelligence MCP

Legaltech funding, acquisitions and event research inside your AI assistant.

**This is the public documentation repository. It does not contain the hosted server implementation or the underlying research collection.** The production application is maintained separately in a private repository. This repository explains what the service exposes and how to connect; it is not a source-code audit of the hosted service.

[Connect your assistant](https://exhibitview-mcp.vercel.app/) · [Usage and analytics](https://exhibitview-mcp.vercel.app/usage) · [Tool details](TOOLS.md) · [Coverage and methodology](COVERAGE.md)

## Connect

Public Streamable HTTP endpoint:

```text
https://exhibitview-intelligence.vercel.app/public/mcp
```

No ExhibitView account, API key, token or OAuth is required. Public usage limits apply; your assistant provider may have separate account requirements or charges.

Choose your assistant on the connection page and copy the setup prompt, or use an example in [setup/](setup/). Merge configuration into existing settings instead of replacing unrelated servers. An assistant may need a restart to load the connection. ChatGPT and Claude web/Desktop can require manual settings and account features. The hosted MCP does not require downloading a server or running this repository.

For Copilot CLI, this command was used in the supplied installation test:

```sh
copilot mcp add --transport http exhibitviewPublic https://exhibitview-intelligence.vercel.app/public/mcp
```

Then reopen Copilot if necessary. Setup is separate from research or diagnostics.

## What you can ask

- Which legaltech companies raised funding in September 2026? Include sources.
- What acquisitions does ExhibitView record for Legora, and when were they announced?
- Show Harvey's recorded funding history and distinguish extensions from separate rounds.
- Which legaltech events are listed for 2027, and which details need confirmation?

## What has been tested

Actual research calls: Codex CLI, Claude Code and Copilot CLI. Copilot CLI was confirmed by the user with a real ExhibitView tool call and a sourced funding answer on October 25, 2026. VS Code Copilot, ChatGPT and Claude web/Desktop remain end-to-end unvalidated. Providing setup guidance is not proof of a successful connection in every client.

## Research coverage

Transactions: January–September 2026. Event candidates: October 2026–December 2027. Coverage is not exhaustive. Records include source links, review labels and unresolved conflicts. Event candidates include unverified research. Confirm event details with organizers. Queries do not independently open source pages, and no automatic refresh schedule is promised.

## Permissions and operational analytics

Six read-only research tools; no data-update or administrative actions are exposed. This describes the MCP's capabilities, not permissions held by the assistant application's other tools. Windgrove monitors tool activity for ExhibitView through Armature. Hosting infrastructure may process request metadata; your assistant provider has separate data practices. Do not submit confidential case material, client information or secrets. See the linked usage notice.

## Feedback

Open an issue for setup problems or record corrections. Include the assistant/client, the public error message and a reproducible question. Do not include credentials, confidential data or private assistant configuration. Product enquiries: [ExhibitView](https://exhibitview.net/).

## Registry metadata

[server.json](server.json) is prepared for the Official MCP Registry. It passed Registry metadata validation on October 25, 2026. That does not mean the listing has been published, reserved or approved. See the actual Registry for current publication status.
