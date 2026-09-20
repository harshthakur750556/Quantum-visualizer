# Quantum Visualizer

An interactive, browser-based visualization of atomic structure. Start at the catalogue landing page and launch the explorer to see electron configurations represented as shells or probability-based orbitals.

## Open the project

No build step is required. Serve the repository with any static file server, or open [`index.html`](index.html) directly in a modern browser. The landing page links to [`atom.html`](atom.html) and automatically opens it after a short introduction.

For a local server with Python:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Features

- Responsive, aesthetic catalogue landing page with an automatic redirect to the explorer.
- Interactive 3D atom rendered with [Three.js](https://threejs.org/).
- Shells view for a schematic, Bohr-style representation.
- Orbitals view showing Monte Carlo samples of electron probability distributions.
- Elements 1–36, from hydrogen through krypton.
- Electron configurations using the Aufbau principle, Hund's rule, and the Pauli exclusion principle.
- Quantum-number details, spin indicators, radial nodes, and an approximate effective nuclear charge using Slater's rules.
- Mouse, touch, drag, pinch, and scroll controls for exploring the scene.

## Project files

| File | Purpose |
| --- | --- |
| `index.html` | Catalogue-style entry page and redirect to the visualizer. |
| `atom.html` | Self-contained interactive atomic orbital explorer. |
| `wrangler.json` | Cloudflare Wrangler configuration, if deploying with Workers/Pages tooling. |

## Scientific note

This is an educational visualization rather than a precision quantum-chemistry simulator. The explorer uses hydrogen-like orbital shapes with Slater screening as a classroom approximation; real multi-electron wavefunctions are correlated and are not exactly separable in this way.

## License

No license has been specified for this repository yet. Add a license before redistributing the project or its assets.
