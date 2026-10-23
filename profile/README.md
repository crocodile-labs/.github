# Crocodile Labs

We build open-source security tools for developers who work with AI coding agents.

<p align="center">
  <a href="https://github.com/crocodile-labs/openmoat">
    <picture>
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/crocodile-labs/openmoat/main/docs/assets/banner-light.svg">
      <img src="https://raw.githubusercontent.com/crocodile-labs/openmoat/main/docs/assets/banner-dark.svg" alt="OpenMoat: security for AI coding agents">
    </picture>
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=claude&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/Codex-412991?style=flat-square&logo=openai&logoColor=white" alt="Codex">
  <img src="https://img.shields.io/badge/Cursor-000000?style=flat-square&logo=cursor&logoColor=white" alt="Cursor">
  <img src="https://img.shields.io/badge/OpenClaw-E5484D?style=flat-square" alt="OpenClaw">
  <img src="https://img.shields.io/badge/GitHub_Copilot_CLI-000000?style=flat-square&logo=githubcopilot&logoColor=white" alt="GitHub Copilot CLI">
  <img src="https://img.shields.io/badge/pi-6E56CF?style=flat-square" alt="pi">
  <img src="https://img.shields.io/badge/Gemini_CLI-8E75B2?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini CLI">
  <br>
  <img src="https://img.shields.io/badge/macOS-000000?style=flat-square&logo=apple&logoColor=white" alt="macOS">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/Windows-0078D4?style=flat-square" alt="Windows">
</p>

## [OpenMoat](https://github.com/crocodile-labs/openmoat)

OpenMoat checks every command, file access, web request and MCP call your coding agent
makes, and blocks the dangerous ones before they run. It works with **Claude Code**,
**Codex**, **Cursor**, **OpenClaw**, **GitHub Copilot CLI**, **pi** and **Gemini CLI**.
Everything it has no rule for it leaves to your agent's own prompt, so your work goes on
as before.

- **Blocks** reading or sending your keys, tokens and `.env` files, unknown hosts,
  `curl … | sh`, destructive git and file commands, and an agent switching it off.
- **Bounds hidden code:** the same policy configures the OS sandbox of Claude Code, Codex
  and Cursor, so a script inside `npm test` cannot reach your secrets.
- **Holds changed MCP servers:** each server definition is pinned, and a new or changed
  one waits for `openmoat mcp accept`.
- **Records** every decision in a local audit log that detects tampering.
- **Runs locally:** one Rust binary for macOS, Linux and Windows; no AI model decides.

```bash
brew install crocodile-labs/tap/openmoat && openmoat init
```

[Website](https://openmoat.dev) · [Docs](https://openmoat.dev/docs/) · [Blog](https://openmoat.dev/blog/) · [Releases](https://github.com/crocodile-labs/openmoat/releases) · [r/openmoat](https://www.reddit.com/r/openmoat/)

## Repositories

| Repository | What |
|---|---|
| [openmoat](https://github.com/crocodile-labs/openmoat) | the `openmoat` command: hook, policy engine, sandboxes, MCP pinning, egress proxy, audit log |
| [openmoat.dev](https://github.com/crocodile-labs/openmoat.dev) | the website, docs and blog |
| [homebrew-tap](https://github.com/crocodile-labs/homebrew-tap) | the Homebrew formula: `brew install crocodile-labs/tap/openmoat` |

## Get involved

Questions and ideas: [r/openmoat](https://www.reddit.com/r/openmoat/). Bugs and false
positives: [OpenMoat issues](https://github.com/crocodile-labs/openmoat/issues/new/choose).
Found a way past OpenMoat? Please report it privately, as described in
[SECURITY.md](https://github.com/crocodile-labs/openmoat/blob/main/SECURITY.md).

Licensed under either of Apache License 2.0 or MIT, at your option.
