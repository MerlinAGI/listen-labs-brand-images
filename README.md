# Listen Labs — Brand Image Library

Brand imagery for the Listen Labs slides skill: researcher portraits, environment
scenes, signature imagery, and client logos, organized by industry.

## Usage (jsDelivr CDN)

Reference any image by prepending the CDN base to its `path` from `manifest.json`:

```
https://cdn.jsdelivr.net/gh/MerlinAGI/listen-labs-brand-images@main/<path>
```

Pin a version tag (e.g. `@v1`) in production decks so re-organizing this repo
never breaks a shipped deck. Bump the tag deliberately.

## manifest.json

Machine-readable index of every image: `path`, `category` (industry), `sub`,
`kind` (researcher / environment / scene / logo), `aspect` (1x1 / 16x9 / …).
The slides skill reads this to pick images without filesystem access — the key
to running the skill on claude.ai and Desktop, not just the terminal.

## Structure

`_<industry>/_researchers/`, `_<industry>/_environments/`, `_signature/`, `_logos/`.
