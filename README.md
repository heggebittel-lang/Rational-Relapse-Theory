# A Structural Model of Rational Addiction

[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.20632874-blue)](https://doi.org/10.5281/zenodo.20632874)
**Author:** Yushang Cheng
[![ORCID](https://img.shields.io/badge/ORCID-0009--0001--3218--6423-green)](https://orcid.org/0009-0001-3218-6423)
**Status:** Working Paper / Complete Manuscript
**License:** [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)

---

## Overview

This repository presents **A Structural Model of Rational Addiction**, an extension of the classic Becker–Murphy (1988) framework. The key innovation is the introduction of quadratic **adjustment friction** and an endogenous **exit mechanism** represented by a family of integral utility functions, providing a microfoundation for voluntary cessation and rational relapse within a standard utility-maximization model.

Unlike traditional models where addiction is often either monotonic convergence or irreversible divergence, this framework reveals a third possibility: **rational relapse**—spiral divergent paths that satisfy all necessary conditions for rational optimality.

## Key Innovation

The **exit mechanism** $g(c_t, A_t) = \int_{c_t}^{A_t} q(s)\,ds$ is axiomatically derived from six conditions (C1)–(C6), generalizing beyond the linear benchmark to a full function family of kernel functions $q(s)$. This provides three core theoretical advantages:

| Feature | Description |
|---|---|
| **Function Family Generalization** | Axiomatic derivation ensures results hold for any convex, monotonic exit utility form, not just a linear specification |
| **Rational Relapse** | Interaction between adjustment friction and exit mechanism generates complex characteristic roots, producing spiral divergent paths compatible with the Euler equation and transversality condition |
| **Empirical Distinguishability** | The three-regime partition yields testable predictions—oscillation frequency, amplitude growth rate $\rho = \beta_d^{-1/2}$, and constant relapse intervals—distinguishing this model from the standard Becker–Murphy framework |

## Repository Structure & Versions

This project has evolved through multiple versions:

### Latest: [v3.0](./v3.0/)

[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.20632874-blue)](https://doi.org/10.5281/zenodo.20632874)

This is the **current version**. The manuscript has been fully translated from Chinese to English. Major theoretical expansions include the axiomatic derivation of the integral-form function family, analytical solutions for spiral trajectories, and a complete welfare analysis. See [v3.0/README.md](./v3.0/README.md) for details.

### [v2.0](./v2.0/) — Complete Manuscript

The original complete manuscript in Chinese, establishing the core theoretical framework, three-regime theorem, and policy implications.

### [v1.0](./v1.0/) — Initial Preprint

The original working paper with a brief sketch of the model.

## Version History

### v3.0 — Function Family Generalization

- **Axiomatic derivation** of the exit mechanism function family with six axioms (C1)–(C6)
- **State invariance proposition** proving the linear benchmark is the unique member satisfying translation invariance
- **Analytical trajectory equations** for spiral paths, including closed-form solutions for addiction stock
- **Exact formulas** for relapse timing, intensity, and the endogenous narrowing of intervention windows
- **Intervention cutoff time** $T^*$ formula with three testable predictions
- **Welfare loss analysis** with qualitative conclusions on early intervention superiority
- **Shadow price feedback term** explicitly incorporated into $H_c$ for clearer regime interpretation

### v2.0.2 — Envelope Theorem Revision

Revised envelope condition derivation and corrected the shadow price feedback mechanism.

### v2.0.1 — Formatting Fixes

Minor formatting corrections and reference updates.

### v2.0.0 — Complete Manuscript

First complete manuscript with full theoretical framework, dynamic programming derivation, three-regime theorem, and empirical predictions.

### v1.0.0 — Initial Preprint

Initial conceptual framework and preliminary mathematical derivation.

## Citation

If you use this work, please cite as:

> Cheng, Y. (2026). *A Structural Model of Rational Addiction* (v3.0). Zenodo. <https://doi.org/10.5281/zenodo.20632874>

For earlier versions:

> Cheng, Y. (2026). *A Structural Model of Rational Addiction* (v2.0). Zenodo. <https://doi.org/10.5281/zenodo.20086392>
>
> Cheng, Y. (2026). *A Structural Model of Rational Addiction* (v1.0). Zenodo. <https://doi.org/10.5281/zenodo.19743247>

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

Copyright (c) 2026 Yushang Cheng.

