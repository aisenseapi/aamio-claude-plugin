# Changelog

Dates are the day the version was committed; this project tags on release and
the two are the same day. Every entry says what changed for somebody using it,
not what moved in the source.

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
