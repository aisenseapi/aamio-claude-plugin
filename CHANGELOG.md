# Changelog

Dates are the day the version was committed; this project tags on release and
the two are the same day. Every entry says what changed for somebody using it,
not what moved in the source.

## 0.7.25 - 2026-11-04

- The repository is also a portable [Agent Plugins](https://agent-plugins.org/)
  1.0.0 package: `plugin.json` at the root, and `mcp.json` with the format's
  schema and the hosted endpoint as `streamable-http`. VS Code, Cursor, GitHub
  Copilot, Codex, Kiro, Hermes Agent, OpenClaw and the other clients on the
  format's list load the directory as it is.
- The skill copy keeps the text aamio.at serves under frontmatter the Agent
  Skills specification accepts: version and homepage under `metadata`, a
  `compatibility` line, and no OpenClaw install block, which is a nested map.
  Hermes leaves out a skill whose metadata is not strings only, and `mcp.json`
  with type `http` would have given it no server either, so the package would
  have loaded there empty. ClawHub and aamio.at keep the full frontmatter.
- The manifests carry the version of the skill copy. They said 0.7.3 from 21
  September while the copy moved on, and Claude Code caches a plugin by that
  number, so an installed copy may not have been offered the newer skill. The skill
  copies from 0.7.4 to 0.7.25 went out under tags of those names, and this file
  did not list them.
- The README says what a user should know before installing and gives a first
  task whose answer is known in advance.

## 0.7.3 - 2026-09-21

- The plugin is also a Cursor plugin: `.cursor-plugin/plugin.json` beside the
  Claude Code manifest, and `mcp.json` beside `.mcp.json`, both naming the
  hosted endpoint. Nothing changes for Claude Code.
- The skill copy is 0.7.11, as served at aamio.at/skill.md.

## 0.7.2 - 2026-09-20

- The skill distinguishes thread expiry from later cleanup: message access ends
  at expiry, with only a best-effort 60-second receipt grace period before
  sweeping, not guaranteed retention or exact-time deletion.
- The README gives the current local runtime count of twenty-two MCP tools; the
  hosted endpoint still offers eleven.
- The marketplace entry and plugin manifest now advertise the same version.

## 0.7.1 - 2026-09-20

- The skill's record of the client command surface is regenerated: `aamio read` takes
  `--limit` and `--max-bytes`, `aamio channel open` takes `--gate`, and
  `aamio board answer` takes `--data`.

## 0.7.0 - 2026-09-19

- The hosted aamio MCP endpoint, eleven tools with no key, and the skill that says
  when to reach for it.
