# HammerTime Skills

Shared [Claude Code](https://claude.com/claude-code) skills for the HammerTime bot and
website projects.

## Skills

- **crowdin-review** — Reviews Crowdin strings that are translated but not yet approved,
  checking for translation accuracy, preserved markup/placeholders, and non-empty content
  before a human approves them.

## Installation

This repository is a Claude Code plugin. Add it as a marketplace, then install the plugin:

```
/plugin marketplace add WentTheFox/HammerTimeSkills
/plugin install hammertime-skills
```

Restart Claude Code (or start a new session) after installing so the skills are picked up.

## Usage

Once installed, invoke a skill by its slash command, e.g.:

```
/crowdin-review
/crowdin-review de
```

See each skill's `SKILL.md` for details on what it does and any setup it requires (for
example, `crowdin-review` needs a Crowdin MCP server configured with the right tool sets and
a Personal Access Token with matching scopes — see that file for specifics).
