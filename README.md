# amlmarketplaces/anthropic

Claude Code marketplace federating all `@amlplugins/anthropic-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-anthropic": {
      "source": { "source": "github", "repo": "amlmarketplaces/anthropic" }
    }
  },
  "enabledPlugins": {
      "anthropic-batches@aml-anthropic": true,
      "anthropic-bedrock@aml-anthropic": true,
      "anthropic-files@aml-anthropic": true,
      "anthropic-messages@aml-anthropic": true,
      "anthropic-prompt-caching@aml-anthropic": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/anthropic`, cached under `~/.claude/plugins/cache/aml-anthropic/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (7 total)

- `anthropic-batches` — [@amlplugins/anthropic-batches](https://github.com/amlplugins/anthropic-batches)
- `anthropic-bedrock` — [@amlplugins/anthropic-bedrock](https://github.com/amlplugins/anthropic-bedrock)
- `anthropic-files` — [@amlplugins/anthropic-files](https://github.com/amlplugins/anthropic-files)
- `anthropic-messages` — [@amlplugins/anthropic-messages](https://github.com/amlplugins/anthropic-messages)
- `anthropic-prompt-caching` — [@amlplugins/anthropic-prompt-caching](https://github.com/amlplugins/anthropic-prompt-caching)
- `anthropic-tool-use` — [@amlplugins/anthropic-tool-use](https://github.com/amlplugins/anthropic-tool-use)
- `anthropic-vertex` — [@amlplugins/anthropic-vertex](https://github.com/amlplugins/anthropic-vertex)

## Related

- npm packages: `@amlplugins/anthropic-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
