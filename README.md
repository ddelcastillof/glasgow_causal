# Causal Inference: An Application on Pensioner Poverty

A research presentation exploring methods for estimating the causal effects of pensioner poverty on health outcomes using panel data.

## Overview

This repository contains materials for a 7-minute presentation prepared for an interview at the **MRC/CSO Social and Public Health Sciences Unit, University of Glasgow**. The presentation addresses the key challenges in estimating causal effects of pensioner poverty on health using observational panel data.

## Research Question

**How can we estimate the causal effect of pensioner poverty on health outcomes?**

### Key Topics Covered

- Definitions and measurement of poverty in the UK
- Conditions for causal inference in observational studies
- Major challenges in estimation:
  - Time-varying confounding
  - Treatment-confounder feedback
  - Reverse causation
  - Heterogeneity in income definitions
  - SUTVA violations
- Potential methods: Marginal Structural Models (MSMs), g-estimation of SNMs, Doubly Robust Estimation
- Proposed analytical approach

## Repository Structure

```
.
├── README.md                      # This file
├── CLAUDE.md                      # Instructions for Claude Code
├── slides.qmd                     # Main Quarto presentation source
├── slides.html                    # Rendered HTML presentation
├── slides.pdf                     # PDF version of presentation
├── delcastilo_slides.pdf          # Additional PDF version
├── references.bib                 # Bibliography file
├── vancouver-superscript.csl      # Citation style
├── theme.scss                     # Custom Reveal.js theme
└── custom.css                     # Additional CSS styling
```

## Prerequisites

To work with this presentation, you need:

- [Quarto](https://quarto.org/) (latest version)
- R (for executing embedded R code)
- Required R packages: `ggdag`, `ggplot2`, `tidyverse`, `pacman`
- Decktape for exporting html slides to pdf

## Building the Presentation

### Render to HTML

```bash
quarto render slides.qmd
```

This generates `slides.html` with embedded resources.

### Live Preview

```bash
quarto preview slides.qmd
```

This opens a browser window with live reload on file changes.

### Export to PDF

```bash
decktape reveal slides.html slides.pdf
```

## Presentation Features

- **Format:** Reveal.js with embedded resources
- **Duration:** 7 minutes
- **Styling:** Custom SCSS theme with additional CSS
- **Interactive Elements:**
  - Slide navigation controls
  - Menu for quick navigation
  - Fade transitions
- **Content Features:**
  - DAG visualization using `ggdag`
  - LaTeX equations for statistical notation
  - Code syntax highlighting
  - Vancouver superscript citation style
  - Responsive design with scrollable slides

## Author

**Darwin Del Castillo**

## References

Key references include:

- Hernán MA, Robins JM. Causal Inference: What If (2025)
- Igelström et al. (2024) on income definitions in health research
- Marmot (2005) on social determinants of health
- GBD 2021 on burden of disease in older adults

Full bibliography available in `references.bib`.

## License

This is academic research material prepared for presentation purposes.
