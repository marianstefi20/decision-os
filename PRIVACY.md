# Privacy Policy

**Decision OS MCP** — Privacy Policy

Last updated: 2025-02-08

## Overview

Decision OS MCP is a local-only MCP (Model Context Protocol) server for decision tracking and learning. It runs entirely on your machine and does not transmit any data to external services.

## Data Collection

Decision OS MCP does **not** collect, transmit, or share any user data. Specifically:

- **No telemetry** — no usage data is sent anywhere.
- **No analytics** — no tracking, metrics, or behavioral data is collected.
- **No network calls** — the server communicates only via stdio with the MCP client (e.g., Cursor, Claude Desktop). It makes no outbound network requests.
- **No third-party services** — no external APIs, databases, or cloud services are used.

## Data Storage

All data is stored **locally on your filesystem** in two locations:

- **Project scope:** `.decision-os/` directory within your project folder.
- **Global scope:** `~/.decision-os/` directory in your home folder.

Data is stored as YAML files and includes:

- Cases (units of work)
- Pressure events (surprises encountered during work)
- Foundations (compressed learnings)
- Project configuration

You have full control over this data. You can read, edit, or delete it at any time using any text editor or file manager.

## Data Sharing

Decision OS MCP does not share data with anyone. Since data is stored as plain files in your project directory, sharing is entirely under your control (e.g., if you choose to commit `.decision-os/` to a Git repository).

## Third-Party Dependencies

Decision OS MCP depends on the following npm packages, none of which collect user data:

- `@modelcontextprotocol/sdk` — MCP protocol implementation
- `yaml` — YAML parsing/serialization
- `zod` — Schema validation

## Changes to This Policy

Changes to this privacy policy will be reflected in this file and in the project's release notes.

## Contact

For questions about this privacy policy, please open an issue on the [GitHub repository](https://github.com/marianstefanescu/decision-os-mcp/issues).
