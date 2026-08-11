# sha3bolly

A Claude Code plugin that makes Claude explain things **like you're a junior
engineer** instead of a scientist:

- Plain language, short sentences — no walls of text.
- Always gives a concrete example (real code / real request-response).
- Draws a flowchart whenever a process has multiple chained steps.

## For teammates — install in 2 commands

This plugin is published as a public marketplace. In Claude Code, run:

```
/plugin marketplace add abueldahabh/sha3bolly
/plugin install sha3bolly@sha3bolly
```

To get a newer version later, re-run the first command to refresh the
marketplace, then reinstall.

## What's inside

```
sha3bolly/
├── .claude-plugin/
│   ├── plugin.json         # plugin manifest
│   └── marketplace.json    # lets it install as a local marketplace
├── skills/
│   └── explain-like-junior/
│       └── SKILL.md        # the actual behavior
└── README.md
```

## Install (from a local folder)

1. Add the marketplace:
   ```
   /plugin marketplace add /path/to/sha3bolly
   ```
2. Install the plugin:
   ```
   /plugin install sha3bolly@sha3bolly
   ```

Or add this to your `.claude/settings.json` and run `/reload-plugins`:

```json
{
  "extraKnownMarketplaces": {
    "sha3bolly": {
      "source": { "source": "directory", "path": "/path/to/sha3bolly" }
    }
  },
  "enabledPlugins": {
    "sha3bolly@sha3bolly": true
  }
}
```

## Install (from git)

```
/plugin marketplace add abueldahabh/sha3bolly
/plugin install sha3bolly@sha3bolly
```
