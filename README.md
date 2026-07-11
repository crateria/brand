# Crateria brand kit

**Canonical source of truth** for Crateria visual identity assets.

If a laptop dies, clone this repo — do not rely on local `Downloads/`.

## Layout

```
marks/          Square transparent PNG masters + size ladder
  *.png         1024×1024 masters (crateria, trance, morphball, trance-plugins)
  *-{32..512}.png   Size ladder for packaging / desktop
  *-on-dark.jpg Preview composites on brand dark
heroes/         Marketing / OG sources (wide + scenic)
repo/           Ready-to-install 512 PNG + embedded SVG (+ org avatar)
```

## Install into product repos

| Product | Files to copy |
|---------|----------------|
| `trance` | `repo/trance.png` → `assets/icon.png`, `repo/trance.svg` → `assets/icon.svg` (also applet `resources/icon.png`) |
| `morphball` | `repo/morphball.png` / `.svg` → `assets/` |
| `trance-plugins` | `repo/trance-plugins.png` / `.svg` → `assets/` |
| `packages` | `repo/crateria.png` → `assets/icon.png` (site favicon) |
| Org profile | `repo/crateria-org-avatar.png` → GitHub org **Settings → Profile picture** (manual UI) |
| `.github` profile README | `repo/*.png` under `profile/icons/` |

Product repos keep **only** the installed icon files they ship. This repo keeps the full ladder and heroes.

## Brand notes

- Palette: neon orange on near-black; pixel / CRT glow language
- Prefer transparent PNG for UI; JPEG heroes for marketing only
- True hand-traced SVG is future work; current `.svg` files embed PNG for README compatibility

## License

Same as Crateria product repos (Apache-2.0) unless noted otherwise.
