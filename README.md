# Crateria brand kit

<p align="center">
  <img src="marks/crateria.png" width="128" height="128" alt="Crateria">
</p>

<p align="center">
  <strong>Canonical source of truth</strong> for Crateria visual identity.
</p>

If a machine is wiped, clone this repo — do not rely on local `Downloads/`.

```bash
git clone https://github.com/crateria/brand.git
```

## Marks

| Mark | Use |
|------|-----|
| ![c](marks/crateria-64.png) **crateria** | Org avatar, packages site, umbrella brand |
| ![t](marks/trance-64.png) **trance** | Screensaver core (daemon / CLI / TUI / applet) |
| ![p](marks/trance-plugins-64.png) **trance-plugins** | Effect suite |
| ![m](marks/morphball-64.png) **morphball** | Archive manager |

## Layout

```
marks/     Square transparent PNG masters (1024) + size ladder (32–512) + on-dark previews
heroes/    Marketing / OG sources (wide + scenic)
repo/      Ready-to-install 512 PNG + embedded SVG (+ org-avatar.png)
```

## Install into product repos

| Product | Copy from `repo/` |
|---------|-------------------|
| [trance](https://github.com/crateria/trance) | `trance.png` → `assets/icon.png`, `trance.svg` → `assets/icon.svg` (+ applet `resources/icon.png`) |
| [morphball](https://github.com/crateria/morphball) | `morphball.png` / `.svg` → `assets/` |
| [trance-plugins](https://github.com/crateria/trance-plugins) | `trance-plugins.png` / `.svg` → `assets/` |
| [packages](https://github.com/crateria/packages) | `crateria.png` → `assets/icon.png` |
| Org profile | `crateria-org-avatar.png` → GitHub **Settings → Profile picture** (manual) |
| [.github](https://github.com/crateria/.github) | icons under `profile/icons/` |

Product repos keep **only** the shipped icons. This repo keeps masters, ladders, and heroes.

## Brand notes

- Palette: neon orange (`#ff8541`) on near-black (`#0b0d0f`–`#121216`)
- Language: pixel / CRT glow, Chozo-adjacent geometry
- Prefer transparent PNG for UI; JPEG heroes for marketing only
- Current `.svg` files embed PNG for README compatibility; hand-traced SVG is future work

## License

[Apache-2.0](LICENSE) · Copyright 2026 [Crateria](https://github.com/crateria)
