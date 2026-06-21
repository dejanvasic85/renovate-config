# renovate-config

Shared [Renovate](https://docs.renovatebot.com/) configuration presets used across personal projects.

## Presets

- **`default.json`** – Base config applied to all repositories. Enables automerge, semantic commits, dependency grouping, and a 1-day minimum release age.
- **`nextjs.json`** – Extends the default config with Next.js-specific rules, including grouped Next.js monorepo updates and an ESLint version pin.

## Usage

Reference a preset from any repository's `renovate.json`:

```json
{
  "extends": ["github>dejanvasic85/renovate-config"]
}
```

Or use the Next.js preset:

```json
{
  "extends": ["github>dejanvasic85/renovate-config:nextjs"]
}
```
