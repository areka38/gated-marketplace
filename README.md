# GATED

**Governed AI Tooling & Engineering Delivery**

**Local-first. Project-bound. Governed AI delivery.**

GATED is a deterministic control plane for AI-assisted software delivery. It binds MCP access to one local project root, enforces lifecycle and write boundaries, and keeps critical human approvals explicit.

## Free Preview

GATED Free Preview is currently **$0**.

Native standalone binaries are published on this repository's **Releases** page. The release pipeline builds and smoke-tests these targets natively:

- Windows x86_64
- Linux x86_64
- macOS Apple Silicon (arm64)
- macOS Intel (x86_64)

Users do not need Python or FastMCP installed to run the standalone binary.

## Privacy boundary

GATED runs on the user's machine. The GATED Marketplace service does **not** request GitHub repository `Contents` permission and does not receive repository source files, diffs, prompts, generated code, local GATED documents, or secrets.

Each MCP process is bound to exactly one absolute local project root.

## Quick start

See [INSTALL.md](INSTALL.md), then:

```text
gated init /path/to/project --idea "Describe what is being built, for whom, and the expected value" --git-init
gated --root /path/to/project connect --list
gated --root /path/to/project connect --client claude-code
```

Supported connection helpers: Claude Code, Codex, Cursor, Claude Desktop (macOS/Windows), and Generic MCP.

The generated customer project does **not** contain the GATED controller/MCP source code. The controller remains in the standalone executable.

## Support and policies

- [Install](INSTALL.md)
- [Privacy](PRIVACY.md)
- [Terms](TERMS.md)
- [Support](SUPPORT.md)
- [Distribution notice](LICENSE.md)

Do not post proprietary source code, credentials, or private AI conversation content in public issues.

The GATED implementation is proprietary. This public repository is the distribution, policy, and support surface; it is not the product source repository.
