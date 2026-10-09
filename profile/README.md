# Crocodile Labs 🐊

We build open-source security tools for developers who work with AI coding agents.

### [OpenMoat](https://github.com/crocodile-labs/openmoat)

OpenMoat checks what AI coding agents do on your computer and stops the dangerous
actions before they run. It works with Claude Code, Codex and Cursor, and `moat run`
sandboxes other agents. The command is `moat`.

- One policy decides allow, ask or deny for each command, file access, web request and
  MCP call the agents report through their hooks.
- The same policy configures each agent's operating-system sandbox.
- Every decision is kept in a local audit log that detects tampering.

Local, deterministic and open source (Apache-2.0 and MIT). Website: [openmoat.dev](https://openmoat.dev)
