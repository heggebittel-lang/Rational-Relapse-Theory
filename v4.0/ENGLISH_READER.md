# v4.0 English Reader — A Structural Model of Rational Addiction

**Author:** Yushang Cheng  
**Original manuscript date:** 26 June 2026  
**Repository version:** v4.0  
**Original internal label:** v6.2

> **Archival note.** This is an English reader's translation of the main structure and results of the historical Chinese manuscript. It is intended to make this research stage understandable to non-Chinese readers. The original Chinese manuscript is the authoritative historical version. Later literature audits, later terminology, and later revisions have not been retrofitted into this account.

## Abstract

This manuscript asks whether, within a rational-addiction framework, recovery can enter utility as an endogenous force that counteracts dynamic reinforcement. Instantaneous utility is decomposed into reinforcement utility $F_0(c,A)$ and recovery utility $G(c,A,R)$, where $R=A-A^*$ is the difference between actual addiction stock and a target stock. The manuscript develops an axiomatic representation and a kernel family, derives conditions under which the recovery component reverses adjacent complementarity in the consumption-stock cross margin, studies steady-state folds and Personal Equilibrium formulations of the target, and adds delayed target formation to generate a two-state system with oscillatory dynamics. The numerical Neimark-Sacker example has a positive first Lyapunov coefficient and is therefore subcritical under the sign convention used in the manuscript.

## 1. States and basic structure

Actual addiction stock evolves according to

$$
A_{t+1}=(1-\delta)A_t+c_t,\qquad \delta\in(0,1).
$$

Let $A_t^*$ denote a target addiction stock and define the recoverable gap

$$
R_t=A_t-A_t^*.
$$

The historical model decomposes current utility as

$$
U_t=F_0(c_t,A_t)+G(c_t,A_t,R_t).
$$

$F_0$ retains the standard Becker-Murphy reinforcement properties, including $(F_0)_{cA}>0$. The target $A_t^*$ is treated as a state rather than a current control: it is fixed in the baseline model and later follows an adaptive law of motion.

## 2. Axiomatic representation

For each state $(A,R)$, the primitive is a conditional preference relation over consumption. The June 2026 manuscript imposes weak order, continuity, addiction complementarity, reference independence at the target, monotone crossing of the recovery increment, convexity of $G$ in consumption, and concavity of $G$ in recoverable stock.

The manuscript states a representation

$$
F(c,A,R)=F_0(c,A)+G(c,A,R),
$$

with the properties

$$
G(c,A,0)=0,\qquad G(R,A,R)=0,\qquad G_c<0,\qquad G_{cc}>0,\qquad G_{RR}<0.
$$

The additive special case has $G_A\equiv0$. The more general construction allows $G_A\neq0$, so two states with the same gap $R$ but different absolute addiction stocks may have different recovery increments.

## 3. Recovery kernel

The early linear benchmark is

$$
G(c_t,A_t,R_t)=\eta(R_t-c_t).
$$

The manuscript then replaces this with the kernel family

$$
G(c_t,A_t,R_t)=\int_{c_t}^{R_t}q(s,A_t)\,ds,
$$

where

$$
q(s,A;\eta)=\eta\,\widetilde q(s,A),\qquad \widetilde q>0,\qquad \widetilde q_s<0.
$$

The scale parameter $\eta$ is separated from the otherwise general two-variable kernel $\widetilde q(s,A)$. A tractable separable subclass is

$$
\widetilde q(s,A)=q_0(ks)\phi(A),
$$

with examples such as $q_0(s)=e^{-ks}$ and $\phi(A)=1+\gamma A$.

The integral structure automatically gives

$$
G(R,A,R)=0.
$$

Absolute-stock dependence is

$$
G_A(c,A,R)=\eta\int_c^R\widetilde q_A(s,A)\,ds,
$$

whose sign is intentionally left unrestricted in this version.

### Reinforcement-substitution reversal

For composite flow utility $U=F_0+G$, the manuscript derives

$$
U_{cA}(c,A)=(F_0)_{cA}(c,A)-\eta\widetilde q_A(c,A).
$$

