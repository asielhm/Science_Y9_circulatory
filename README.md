# Heart Lab — Y9 Circulatory System

A GitHub Pages–ready learning website built from the uploaded OrganUI heart model (`heart-3d-main`). No build tools are needed.

## Lesson flow

1. **In the body** — illustrated location of the heart between the lungs.
2. **Zoom into the heart** — a real rotatable anatomical GLB heart model; clicking structures displays their function.
3. **Guided virtual dissection** — staged removal of the right atrial wall, left atrial wall, and *combined* ventricular wall to reveal ventricular cavity surfaces, with knowledge checks.

**Scientific limitation:** This is a staged hide/reveal model, not physically accurate freehand scalpel dissection. The source GLB combines the two ventricular walls into one mesh, and does not contain the heart valves, pulmonary veins, full lung geometry or body. The torso on page 1 is an illustrative SVG. Missing anatomy is explicitly explained in the lesson. Do not claim that users can dissect valves in 3D.

## Publish on GitHub Pages

1. Create a new public GitHub repository (e.g. `y9-heart-lab`).
2. Upload **all files**, retaining the `models/heart.glb` folder and `index.html` at repository root.
3. Go to Settings → Pages → Build and deployment → Deploy from a branch → `main` → `/ (root)` → Save.
4. Open `https://YOUR-USERNAME.github.io/y9-heart-lab/` after deployment.

You can also publish from a repository you already have, by placing these files at its root (be aware that replacing its `index.html` will replace its old homepage).

The 3D viewer loads Three.js modules from jsDelivr CDN. Internet is needed at least on initial load. Opening `index.html` directly as a `file://` local file may not work because the browser blocks module/model loading. Use GitHub Pages or a local web server such as `python -m http.server 8000`.

## Attribution

The model `models/heart.glb` comes from the supplied OrganUI project and its BodyParts3D anatomical reconstruction. Model attribution and license information is in `MODEL-ATTRIBUTION.md`. BodyParts3D material is CC BY 4.0. Preserve attribution if you republish. The app page implementation is an original educational adaptation.
