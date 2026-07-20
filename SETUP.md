# Setup

Delete this file once you've done the four things on it.

## 1. Drop the files in

Extract into a clone of `ImTani/imTani`. The tree must look exactly like this —
`.github/workflows/` is not negotiable, Actions ignores any other path.

```
imTani/
├── README.md
├── header.svg
├── .github/workflows/status.yml
└── rooms/
```

```bash
git add -A && git commit -m "feat: rebuild profile" && git push
```

## 2. Give the Action write access

Settings → Actions → General → Workflow permissions → **Read and write permissions**.

The workflow declares `contents: write`, but the repo-level setting overrides it and
new repos default to read-only. This is the step everyone misses.

## 3. Run it once, now

Actions → **Update status block** → Run workflow. Don't wait six hours to find out
it's broken. It should rewrite the block between the `STATUS` markers in README.md
and push a commit as `github-actions[bot]`.

Live values as of packaging, so you know what "working" looks like:

| Service | Uptime | Response |
|---|---|---|
| API Gateway | 100% | 109 ms |
| Aptos Relayer | 99.84% | 311 ms |
| Avalanche Bundler | 100% | 783 ms |

## 4. Fill the four gaps

- **`header.svg`** — mine is geometry. You animate. Redraw it. The technique is proven:
  `<style>` with `@keyframes` inside the SVG, embedded as a plain `<img>`. No scripts,
  no `foreignObject`. Respects `prefers-reduced-motion` and inverts for dark mode.
- **The Medium link** in README.md is a guess at your profile URL. Point it at the
  actual InSight article.
- **`rooms/hall.md`** — my handwriting. Replace it.
- **`rooms/study.md`** — music, drawing, the poems. Write this one *second*, not last.

## Pins (set manually on your profile)

`clipd` · `SmoothSend/smoothsend-sdk` · `godot-time-rewind-2d` ·
`godot-property-selection-window` · `FinWise` · and a **game** for the sixth.

## Bio field (160 chars, separate from this README)

```
ML @ AiHello · co-founder @ SmoothSend · Rust, TypeScript, Godot · I build small tools and give them away.
```

## Still open elsewhere

- `@smoothsend/mcp` still has no `repository`, `bugs` or `homepage`. Needs its own patch publish.
- Keep `tanidev69@gmail.com` attached to your GitHub account — 222 clipd commits and 63
  SDK commits are authored under it. Set it private; don't remove it.
- Two testnet services are still showing red on status.smoothsend.xyz.
