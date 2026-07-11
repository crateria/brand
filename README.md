<p align="center">
  <a href="https://github.com/crateria">
    <img src="headers/crateria-header.jpg" alt="Crateria" width="100%">
  </a>
</p>

# Crateria brand kit

Canonical visual assets for the Crateria organization.

## Public brand: header only

GitHub READMEs, the org profile, and the packages site use the **header banner**. There is no product icon set in this repository.

**Header source of truth:** `headers/crateria-header.jpg` (also `assets/crateria-header.jpg`).

Product repos keep a **copy** at `assets/crateria-header.jpg` so README relative paths work without depending on a cross-repo CDN.

## Header

`headers/crateria-header.jpg` (1280×240) — used on product READMEs and org pages.

- **Left:** Crateria C (oversized, cropped top/bottom)
- **Right:** rusted environment from the original scenic art
- One continuous frame (not two images spliced mid-banner)

![Crateria header](headers/crateria-header.jpg)

## Directory layout

```
headers/  README banner (crateria-header.jpg)
assets/   Same header copy for convenience
heroes/   Optional wide / scenic marketing stills (not used on GitHub READMEs)
```

## Installing the header into product repositories

| Target | Copy |
|--------|------|
| All product READMEs | `headers/crateria-header.jpg` → `assets/crateria-header.jpg` |
| [crateria/crateria](https://github.com/crateria/crateria) | → `assets/crateria-header.jpg` |
| [.github](https://github.com/crateria/.github) | → `crateria-header.jpg` (repo root + `profile/`) |

README pattern:

```html
<p align="center">
  <a href="https://github.com/crateria">
    <img src="assets/crateria-header.jpg" alt="Crateria" width="100%">
  </a>
</p>

# Product name
```

## Design notes

| Token | Value |
|-------|--------|
| Accent | `#ff8541` |
| Background | `#0b0d0f` – `#121216` |

## License

[Apache-2.0](LICENSE) · Copyright 2026 Crateria
