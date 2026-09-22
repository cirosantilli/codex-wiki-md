# Pseudo-arclength continuation

↑ **Parent:** [Continuation method](continuation-method.md)

[Pseudo-arclength continuation](pseudo-arclength-continuation.md) allows both the state and the parameter to change. Write $z=(u,\lambda)$ and choose a [unit vector](unit-vector.md) $t_k$ in the [kernel](kernel-of-a-linear-map-split.md) of the full [Jacobian matrix](jacobian-matrix.md) $DF(z_k)$. A [continuation predictor-corrector step](continuation-predictor-corrector-step.md) seeks the next solution on a [hyperplane](hyperplane.md) perpendicular to $t_k$, a distance $h>0$ along the old [tangent vector](tangent-vector-split.md). This adds one equation to $F(z)=0$ and makes the correction a square system. The constraint approximates [arc length](arc-length.md); $h$ is the displacement projected onto the old [tangent vector](tangent-vector-split.md), rather than the exact curved distance.[§2.2, equations (2.2)–(2.5), printed pp. 265–266: unit tangent and hyperplane normalization; Corollary 2.3 gives local Newton convergence for sufficiently small steps](condition-estimates-for-pseudo-arclength-continuation-by-k-i-dickson-and-others.md)

**Table of contents**

- [Continuation predictor-corrector step](continuation-predictor-corrector-step.md)

## ↑ Ancestors (6)

1. [Continuation method](continuation-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Continuation method](continuation-method.md)
- [Pseudo-arclength continuation](pseudo-arclength-continuation.md)
