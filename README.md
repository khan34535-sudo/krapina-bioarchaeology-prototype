# Krapina Cave · Bioarchaeological Evidence Archive

> ⚠ **Prototype · Demonstrator Only · Not for Research Citation**

An experimental interface exploring how archaeological, osteological, and material-culture evidence might be presented interactively — through satellite terrain, 3D specimen models, stratigraphic animation, and multi-proxy narratives.

**Asia Khan, Hon. BA (McMaster University)**
Behavioral UX Researcher & Design Anthropologist

---

## 🔗 Live Prototype

→ [View the interactive prototype](https://khan34535-sudo.github.io/krapina-bioarchaeology-prototype/)

*(If the link doesn't work, enable GitHub Pages in `Settings → Pages → main branch → / (root)`)*

---

## ⚠ Disclaimer

This is a **design prototype and demonstrator**. It is intended to show *how* archaeological information could be presented, not to serve as a primary research source.

- Site names and APA citations point to **real literature**
- Coordinates, artifact descriptions, and numerical indices are **illustrative examples**
- All 3D models and artifact images are **placeholders**
- **Do not cite this prototype in academic work** — consult original publications

---

## What This Demonstrates

- **Spatial context** — Real satellite imagery with 3D terrain, hosting site nodes as spatial anchors
- **3D specimen models** — Procedural Three.js models of Mousterian tools, hominin crania, fauna, and symbolic artifacts
- **Multi-proxy integration** — Lithics, morphology, dental anthropology, pathology, fauna, isotopes, and symbolic evidence side-by-side
- **Stratigraphic animation** — A playable sequence showing how repeated site-use cycles deposit archaeological layers over deep time
- **Readable citations** — Every panel surfaces its own APA 7th reference
- **Site-use cycle narrative** — Explorable *chaîne opératoire* from raw material procurement to discard

---

## What's Real vs. Placeholder

| Status | Item |
|---|---|
| ✅ Real | Site name & regional context (Krapina / Hušnjakovo) |
| ✅ Real | APA 7th citations to published literature |
| ✅ Real | Archaeological and osteological concepts |
| ✅ Real | Raw-material procurement geography |
| ⚠ Partial | Site coordinates (regional centroids) |
| ⚠ Partial | Layer count & dates in stratigraphy animation |
| ❌ Placeholder | All 3D specimen models |
| ❌ Placeholder | Artifact images & diagrams |
| ❌ Placeholder | Isotope values & mobility indices |
| ❌ Placeholder | Site-level descriptive text |

---

## About the 3D Models — All Placeholders

Every 3D object is a **procedurally generated placeholder** built from basic geometry inside the browser. None are photogrammetry scans, CT reconstructions, or museum-licensed models. They demonstrate **interface structure, taxonomy, and interaction** — not specific specimens.

---

## Important Notes

- **Not a citable source.** The APA references inside the interface point to the real papers — cite those instead.
- **Interpretations are simplified.** Debated areas (cannibalism hypothesis, eagle talon status, dental intervention) are presented as readable summaries, not full scholarly disagreement.
- **No aDNA at Krapina.** The bones are not suitable for genetic analysis — a deliberate structural choice.
- **Accessibility.** Colour encodes meaning; a production version should add pattern coding and screen-reader support.
- **Browser requirements.** Three.js + MapLibre GL + TailwindCSS (CDN). Requires a modern browser with WebGL. Geolocation will not work via `file://`.
- **External tiles.** Satellite and label tiles load live from Esri.
- **No warranty.** Provided as-is, for demonstration.

---

## Running Locally

**Option 1 — Open directly:**
Save as `index.html` and open in Chrome, Edge, Firefox, or Safari. Most features work; geolocation does not.

**Option 2 — Local server (recommended):**
```bash
python3 -m http.server 8000
# then open http://localhost:8000
