# GATED Privacy Policy

_Last updated: 2026-08-09_

GATED is designed as a **local-first, project-bound AI software delivery control plane**.

## Repository content

GATED Marketplace services do **not** request, receive, upload, or store:

- repository file contents or source code;
- diffs, patches, or generated code;
- prompts or AI conversation context;
- local GATED documents, reports, task cards, or state files;
- repository secrets, credentials, environment files, or private keys.

The local GATED executable and its MCP server operate on the user's machine. Each MCP process is bound to one explicitly configured local project root.

## GitHub metadata

To operate a GitHub Marketplace listing, the metadata-only gateway may process the minimum GitHub metadata required for installation and plan lifecycle events, including:

- GitHub account ID, login, and account type;
- GitHub App installation ID;
- Marketplace plan ID and plan name;
- Marketplace event/action and effective date;
- webhook delivery ID.

The initial free gateway is stateless and does not intentionally persist full webhook payloads in an application database. Hosting infrastructure may temporarily retain sanitized operational logs according to the hosting provider's log-retention settings.

## GitHub App permissions

The initial GATED GitHub App does not request repository **Contents** permission. It is not designed to read repository source through the GitHub App.

## Third-party AI providers

If a user connects GATED to Claude, Codex, Cursor, ChatGPT, another cloud AI service, or a local model, that provider's own data-handling terms apply independently. GATED's promise that its Marketplace service does not receive repository source code does not change the behavior of the AI provider chosen by the user.

## Support

For privacy or security questions, open a support issue without attaching proprietary source code or secrets:

`https://github.com/areka38/gated-marketplace/issues`
