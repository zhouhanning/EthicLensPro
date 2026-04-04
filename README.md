# EthicLens Pro

**Decision support for lawful, fair, and defensible analytics.**

EthicLens Pro is a single-page web app that helps data analysts walk through an **AI data governance cycle**, with reference material on **GDPR-aligned privacy**, **explainable AI (XAI) and accountability**, **scientific integrity**, **bias and fairness**, and **AI risk / foresight**. It is a structured checklist and learning aid—not a substitute for legal, compliance, or institutional review.

## Features

### Governance cycle (8 steps)

For each stage: a guiding question (“system signal”), mandatory actions, strict prohibitions, primary principle, philosophical/legal basis, and an expandable **Rationale & context** section.

- **Navigation** — Previous/Next buttons, clickable step dots, a progress bar, and **← / →** keyboard shortcuts (when the Governance cycle tab is active and focus is not in a form field).
- **Step 8** — Explainability and accountability (ties to the XAI tab: documentation, redress, limits of explanations).

### Reference tabs

- **Ethical frameworks** — Utilitarian, deontological, contractualist, and particularist lenses; social models of exchange; moral-psychology notes.
- **Privacy & GDPR** — Data-subject rights, principles, legal bases, sensitive categories, consent, re-identification risk, and privacy–utility trade-offs.
- **Bias & fairness** — Selection bias, proxy bias, fairness impossibility (conflicting error metrics), accountability.
- **Rigorous analysis** — Hypothesis testing order, Type I/II thinking, anti-patterns (e.g., HARKing, p-hacking), mitigations.
- **AI risk & foresight** — Framings of AI discourse, risk themes, structured forecasting practices.
- **XAI & accountability** — Interpretability vs post-hoc explanation; methods (e.g., LIME, SHAP, counterfactuals, global dependence); GDPR Article 22–style transparency; interactive audience selector, complexity slider, and true/false checks.

### Quick checks

- Flip-card Q&A (keyboard: flip with Enter/Space; arrows to move through the deck).
- Short interactive scenario (e.g., re-identification response).

## Tech stack

- **HTML5** + **vanilla JavaScript** (no build step)
- **Tailwind CSS** (via CDN)
- **Font Awesome 6** (via CDN)

## Getting started

### Run locally

1. Clone or download this repository.
2. Open `index.html` in a modern browser (double-click, or use a local static server if you prefer).

Example with Python:

```bash
cd ethic
python -m http.server 8080
```

Then visit `http://localhost:8080` in your browser.

### Deploy to GitHub Pages

1. Push this repository to GitHub.
2. In the repo **Settings → Pages**, set the source to your default branch and `/ (root)` or the folder containing `index.html`.
3. Your site will be served as static files; no build command is required.

## Project structure

```
ethic/
├── index.html           # Full application (markup, styles, scripts)
├── README.md            # This file
└── README-for-GitHub.txt # Plain-text copy of the README (optional copy/paste)
```

## Disclaimer

EthicLens Pro is an **educational and decision-support prototype**. It does not provide legal advice, regulatory certification, or approval for human-subjects research. Always follow your organization’s policies, applicable law (including GDPR where relevant), and ethics review requirements.

## License

Add a `LICENSE` file if you plan to open-source this project; until then, all rights are reserved unless you specify otherwise.
