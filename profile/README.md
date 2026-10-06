# Crocodile Labs 🐊

We build open-source security tools for developers who work with AI coding agents.

### [OpenMoat](https://github.com/crocodile-labs/openmoat)

OpenMoat checks every action an AI coding agent takes on your computer and stops the
dangerous ones before they run. It works with Claude Code, Codex and Cursor today, can
sandbox any other agent with `moat run`, and support for more agents is on the way. The
command is `moat`.

- One policy decides allow, ask or deny for every command, file access, web request and
  MCP call.
- The same policy configures each agent's operating-system sandbox.
- Every decision is kept in a local audit log that detects tampering.

Local, deterministic and open source (Apache-2.0 and MIT).
