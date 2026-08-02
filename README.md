# inspercidades.r-universe.dev

Package registry for the [Insper Cidades](https://github.com/inspercidades)
r-universe: <https://inspercidades.r-universe.dev>

## Installing

```r
install.packages(
  "insperplot",
  repos = c("https://inspercidades.r-universe.dev", "https://cloud.r-project.org")
)
```

## Adding a package

Append an entry to `packages.json`:

```json
{
  "package": "<name>",
  "url": "https://github.com/inspercidades/<repo>"
}
```

Optional keys: `branch` (defaults to the repo's default branch) and `subdir`
(when the package is not at the repo root).

r-universe builds from the **tip of the tracked branch**, not from git tags. A
new version is published when `Version:` in that package's `DESCRIPTION`
changes; tagging a release does not by itself trigger a rebuild.

### Queued

- `inspercidados` — next in line after `insperplot`.
- `utilscidados` — too early; revisit once the API settles.
