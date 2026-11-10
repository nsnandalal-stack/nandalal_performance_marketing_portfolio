# Nandalal — Interactive 3D Performance Marketing Portfolio

A static portfolio experience built with Three.js. Visitors can walk through workplace-inspired career chapters, view your portrait as the lead guide, and choose a companion avatar that follows behind.

## Publish with GitHub Pages

1. Open **Settings → Pages** in this repository.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Choose branch **main** and folder **/(root)**, then click **Save**.
4. After GitHub Pages finishes its first deployment, open the URL shown in the Pages settings. It is expected to be:
   `https://nsnandalal-stack.github.io/nandalal_performance_marketing_portfolio/`

## Local preview

Run `python3 -m http.server 8000` from the repository root, then open `http://localhost:8000`.

## Controls

- Choose a male or female companion at the opening screen.
- Use **WASD** or the arrow keys to move; drag to look around.
- Select a glowing marker or career milestone to open a chapter.
- Use **Narrate** for browser speech narration.

## Implementation notes

The HTML experience is gzip-compressed in `assets/site-payload.bin` and expanded by the root `index.html` loader using the browser's `DecompressionStream` API. Three.js is loaded from a CDN, so an internet connection is required. The lead character uses the supplied portrait image on a 3D body/plane; it is not a fully rigged photorealistic 3D human. Company marks are loaded as website favicons rather than verified vector logo assets.
