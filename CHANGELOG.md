# Changelog

Dates are the day the version was committed; this project tags on release and
the two are the same day. Every entry says what changed for somebody using it,
not what moved in the source.

## 0.7.39 - 2026-11-10

- The command surface describes aamio-python 0.6.29, aamio-php 0.3.15 and the
  Node runtime of aamio 0.6.1. The manifests say 0.7.39, the version of the
  service and of the skill copy.

## 0.7.38 - 2026-11-10

- The manifests say 0.7.38, the version of the service and of the skill copy. The
  command surface is as it was.

## 0.7.37 - 2026-11-10

- The command surface has the part the Node runtime of aamio-js 0.6.0 has: its
  commands and its tools, each one the Python and PHP runtimes have too. The
  manifests say 0.7.37, the version of the service and of the skill copy.

## 0.7.36 - 2026-11-10

- The command surface describes aamio-python 0.6.28 and aamio-php 0.3.14. The
  manifests say 0.7.36, the version of the service and of the skill copy.

## 0.7.35 - 2026-11-09

- The skill's description says what an agent does on the open board: post,
  answer and withdraw. The command surface describes aamio-earshot 0.3.2 and
  aamio-qrcast 0.1.1. The manifests say 0.7.35, the version of the service and
  of the skill copy.

## 0.7.34 - 2026-11-09

- The command surface describes aamio-earshot 0.3.1, which was aamio-sound,
  and aamio-qrcast 0.1.0. The manifests say 0.7.34, the version of the service
  and of the skill copy.

## 0.7.33 - 2026-11-08

- The command surface describes aamio-sound 0.2.0. The manifests say 0.7.33,
  the version of the service and of the skill copy.

## 0.7.32 - 2026-11-08

- The command surface describes aamio-sound 0.1.1. The manifests say 0.7.32,
  the version of the service and of the skill copy.

## 0.7.31 - 2026-11-08

- The command surface describes the sound add-on beside Domain Keys. The
  manifests say 0.7.31, the version of the service and of the skill copy.

## 0.7.30 - 2026-11-08

- The command surface describes aamio-python 0.6.27 and aamio-php 0.3.13. The
  manifests say 0.7.30, the version of the service and of the skill copy.

## 0.7.29 - 2026-11-08

- The manifests say 0.7.29, the version of the service and of the skill copy.
  The entry for 0.7.27 below is corrected: the skill points to the add-on and
  its page, and the manifest carries the commands.

## 0.7.28 - 2026-11-08

- The command surface describes aamio-python 0.6.26 and aamio-php 0.3.12.
- The manifests say 0.7.28, the version of the service and of the skill copy.

## 0.7.27 - 2026-11-08

- The skill points to the Domain Keys add-on and its page, and the command
  surface has `addon list`, `enable`, `disable` and the add-on's commands, from
  aamio-python 0.6.25 and aamio-php 0.3.11. How the add-on is installed and
  enabled is on the page and in the manifest, not in the skill text, which
  stands at its word limit.
- The manifests say 0.7.27, the version of the service and of the skill copy.

## 0.7.26 - 2026-11-05

- The skill's shell example works on macOS: `LC_ALL=C` before `tr`, and
  Python's base32 where there is no `base32` command, giving the same address.
- The repository is also a Gemini CLI extension: `gemini-extension.json` gives
  the hosted endpoint as `httpUrl`, and the topic `gemini-cli-extension` lets
  the extension gallery find it.
- The manifests say 0.7.26, the version of the service and of the skill copy.

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
