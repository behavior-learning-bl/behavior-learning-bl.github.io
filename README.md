# Behavior Learning — project website

A **ready-to-publish static GitHub Pages site** for:

> **Behavior Learning (BL): Learning Hierarchical Optimization Structures from Data**  
> Zhenyao Ma, Yue Liang, Dongxu Li. [arXiv:2602.20152](https://arxiv.org/abs/2602.20152).

The English narrative is deliberately aligned to the uploaded BL manuscript's Introduction: scientific motivation → performance–interpretability trade-off → two limitations → the UMP perspective → BL modular architecture and conditional Gibbs modeling → hierarchical optimization → identifiable BL → theory → evidence. The abstract is reproduced almost verbatim (links formatted for the web); figures are taken directly from the provided manuscript files.

## Publish to GitHub Pages

1. Create a new public repository on GitHub. For a personal homepage, name it `<your-username>.github.io`; for a project page, any repo name works (e.g. `behavior-learning-site`).
2. Upload **the contents of this folder** to the repository's root (so `index.html` lives at the root). Commit and push to the `main` branch.
3. Open **Settings → Pages → Build and deployment**. Choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. GitHub will publish at `https://<your-username>.github.io/` for a personal homepage, or `https://<your-username>.github.io/<repo-name>/` for a project page.

You do **not** need Node.js, React, Jekyll, npm, or a build system.

### Preview locally

Open `index.html` in your browser, or (recommended) run:

```bash
python -m http.server 8000
```

and navigate to `http://localhost:8000`.

External dependencies: Google Fonts and MathJax CDN for rendering mathematical formulas. Figures and the paper PDF are bundled and served locally. GitHub Pages supports these assets directly.

### Important links

- Paper: https://arxiv.org/abs/2602.20152
- Code: https://github.com/MoonYLiang/Behavior-Learning
- Install: `pip install blnetwork`

### Editing

- `index.html`: all English content, styles and figure interactions.
- `static/images/*.webp`: compressed, high-quality figures exported from the supplied paper PDFs. Clickable for close-up viewing.
- `static/favicon.svg`: simple BL icon.
- `paper.pdf`: the original supplied BL paper PDF.
- `.nojekyll`: tells GitHub Pages to serve static files without Jekyll processing.

The project page does not imply new empirical findings beyond those described in the manuscript. Verify the final BibTeX metadata against your preferred definitive publication record before making the website public.
