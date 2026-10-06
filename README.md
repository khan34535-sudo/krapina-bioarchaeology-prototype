<!DOCTYPE html>
<html lang="en" class="dark">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>README · Krapina Cave Bioarchaeological Evidence Archive</title>
<script src="https://cdn.tailwindcss.com"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/js/all.min.js"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Merriweather:wght@400;700;900&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<script>
tailwind.config = {
  darkMode: 'class',
  theme: {
    extend: {
      colors: {
        terracotta: { 600: '#C85A32', 700: '#A0431E', 800: '#7E3314' },
        forest: { 600: '#2E5A44', 700: '#204131', 900: '#11231A' },
        parchment: { 100: '#FDFBF7', 200: '#F4EFE6', 800: '#2D2823', 900: '#1C1917' },
        gold: { 500: '#D4AF37', 600: '#AA8C2C' }
      },
      fontFamily: {
        sans: ['Inter', 'sans-serif'],
        serif: ['Merriweather', 'serif'],
        mono: ['JetBrains Mono', 'monospace']
      }
    }
  }
}
</script>
<style>
  body { font-family: 'Inter', sans-serif; background-color: #0b1711; color: #F4EFE6; line-height: 1.65; }
  .glass-panel { background: rgba(22, 38, 29, 0.88); backdrop-filter: blur(14px); border: 1px solid rgba(212, 175, 55, 0.25); }
  .glass-card { background: rgba(35, 52, 42, 0.8); backdrop-filter: blur(10px); border: 1px solid rgba(200, 90, 50, 0.3); }
  .prose-block p { margin-bottom: 0.9rem; }
  .prose-block ul { list-style: none; padding-left: 0; margin-bottom: 0.9rem; }
  .prose-block ul li { position: relative; padding-left: 1.5rem; margin-bottom: 0.5rem; }
  .prose-block ul li::before { content: "▸"; position: absolute; left: 0; color: #D4AF37; font-weight: 700; }
  ::-webkit-scrollbar { width: 8px; }
  ::-webkit-scrollbar-track { background: #0b1711; }
  ::-webkit-scrollbar-thumb { background: #C85A32; border-radius: 4px; }
  .pill { display: inline-flex; align-items: center; gap: 6px; padding: 3px 10px; border-radius: 999px; font-size: 11px; font-weight: 600; letter-spacing: 0.03em; }
  .pill-warn { background: rgba(200, 90, 50, 0.15); color: #E8A07A; border: 1px solid rgba(200, 90, 50, 0.4); }
  .pill-info { background: rgba(212, 175, 55, 0.12); color: #E8CE82; border: 1px solid rgba(212, 175, 55, 0.4); }
  .pill-ok { background: rgba(46, 90, 68, 0.3); color: #8FCFA8; border: 1px solid rgba(46, 90, 68, 0.6); }
  .pill-lock { background: rgba(126, 51, 20, 0.25); color: #E0A48A; border: 1px solid rgba(126, 51, 20, 0.5); }
  a.link { color: #D4AF37; text-decoration: none; border-bottom: 1px dotted rgba(212, 175, 55, 0.5); }
  a.link:hover { border-bottom-style: solid; color: #FDFBF7; }
  .divider { height: 1px; background: linear-gradient(90deg, transparent, rgba(212, 175, 55, 0.35), transparent); margin: 2.5rem 0; }
  .callout-warn {
    background: linear-gradient(135deg, rgba(200, 90, 50, 0.18), rgba(126, 51, 20, 0.12));
    border: 1px solid rgba(200, 90, 50, 0.55);
    border-left: 4px solid #C85A32;
  }
  .callout-info {
    background: linear-gradient(135deg, rgba(212, 175, 55, 0.12), rgba(170, 140, 44, 0.08));
    border: 1px solid rgba(212, 175, 55, 0.45);
    border-left: 4px solid #D4AF37;
  }
  .callout-lock {
    background: linear-gradient(135deg, rgba(126, 51, 20, 0.25), rgba(60, 25, 10, 0.2));
    border: 1px solid rgba(212, 175, 55, 0.5);
    border-left: 4px solid #7E3314;
  }
  .callout-ethics {
    background: linear-gradient(135deg, rgba(46, 90, 68, 0.25), rgba(17, 35, 26, 0.3));
    border: 1px solid rgba(46, 90, 68, 0.6);
    border-left: 4px solid #2E5A44;
  }
  table.status-table { width: 100%; border-collapse: collapse; font-size: 13px; }
  table.status-table th { text-align: left; padding: 10px 12px; background: rgba(11, 23, 17, 0.7); color: #D4AF37; font-family: 'Merriweather', serif; font-weight: 700; font-size: 12px; letter-spacing: 0.05em; text-transform: uppercase; border-bottom: 1px solid rgba(212, 175, 55, 0.3); }
  table.status-table td { padding: 10px 12px; border-bottom: 1px solid rgba(212, 175, 55, 0.1); color: rgba(244, 239, 230, 0.9); }
  table.status-table tr:last-child td { border-bottom: none; }
  table.status-table tr:hover td { background: rgba(212, 175, 55, 0.04); }
  code, pre { font-family: 'JetBrains Mono', monospace; }
  code { background: rgba(11, 23, 17, 0.8); color: #9bc2da; padding: 2px 6px; border-radius: 4px; font-size: 12px; }
  pre { background: #0a141d; color: #9bc2da; border-radius: 8px; padding: 14px; font-size: 12px; overflow-x: auto; border: 1px solid rgba(212, 175, 55, 0.2); }
</style>
</head>
<body class="min-h-screen">

<!-- TOP BANNER -->
<div class="bg-gradient-to-r from-terracotta-700 via-terracotta-600 to-gold-600 text-parchment-100 text-xs py-2 px-4 text-center font-medium border-b border-gold-500/40 shadow-md flex flex-wrap items-center justify-center gap-2">
  <span class="bg-gold-500 text-forest-900 px-2 py-0.5 rounded text-[10px] font-bold tracking-wider uppercase">◈ Prototype · README</span>
  <span class="hidden md:inline text-gold-500">◆</span>
  <span class="font-medium tracking-wide">Asia Khan, Hon. BA (McMaster University)</span>
  <span class="hidden md:inline text-gold-500">◆</span>
  <span class="text-gold-500 italic">Behavioral UX Researcher and Design Anthropologist</span>
</div>

<div class="max-w-4xl mx-auto px-5 md:px-8 py-10">

  <!-- TITLE -->
  <header class="mb-8">
    <h1 class="font-serif font-black text-3xl md:text-4xl text-parchment-100 leading-tight mb-3">
      Krapina Cave · Bioarchaeological Evidence Archive
    </h1>
    <p class="text-sm text-parchment-200/80 font-serif italic mb-4">
      An experimental interface exploring how archaeological, osteological, and material-culture evidence might be presented interactively — through satellite terrain, 3D specimen models, stratigraphic animation, and multi-proxy narratives.
    </p>
    <div class="flex flex-wrap gap-2">
      <span class="pill pill-warn"><i class="fa-solid fa-flask"></i> Prototype · Demonstrator Only</span>
      <span class="pill pill-info"><i class="fa-solid fa-cube"></i> 3D Placeholders</span>
      <span class="pill pill-ok"><i class="fa-solid fa-book-open"></i> Educational</span>
      <span class="pill pill-lock"><i class="fa-solid fa-lock"></i> All Rights Reserved</span>
    </div>
  </header>

  <!-- LIVE PROTOTYPE -->
  <section class="glass-panel rounded-2xl p-5 md:p-6 mb-8">
    <h2 class="font-serif font-bold text-lg text-gold-500 mb-3 flex items-center gap-2">
      <i class="fa-solid fa-link"></i> Live Prototype
    </h2>
    <p class="text-sm text-parchment-200/90 mb-3">
      → <a class="link" href="#" target="_blank">View the interactive prototype</a>
    </p>
    <p class="text-xs text-parchment-200/60 italic mb-0">
      (If the link doesn't work, enable GitHub Pages in <code>Settings → Pages → main branch → / (root)</code>)
    </p>
  </section>

  <!-- CRITICAL DISCLAIMER -->
  <section class="callout-warn rounded-xl p-5 md:p-6 mb-8">
    <div class="flex items-start gap-3">
      <i class="fa-solid fa-triangle-exclamation text-terracotta-600 text-xl mt-0.5"></i>
      <div>
        <h2 class="font-serif font-bold text-lg text-parchment-100 mb-3">Disclaimer</h2>
        <div class="text-sm text-parchment-200/95 prose-block">
          <p>This is a <b>design prototype and demonstrator</b>. It is intended to show <i>how</i> archaeological information could be presented, not to serve as a primary research source.</p>
          <ul class="mb-0">
            <li>Site names and APA citations point to <b>real literature</b></li>
            <li>Coordinates, artifact descriptions, and numerical indices are <b>illustrative examples</b></li>
            <li>All 3D models and artifact images are <b>placeholders</b></li>
            <li><b>Do not cite this prototype in academic work</b> — consult original publications</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- WHAT THIS DEMONSTRATES -->
  <section class="glass-panel rounded-2xl p-5 md:p-7 mb-8">
    <h2 class="font-serif font-bold text-xl text-gold-500 mb-4 flex items-center gap-2">
      <i class="fa-solid fa-bullseye"></i> What This Demonstrates
    </h2>
    <div class="text-sm text-parchment-200/90 prose-block">
      <ul class="mb-0">
        <li><b>Spatial context</b> — Real satellite imagery with 3D terrain, hosting site nodes as spatial anchors</li>
        <li><b>3D specimen models</b> — Procedural Three.js models of Mousterian tools, hominin crania, fauna, and symbolic artifacts</li>
        <li><b>Multi-proxy integration</b> — Lithics, morphology, dental anthropology, pathology, fauna, isotopes, and symbolic evidence side-by-side</li>
        <li><b>Stratigraphic animation</b> — A playable sequence showing how repeated site-use cycles deposit archaeological layers over deep time</li>
        <li><b>Readable citations</b> — Every panel surfaces its own APA 7th reference</li>
        <li><b>Site-use cycle narrative</b> — Explorable chaîne opératoire from raw material procurement to discard</li>
      </ul>
    </div>
  </section>

  <!-- WHAT'S REAL VS PLACEHOLDER -->
  <section class="glass-panel rounded-2xl p-5 md:p-7 mb-8">
    <h2 class="font-serif font-bold text-xl text-gold-500 mb-4 flex items-center gap-2">
      <i class="fa-solid fa-scale-balanced"></i> What's Real vs. Placeholder
    </h2>
    <div class="overflow-x-auto rounded-lg border border-gold-500/20">
      <table class="status-table">
        <thead>
          <tr><th style="width: 110px;">Status</th><th>Item</th></tr>
        </thead>
        <tbody>
          <tr><td><span class="text-emerald-400">✅ Real</span></td><td>Site name &amp; regional context (Krapina / Hušnjakovo)</td></tr>
          <tr><td><span class="text-emerald-400">✅ Real</span></td><td>APA 7th citations to published literature</td></tr>
          <tr><td><span class="text-emerald-400">✅ Real</span></td><td>Archaeological and osteological concepts (Mousterian, taurodontism, fibrous dysplasia, etc.)</td></tr>
          <tr><td><span class="text-emerald-400">✅ Real</span></td><td>Raw-material procurement geography (local flint, imported stone sources)</td></tr>
          <tr><td><span class="text-amber-400">⚠ Partial</span></td><td>Site coordinates (regional centroids; excavation sub-grids simplified)</td></tr>
          <tr><td><span class="text-amber-400">⚠ Partial</span></td><td>Layer count &amp; dates in stratigraphy animation (illustrative, not exact published sequence)</td></tr>
          <tr><td><span class="text-red-400">❌ Placeholder</span></td><td>All 3D specimen models (procedural Three.js primitives)</td></tr>
          <tr><td><span class="text-red-400">❌ Placeholder</span></td><td>Artifact images &amp; diagrams</td></tr>
          <tr><td><span class="text-red-400">❌ Placeholder</span></td><td>Isotope values &amp; mobility indices</td></tr>
          <tr><td><span class="text-red-400">❌ Placeholder</span></td><td>Site-level descriptive text (summarised from real sources, but simplified)</td></tr>
        </tbody>
      </table>
    </div>
  </section>

  <!-- PLACEHOLDER NOTICE -->
  <section class="callout-info rounded-xl p-5 md:p-6 mb-8">
    <div class="flex items-start gap-3">
      <i class="fa-solid fa-cube text-gold-500 text-xl mt-0.5"></i>
      <div>
        <h2 class="font-serif font-bold text-lg text-parchment-100 mb-2">About the 3D models — all placeholders</h2>
        <div class="text-sm text-parchment-200/95 prose-block">
          <p>Every 3D object is a <b>procedurally generated placeholder</b> built from basic geometry inside the browser. None are photogrammetry scans, CT reconstructions, or museum-licensed models.</p>
          <p class="mb-0">They demonstrate <b>interface structure, taxonomy, and interaction</b> — not specific specimens. A production version would replace each placeholder with licensed scans (MorphoSource, Smithsonian 3D, NESPOS) via a GLTF loader.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- IMPORTANT NOTES -->
  <section class="glass-panel rounded-2xl p-5 md:p-7 mb-8">
    <h2 class="font-serif font-bold text-xl text-gold-500 mb-4 flex items-center gap-2">
      <i class="fa-solid fa-circle-info"></i> Important Notes
    </h2>
    <div class="text-sm text-parchment-200/90 prose-block">
      <p><b>Not a citable source.</b> Do not reference this prototype in academic work. The APA references inside the interface point to the real papers — cite those instead.</p>
      <p><b>Interpretations are simplified.</b> Several areas of Krapina research are actively debated (the cannibalism hypothesis, the status of eagle talons as ornament, the nature of the dental intervention). This prototype presents readable summaries, not the full scholarly disagreement.</p>
      <p><b>No aDNA at Krapina.</b> The bones are not suitable for genetic analysis. This project therefore has no genomics tab — a deliberate structural choice, not an oversight.</p>
      <p><b>Accessibility.</b> Colour encodes meaning (hominin orange, lithic blue, fauna green). Colour-blind users may benefit from accompanying labels and legends; a production version should add pattern coding and screen-reader support.</p>
      <p><b>Browser requirements.</b> Uses <i>Three.js</i> (r128), <i>MapLibre GL JS</i>, and <i>TailwindCSS</i> (CDN). Requires a modern browser with WebGL. Geolocation will not work when the file is opened via <code>file://</code> — host it locally or online.</p>
      <p><b>External tiles.</b> Satellite and label raster tiles load live from Esri. If their service rate-limits or changes, labels may disappear. A toggle button in the GIS tab can hide them.</p>
      <p class="mb-0"><b>No warranty.</b> Provided as-is, for demonstration. Not audited for factual accuracy, scholarly completeness, or technical robustness.</p>
    </div>
  </section>

  <!-- HOW TO RUN -->
  <section class="glass-panel rounded-2xl p-5 md:p-7 mb-8">
    <h2 class="font-serif font-bold text-xl text-gold-500 mb-4 flex items-center gap-2">
      <i class="fa-solid fa-terminal"></i> Running Locally
    </h2>
    <div class="text-sm text-parchment-200/90 prose-block">
      <p><b>Option 1 — open directly:</b> save the file as <code>index.html</code> and open it in Chrome, Edge, Firefox, or Safari. Most features work; geolocation does not.</p>
      <p><b>Option 2 — local server (recommended):</b></p>
      <pre>python3 -m http.server 8000
# then open http://localhost:8000</pre>
      <p class="mb-0"><b>Option 3 — GitHub Pages:</b> push to a repo, enable Pages on the <code>main</code> branch, and it will be served as a live site. Note that GitHub does not render HTML files in the repository view — it shows source code.</p>
    </div>
  </section>

  <!-- ETHICS -->
  <section class="callout-ethics rounded-xl p-5 md:p-6 mb-8">
    <div class="flex items-start gap-3">
      <i class="fa-solid fa-hands-holding-heart text-emerald-400 text-xl mt-0.5"></i>
      <div>
        <h2 class="font-serif font-bold text-lg text-parchment-100 mb-2">Ethics &amp; Heritage Context</h2>
        <div class="text-sm text-parchment-200/95 prose-block">
          <p>Krapina is a site of major scientific and cultural significance. The hominin remains excavated there are among the largest Neanderthal skeletal collections in the world, and their interpretation has shaped how Neanderthals are understood in both academic and public contexts.</p>
          <p>Presentation of such material in digital form carries responsibility — accuracy in representation, transparency about what is reconstructed versus observed, and acknowledgement that these are the remains of real people, not abstractions.</p>
          <p class="mb-0">This prototype is a <b>technical demonstration only</b>. Any real deployment of a public-facing resource on Krapina or comparable sites should involve consultation with the institutions that curate the collections and the descendant and local communities connected to the landscape.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- TECH STACK -->
  <section class="glass-panel rounded-2xl p-5 md:p-7 mb-8">
    <h2 class="font-serif font-bold text-xl text-gold-500 mb-4 flex items-center gap-2">
      <i class="fa-solid fa-code"></i> Tech Stack
    </h2>
    <div class="text-sm text-parchment-200/90 prose-block">
      <ul class="mb-0">
        <li><b>MapLibre GL JS</b> — satellite + terrain rendering</li>
        <li><b>Esri World Imagery</b> — free public satellite tiles</li>
        <li><b>Esri World Boundaries and Places</b> — label layer</li>
        <li><b>AWS Terrain DEM</b> — elevation tiles</li>
        <li><b>Three.js r128</b> — 3D specimen models &amp; stratigraphic animation</li>
        <li><b>Tailwind CSS</b> — layout &amp; styling</li>
        <li><b>Google Fonts</b> — Merriweather + Inter + JetBrains Mono</li>
        <li><b>Font Awesome 6</b> — iconography</li>
      </ul>
    </div>
  </section>

  <!-- CREDITS -->
  <section class="glass-panel rounded-2xl p-5 md:p-7 mb-8">
    <h2 class="font-serif font-bold text-xl text-gold-500 mb-4 flex items-center gap-2">
      <i class="fa-solid fa-id-badge"></i> Credits
    </h2>
    <div class="text-sm text-parchment-200/90 prose-block">
      <p class="mb-2"><b>Prototype:</b> Asia Khan, Hon. BA (McMaster University)</p>
      <p class="text-parchment-200/70 italic text-xs mb-3">Behavioral UX Researcher and Design Anthropologist</p>
      <p class="mb-2"><b>Imagery:</b> Esri · AWS Terrain · OpenStreetMap contributors</p>
      <p class="mb-0"><b>Referenced scholarly work:</b> The APA citations inside the interface point to real published research by authors including Caspari &amp; Radovčić, Monge et al., Frayer &amp; Russell, Radovčić et al., Trinkaus, Malez, and Gorjanović-Kramberger, among others. Full citations appear in each section.</p>
    </div>
  </section>

  <div class="divider"></div>

  <!-- LICENSE -->
  <section class="callout-lock rounded-xl p-5 md:p-7 mb-8">
    <div class="flex items-start gap-3">
      <i class="fa-solid fa-lock text-gold-500 text-2xl mt-0.5"></i>
      <div class="w-full">
        <h2 class="font-serif font-black text-xl text-parchment-100 mb-3 tracking-wide">License · All Rights Reserved</h2>
        <div class="text-sm text-parchment-200/95 prose-block">
          <p><b>© 2026 Asia Khan · All Rights Reserved</b></p>
          <p>This prototype, including its source code, interface design, written content, and procedural 3D models, is the intellectual property of the author. No part of this work may be reproduced, distributed, modified, or transmitted in any form or by any means without prior written permission from the author.</p>
          <p>The prototype is provided "as is" for demonstration and educational viewing purposes only, without warranty of any kind.</p>
          <p class="mb-0 text-parchment-200/80 text-xs italic">Third-party libraries (MapLibre GL, Three.js, Tailwind CSS, Google Fonts, Font Awesome, Esri imagery, AWS terrain tiles) are used under their respective licenses and remain the property of their original creators.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="mt-10 text-center text-xs text-parchment-200/50">
    <p class="mb-1"><i class="fa-solid fa-flask text-terracotta-600"></i> Prototype · for demonstration and educational commentary only</p>
    <p>© 2026 Asia Khan · All Rights Reserved</p>
  </footer>

</div>
</body>
</html>
