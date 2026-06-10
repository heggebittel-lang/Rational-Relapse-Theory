# A Structural Model of Rational Addiction — v3.0

[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.20632874-blue)](https://doi.org/10.5281/zenodo.20632874)
**Author:** Yushang Cheng
**ORCID:** [0009-0001-3218-6423](https://orcid.org/0009-0001-3218-6423)
**License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

---

## About This Version

This is **v3.0** of *A Structural Model of Rational Addiction*. It represents a major revision of the previous v2.0 manuscript, featuring:

1. **Complete English translation** of the entire manuscript and all appendices
2. **Axiomatic generalization** of the exit mechanism from a linear benchmark to a full function family
3. **Analytical closed-form solutions** for spiral relapse trajectories, timing, and intensity
4. **Complete welfare analysis** of rational relapse paths

---

## Main Contributions

### 1. Axiomatic Function Family for the Exit Mechanism

The exit utility is generalized from the linear benchmark $g(c_t, A_t) = \eta(A_t - c_t)$ to an integral-form function family:

$$g(c_t, A_t) = \int_{c_t}^{A_t} q(s)\,ds, \quad q(s) > 0,\; q'(s) < 0$$

governed by six axioms (C1)–(C6): convexity, monotonicity, boundary condition, linear degeneracy, separability, and curvature persistence. This ensures the model's qualitative conclusions hold for any convex, monotonic exit utility specification.

**Proposition (State Invariance):** The linear benchmark $g(c_t, A_t) = \eta(A_t - c_t)$ is the *unique* member of the function family satisfying state invariance $g(c_t + k, A_t + k) = g(c_t, A_t)$, providing a rigorous characterization of when the linear benchmark suffices and when the general family is required.

### 2. Rational Relapse: Analytical Characterization

The interaction between adjustment friction $\gamma$ and the exit mechanism generates complex characteristic roots in the linearized Euler equation when $\Delta < 0$ (Regime II). The consumption path follows:

$$\tilde{c}_t = R\,\rho^{\,t}\cos(t\theta + \phi), \quad \rho = \beta_d^{-1/2} > 1$$

This spiral divergent path satisfies both the Euler equation and the transversality condition, establishing compatibility with fully rational optimization.

**Hartman–Grobman Extension (Corollary):** The qualitative spiral divergence conclusion holds strictly for the *original nonlinear system* via topological conjugacy, independent of linearization accuracy.

### 3. Exact Analytical Formulas for Relapse Dynamics

The appendices provide closed-form solutions for:

- **Relapse timing:** $t_n^{\max} = \dfrac{(2n-1)T}{4} - \dfrac{\phi}{\theta}$, with constant inter-relapse interval $T/2$
- **Relapse intensity:** $\tilde{c}_{t_n^{\max}} = C_0\,\varrho^{2n-1}$, growing as a geometric series with ratio $\varrho^2 = \beta_d^{-T/2}$
- **Intervention cutoff time:** $T^* = \dfrac{\ln(\bar{c} - c^*) - \ln R}{\ln\rho}$, yielding three testable predictions
- **Endogenous window narrowing:** the relapse trough increases monotonically with cycle count, narrowing the intervention window geometrically

### 4. Complete Welfare Analysis

A formal welfare loss framework quantifies the cumulative utility gap between the actual spiral path and the hypothetical steady-state path:

$$\mathcal{W} = \sum_{t=0}^{T^*} \beta_d^t\bigl[U(\bar{c}, \bar{A}) - U(c_t, A_t)\bigr]$$

Three qualitative conclusions emerge directly from the spiral structure:
- Welfare loss grows **superlinearly** with initial deviation $R$
- Loss **increases** as the discount factor $\beta_d$ decreases
- The benefit of early intervention **decreases strictly** with delay, confirming the superiority of early intervention

### 5. Empirical Compatibility

The linearized Euler equation maintains full compatibility with the empirical literature (Chaloupka 1991, Becker et al. 1994). The identification result $\beta_d = \phi_2/\phi_1$ remains robust to the specific form of the utility function. The model adds a fifth testable prediction: under Regime II, individual consumption paths should exhibit oscillations with angular frequency $\omega$ and amplitude growth rate $\rho$, providing a basis for **empirical distinguishability** from the standard Becker–Murphy framework.

---

## What's New in v3.0

| Feature | v2.0 | v3.0 |
|---|---|---|
| Language | Chinese | English (full translation) |
| Exit mechanism | Linear benchmark $g = \eta(A_t - c_t)$ | Axiomatic function family $\int_{c_t}^{A_t} q(s)\,ds$ with (C1)–(C6) |
| State invariance | Not discussed | Proposition with full proof |
| Relapse timing | Qualitative description | Exact analytical formula $t_n^{\max}$ |
| Relapse intensity | Qualitative description | Closed-form geometric series $C_0\varrho^{2n-1}$ |
| Intervention cutoff | Conceptual discussion | Precise formula $T^*$ with three testable predictions |
| Welfare analysis | Not included | Complete framework with qualitative conclusions |
| Nonlinear extension | Mentioned | Hartman–Grobman corollary with full proof |
| Shadow price feedback | Implicit | Explicitly separated in $H_c$ expression |
| Appendix structure | Minimal | Four detailed technical appendices |

---

## File Structure

```
v3.0/
├── v3.0.tex          # Main LaTeX source file
├── v3.0.pdf          # Compiled manuscript
├── README.md         # This file
├── fig1_regimes.png  # Three-regime partition figure
├── fig2_transition.png # Endogenous regime transition figure
├── fig3_timeseries.png # Analytical consumption path
├── fig4_phase.png    # Phase diagram
├── fig4_new.png      # Regime partition under linear baseline
└── fig5_multifunction.png # Exit utility function family comparison
```

---

## Citation

> Cheng, Y. (2026). *A Structural Model of Rational Addiction* (v3.0). Zenodo. <https://doi.org/10.5281/zenodo.20632874>

---

## License

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Copyright (c) 2026 Yushang Cheng.
