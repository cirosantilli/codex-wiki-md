# Non-Boussinesq top-hat plume equations

↑ **Parent:** [Top-hat plume model](top-hat-plume-model.md)

For a [turbulent plume](turbulent-plume-split.md) in a homogeneous ambient of density $\rho_0$, define actual sectional [mass flux](mass-flux.md), [momentum flux](momentum-flux.md) and density-weighted [buoyancy flux](buoyancy-flux.md) by $Q=\pi b^2\rho w$, $M=\pi b^2\rho w^2$ and $F=\pi b^2wg(\rho_0-\rho)$. With non-Boussinesq [Batchelor entrainment](batchelor-entrainment-hypothesis.md) $v_e=\alpha w\sqrt{\rho/\rho_0}$, their balances are

$$
\partial_t(Q^2/M)+\partial_zQ=2\alpha\sqrt{\pi\rho_0M},\qquad
\partial_tQ+\partial_zM=QF/M,\qquad
\partial_t(QF/M)+\partial_zF=0.
$$

Here $Q^2/M$ is sectional mass, $QF/M$ is sectional density-deficit buoyancy, and the entrained ambient initially has zero vertical momentum. The last equation follows by subtracting mass conservation from $\rho_0$ times volume conservation. [Scase, Caulfield, Dalziel and Hunt's time-dependent plume model](https://doi.org/10.1017/S0022112006001212) derives the equivalent system with the common factor $\pi$ suppressed.

**Table of contents**

- [Non-Boussinesq pure-plume density transition](non-boussinesq-pure-plume-density-transition.md)

## ↑ Ancestors (6)

1. [Top-hat plume model](top-hat-plume-model.md)
2. [Turbulent plume](turbulent-plume-split.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345/3/b/solution.md)
