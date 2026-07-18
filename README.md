# atelier-nyaarium

Umbrella Claude Code plugin marketplace for Nyaarium's plugins.

## Install

```
claude plugin marketplace add atelier-nyaarium/claude-marketplace

claude plugin install switchboard@atelier-nyaarium

claude plugin install nyaaskills@atelier-nyaarium
```

Autoupdate is a settings flag. One-line jq version:

```
tmp=$(mktemp) && jq '. * {extraKnownMarketplaces: {"atelier-nyaarium": {autoUpdate: true}}}' ~/.claude/settings.json > "$tmp" && mv "$tmp" ~/.claude/settings.json
```

## Plugins

- **switchboard** - Cross-team communication, devcontainer orchestration, evie-bot bridge. Source: [atelier-nyaarium/switchboard](https://github.com/atelier-nyaarium/switchboard)
- **nyaaskills** - Shared agents and skills for testability, quality, code analysis, debugging, and team collaboration. Source: [atelier-nyaarium/nyaaskills](https://github.com/atelier-nyaarium/nyaaskills)
