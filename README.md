# Nandalal — Digital Marketing Portfolio

A static, interactive Three.js portfolio with a portrait-led main character, a selectable companion avatar, a modern workplace atrium, company-name wall signage, career timeline, projects, skills, credential artwork and contact actions.

## Publish with GitHub Pages
In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, then save.

Expected address:
https://nsnandalal-stack.github.io/nandalal_performance_marketing_portfolio/

## Controls
- Choose a male or female companion in the top-right controls.
- Use W/A/S/D or arrow keys to move. The on-screen directional pad works on touch screens.
- Drag on the 3D environment to look around.
- Select a glowing marker or a career milestone to open its details.
- Use the left navigation for experience, projects, skills, credentials and contact.
- Narration uses the browser's speech synthesis.

## Company references and logos
The company destinations are matched to these official domains: Stark — stark.in; Toonz — toonz.co; FAARMS — faarms.in; Acharya — acharya.ac.in; Xentrix — xentrixstudios.com. Small brand icons are website favicons loaded from those domains through Google's favicon service. The 3D lobby wall uses company-name wordmarks rather than recreated official vector artwork.

## Implementation notes
The main guide uses the supplied portrait, attached to a simple 3D lower body; it is not a fully rigged photorealistic 3D model. The companion is a procedural stylised avatar. Three.js is loaded from jsDelivr, and favicon icons are fetched from Google's favicon service, so an internet connection is required. Metrics shown are portfolio-reported figures, not third-party audited results. The website HTML is stored as a gzip payload in `assets/site-payload.bin` and decompressed by the root `index.html` loader.
