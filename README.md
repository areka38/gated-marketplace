# GATED

**Local-first governed AI software delivery.**

GATED is a deterministic control plane for AI-assisted software delivery. It binds MCP access to one local project root, enforces lifecycle and write boundaries, and keeps critical human approvals explicit.

## Privacy boundary

GATED runs on the user's machine. The GATED Marketplace service does **not** request GitHub repository `Contents` permission and does not receive repository source files, diffs, prompts, generated code, local GATED documents, or secrets.

## Install

Native Windows, macOS, and Linux binaries will be published on this repository's **Releases** page after the cross-platform release workflow succeeds.

Typical local flow:

```text
gated init /path/to/project --idea "Describe what is being built, for whom, and the expected value" --git-init
gated --root /path/to/project connect --client claude-code
```

Supported connection helpers: Claude Code, Codex, Cursor, Claude Desktop (macOS/Windows), and Generic MCP.

Each MCP process is bound to exactly one absolute local project root.

## Support and policies

- [Privacy](PRIVACY.md)
- [Terms](TERMS.md)
- [Support](SUPPORT.md)

The GATED implementation is proprietary. This public repository is the distribution, policy, and support surface; it is not the product source repository.