Thus the usual adjacent complementarity is preserved when $\widetilde q_A=0$. At a fixed point $(c,A)$, reversal occurs when

$$
\widetilde q_A(c,A)>\frac{(F_0)_{cA}(c,A)}{\eta},
$$

which implies $U_{cA}<0$. This was called the **reinforcement-substitution reversal** in the historical manuscript.

The manuscript also considers a more general target-dependent kernel $q(s,A,R)$, for which $G_{cR}$ need not vanish.

## 4. Dynamic programming

The forward-looking agent solves

$$
V(A_t;A_t^*)=\max_{c_t}\left\{F_0(c_t,A_t)+G(c_t,A_t,R_t)+\beta_dV(A_{t+1};A_t^*)\right\},
$$

subject to the stock law above. For an interior choice,

$$
(F_0)_c(c_t,A_t)-q(c_t,A_t)+\beta_dV'(A_{t+1};A_t^*)=0.
$$

The envelope condition accounts for both the direct effect of $A_t$ on recovery and the effect operating through $R_t=A_t-A_t^*$.

## 5. Steady states and the fold threshold

At a stationary solution,

$$
\bar A=\frac{c^*}{\delta},\qquad \bar R=\frac{c^*}{\delta}-A^*,\qquad r=1-\beta_d(1-\delta).
$$

After eliminating the shadow value, the steady-state equation is written as $\Phi(c^*;\eta)=0$. Because $q=\eta\widetilde q$, the manuscript observes that this equation is exactly affine in $\eta$:

$$
\Phi(c^*;\eta)=\Phi_0(c^*)+\eta\Xi(c^*),
$$

where

$$
\Phi_0(c^*)=(F_0)_c(c^*,\bar A)+\frac{\beta_d}{r}(F_0)_A(c^*,\bar A),
$$

and

$$
\Xi(c^*)=-\widetilde q(c^*,\bar A)+\frac{\beta_d}{r}\left[\int_{c^*}^{\bar R}\widetilde q_A(s,\bar A)\,ds+\widetilde q(\bar R,\bar A)\right].
$$

Defining

$$
H(c^*)=-\frac{\Phi_0(c^*)}{\Xi(c^*)},
$$

the manuscript characterizes a degenerate steady-state root by a critical point of $H$: if $c^\dagger$ is such a point under the stated regularity conditions, then the fold parameter is $\eta^\dagger=H(c^\dagger)$.

### Historical numerical example

The illustrative specification is

$$
F_0(c,A)=\ln c+\alpha cA,\qquad q_0(s)=e^{-ks},\qquad \phi(A)=1+\gamma A,
$$

with $\delta=0.1$, $\beta_d=0.95$, $\alpha=1$, $k=1$, $\gamma=0.5$, and $A^*=2$. The reported numerical fold is

$$
c^\dagger\approx1.0190,\qquad \eta^*_{\mathrm{fold}}\approx17.716.
$$

For $\eta=10$ there is no root in the displayed region; at the threshold the steady-state equation is tangent to zero; and for $\eta=25$ the manuscript reports two positive roots near $0.735$ and $1.686$.

The historical fold figure visualizes exactly this $0\rightarrow2$ root creation.

## 6. Target stock as a Personal Equilibrium

The manuscript next asks whether the target can itself be a fixed point: the target stock equals the steady-state stock generated when that target is maintained. At such a Personal Equilibrium, $c^{*PE}=\delta A^{*PE}$ and the recoverable gap is zero.

In the separable family with linear modulation

$$
\phi(A)=1+\gamma A,
$$

the manuscript obtains a nonexistence result under $\beta_d/r>1$: for $\gamma\ge0$, the Personal Equilibrium equation remains positive for every $c^*>0$.

Two alternative constructions are then used to show that the tension comes from the tractable linear family rather than from the general idea:

1. **Exponential modulation:** $\phi(A)=\phi_0e^{\kappa A}$ with $\kappa>k$ restores Personal Equilibrium existence for every $\eta>0$ under the stated conditions, and sufficiently large equilibrium stock can also satisfy the reversal condition.
2. **Target-dependent kernel:** keeping linear $\phi(A)$ but allowing $q(s,A,R)=\eta q_0(ks)\phi(A)\chi(R)$ restores existence when $\chi'(0)>k\chi(0)$ and $\eta$ exceeds an explicit threshold.

