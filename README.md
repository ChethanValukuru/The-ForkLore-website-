# ForkLore

A single-page marketing site for **ForkLore** — a structured Indian
meal-plan and nutrition system. The site turns a fitness goal into a
daily nutrition system: planned meals, controlled portions and clear,
verifiable numbers.

## What's here

| File | Purpose |
| --- | --- |
| `ForkLore.dc.html` | **Editable source.** The full site authored with the `<x-dc>` design-component runtime (`support.js`), hash-routed across Home, How It Works, Meal Plans, Nutrition, Our Story, FAQ and Get Started. |
| `ForkLore-offline.html` | **Self-contained build.** A single bundled HTML file with the runtime, fonts and images inlined — this is what gets deployed and shared. |
| `index.html` | Entry point. Redirects to `ForkLore-offline.html`, preserving the URL hash so deep links keep working. |
| `support.js` / `image-slot.js` | The design-component runtime and the drag-and-drop image placeholder element. |
| `forklore-image-prompts.md` / `forklore-home-image-prompts.md` | Art-direction briefs for the photography slots. |
| `screens/` | Reference screenshots. |

## Design system

- **Palette:** Bone `#F5F0EB`, Navy `#2F4156`, Slate blue `#567C8D`, Light blue `#C8D9E6`.
- **Type:** Fraunces (editorial serif headings) + Karla (sans body) + Caveat (handwritten annotations).
- **Motion:** section reveals and time-based `--p` morphs on the How It Works page; hand-drawn `data-draw` line accents throughout.

## Viewing it locally

It's static HTML — open `ForkLore-offline.html` in a browser, or serve the
folder:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Editing

Edit `ForkLore.dc.html` (the source), then mirror the change into
`ForkLore-offline.html` (the bundled build). See [`docs/BUILD.md`](docs/BUILD.md)
for how the two files relate.

## Deploy

Hosted on GitHub Pages from the repository root (`.nojekyll` disables
Jekyll processing). Live at
<https://chethanvalukuru.github.io/The-ForkLore-website-/>.
