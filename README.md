# Exact Boolean Support Identification from Sector Counts and Weight-Limited Queries

Reproducibility materials for the research manuscript being prepared for *Information Sciences*. This repository is a **research artifact**, not a claim of publication, independent certification of every computation, or a final release.

## Download the research package

The current `main` branch contains [IS_GITHUB_REPRODUCIBILITY_STAGING_2026-10-22.zip](IS_GITHUB_REPRODUCIBILITY_STAGING_2026-10-22.zip). Unzip it locally. The package contains 45 items under `boolean-support-reproducibility/`.

**Important:** The ZIP is still a staging snapshot. Historical components may require additional source data and dependencies. A versioned, individually browsable source release will follow audit.

## Most useful reproducibility checks

From the extracted `boolean-support-reproducibility` directory, with Python 3.10+:

```bash
python adaptive_n5/verify_saved_tree.py
python proofs/verify_nonadaptive_witnesses.py
```

The first verifies a saved adaptive tree of depth 14 on 2,250 five-variable Boolean functions sharing the profile `(0,0,1,2,1,0)`. The second tests finite nonadaptive conflicting-pair witnesses and does not replace the analytical proof for arbitrary dimension.

## What the package contains

- `src/`: original baseline programs, exact finite certificate and minimax checks, empirical corpus utilities
- `k6/`: independent reproduction of 147 capped-certificate tasks, with archival outputs and conditions
- `adaptive_n5/`: saved tree and independent verifier; the **exact adaptive optimum is not known yet**
- `proofs/`: analytical unbounded additive-gap theorem, finite witness tests and tabulated bounds
- `experimental/`: derived retrospective BLADE analysis and uncertainty tables
- `search/`: ongoing resumable CPU/Colab search, *not* a completed optimality certificate
- `CHECKS.md` and `DATA_PROVENANCE.md`: verification scope and provenance

## Scope

The experimental analysis does **not** demonstrate that obtaining a sector profile saves physical measurement cost. Its thresholds are exploratory. Third-party raw network and laboratory datasets are not mirrored without a redistribution review.

**No license has yet been selected for original research code.** Do not assume permission for redistribution or derivative use beyond applicable law.

For citation, use a fixed GitHub commit after review, or a tagged release/DOI once available.
