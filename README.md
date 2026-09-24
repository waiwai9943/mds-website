# Isaac Wu's Personal Web

This repository contains the source code for Isaac Wu's personal website and blog. It is built using Quarto and deployed via GitHub Pages.

## Prerequisites

Before you begin, ensure you have the following installed (these are the versions used to build this site):

- **Quarto:** v1.10.18
- **uv:** v0.12.7
- **R:** v4.6.1


**1. Clone the repository (Run in Shell):**
```bash
git clone https://github.com/waiwai9943/mds-website.git
cd mds-website
```

**2. Install Python dependencies (Run in Shell):**
```bash
uv sync
```

**3. Install R dependencies (Run in R console at the project root):**
```R
renv::restore()
```

**4. Build the site (Run in Shell):**
```bash
uv run quarto render
```
or
```bash
uv run quarto preview
```

- **Python & R Data Sources:** The blog posts demonstrate importing the Palmer Penguins dataset using language-specific packages. In Python, the dataset is loaded via the `palmerpenguins` Python package (`load_penguins()`). In R, it is loaded via the `palmerpenguins` R library (`data("penguins")`).