The manuscript itself notes that the exponential route creates a new growth tension with the earlier fold analysis.

## 7. Delayed target formation and oscillatory dynamics

The final extension replaces the fixed target with an adaptive state:

$$
A_{t+1}^*=(1-\rho)A_t^*+\rho w(A_t),\qquad \rho\in(0,1).
$$

Actual stock follows

$$
A_{t+1}=(1-\delta)A_t+c^*(A_t,A_t^*).
$$

Define local policy sensitivities at a steady state by

$$
c_A=\frac{\partial c^*}{\partial A_t},\qquad c_{A^*}=\frac{\partial c^*}{\partial A_t^*}.
$$

Linearization gives

$$
\begin{pmatrix}x_{t+1}\\y_{t+1}\end{pmatrix}
=
\begin{pmatrix}
1-\delta+c_A & c_{A^*}\\
\rho w_A & 1-\rho
\end{pmatrix}
\begin{pmatrix}x_t\\y_t\end{pmatrix}.
$$

Its characteristic polynomial is

$$
\lambda^2-T\lambda+D=0,
$$

with

$$
T=2-\delta-\rho+c_A,
$$

$$
D=(1-\delta+c_A)(1-\rho)-c_{A^*}\rho w_A.
$$

Complex roots arise when $T^2<4D$. If $D<1$, the oscillation contracts; if $D=1$, its linearized amplitude is constant; if $D>1$, it expands.

### Neimark-Sacker condition

Using $\rho$ as a bifurcation parameter, the manuscript imposes at $\rho^*$: complex roots, transversality of the crossing of $D=1$, nonresonance, and a nonzero first Lyapunov coefficient $l_1$.

In the numerical example, $w(A)=\omega A$ with $\omega=0.483$. The selected steady state is reported as

$$
\bar c\approx1.21495,\quad \bar A\approx12.150,\quad \bar A^*\approx5.868,\quad \bar R\approx6.281.
$$

The bifurcation point is

$$
\rho^*\approx0.029261,
$$

with

$$
T(\rho^*)\approx1.999143,\qquad D(\rho^*)\approx1,
$$

and eigenvalues approximately

$$
0.99957\pm0.02926i.
$$

The manuscript reports a numerical transversality derivative around $-1.990$ and an implied linearized rotation period of roughly $215$ periods. This is explicitly described as an illustrative magnitude, not an empirical calibration.

After computing second- and third-order policy derivatives, the manuscript obtains

$$
l_1\approx0.4906>0.
$$

Therefore the reported Neimark-Sacker bifurcation is **subcritical**. The manuscript explicitly acknowledges that this numerical example does *not* generate the stable quasiperiodic relapse-cessation cycle imagined in the original motivation; under its sign convention, a stable invariant curve would require $l_1<0$.

## 8. Open issues already acknowledged in v4.0

The June 2026 conclusion leaves four issues open:

- **Dynamic self-correction:** reversal of $U_{cA}$ does not prove that the optimal policy necessarily moves the state toward the target.
- **Full target endogenization:** adaptive target dynamics and Personal Equilibrium are distinct constructions; the manuscript does not unify them completely.
- **Identification:** the paper does not establish that observed consumption-stock paths separately identify $F_0$ and the recovery-kernel parameters.
- **Calibration:** the fold and Neimark-Sacker exercises are illustrative numerical examples rather than estimates from data.

## Archival interpretation

At this stage of the project, the central object was an endogenous recovery term evaluated by the same forward-looking agent who values addictive consumption. The manuscript had already moved from a specific functional form to an axiomatic/kernel representation and then to target fixed points and two-state local dynamics. It also already contained an important internal limitation: a local cross-margin reversal is not a theorem of dynamic recovery, and the numerical bifurcation example is subcritical rather than a stable relapse cycle.

Later versions of the project changed the primitives, language, and interpretation substantially. This file is preserved so that the historical v4.0 stage can be read without treating its claims as the author's final position.
