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

## [OpenMoat](https://github.com/crocodile-labs/openmoat)

OpenMoat checks every command, file access, web request and MCP call your coding agent
makes, and blocks the dangerous ones before they run. It works with **Claude Code**,
**Codex** and **Cursor**. Everything it has no rule for it leaves to your agent's own
prompt, so your work goes on as before.

- **Blocks** reading or sending your keys, tokens and `.env` files, unknown hosts,
  `curl … | sh`, destructive git and file commands, and an agent switching it off.
- **Bounds hidden code:** the same policy configures each agent's OS sandbox, so a
  script inside `npm test` cannot reach your secrets.
- **Records** every decision in a local audit log that detects tampering.
- **Runs locally:** one Rust binary, about 10 ms per check, no AI model decides.

```bash
brew install crocodile-labs/tap/moat && moat init
```

[Website](https://openmoat.dev) · [Docs](https://openmoat.dev/docs/) · [Blog](https://openmoat.dev/blog/) · [Releases](https://github.com/crocodile-labs/openmoat/releases) · [r/openmoat](https://www.reddit.com/r/openmoat/)

## Repositories

| Repository | What |
|---|---|
| [openmoat](https://github.com/crocodile-labs/openmoat) | the `moat` command: hook, policy engine, sandboxes, audit log |
| [openmoat.dev](https://github.com/crocodile-labs/openmoat.dev) | the website, docs and blog |
| [homebrew-tap](https://github.com/crocodile-labs/homebrew-tap) | the Homebrew formula: `brew install crocodile-labs/tap/moat` |

## Get involved

Questions and ideas: [r/openmoat](https://www.reddit.com/r/openmoat/). Bugs and false
positives: [OpenMoat issues](https://github.com/crocodile-labs/openmoat/issues/new/choose).
Found a way past OpenMoat? Please report it privately, as described in
[SECURITY.md](https://github.com/crocodile-labs/openmoat/blob/main/SECURITY.md).

Open source under MIT or Apache-2.0.
