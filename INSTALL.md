# Install GATED Free Preview

Download the latest `v0.3.0-preview` asset for your operating system from GitHub Releases.

## Windows x86_64

Download `gated-windows-x86_64.exe`, place it in a directory on `PATH`, and optionally rename it to `gated.exe`.

## Linux x86_64

Download `gated-linux-x86_64`, mark it executable, place it on `PATH`, and optionally rename it to `gated`.

## macOS Apple Silicon

Download `gated-macos-arm64`, mark it executable, place it on `PATH`, and optionally rename it to `gated`.

## macOS Intel

Download `gated-macos-x86_64`, mark it executable, place it on `PATH`, and optionally rename it to `gated`.

## Preview signing status

The current Free Preview binaries are CI-built but **not yet platform code-signed/notarized**. Windows SmartScreen or macOS Gatekeeper may therefore show an unknown-developer warning. Verify the SHA-256 checksum from the release before running the binary. Signed installers are planned before a polished production release.

## Verify GATED

```text
gated --help
```

Initialize a project:

```text
gated init . --idea "Describe the product, target user, problem, and expected value." --git-init
```

Inspect supported MCP clients:

```text
gated --root . connect --list
```

For a generic MCP client, print the exact project-bound stdio configuration without modifying client settings:

```text
gated --root . connect --client generic
```

GATED binds MCP to the exact project root. Do not configure it with your home directory or a parent directory containing multiple projects.
