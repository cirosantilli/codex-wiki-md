# SIR model with demography and permanent immunity

↑ **Parent:** [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)

With susceptible, infective, and immune populations $X,Y,Z$, equal per-capita birth and death rate $\mu$, mass-action transmission coefficient $\beta$, and recovery rate $\nu$, the equations are

$$
X'=\mu N-\beta XY-\mu X,
\qquad Y'=\beta XY-(\mu+\nu)Y,
\qquad Z'=\nu Y-\mu Z.
$$

The conserved population is $N=X+Y+Z$, and the threshold population is $N_c=(\mu+\nu)/\beta$.

**Table of contents**

- [Endemic equilibrium of the SIR model with demography](endemic-equilibrium-of-the-sir-model-with-demography.md)

## ↑ Ancestors (5)

1. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
2. [Mathematical biology](mathematical-biology-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/6a/a/solution.md)
