# Signed swept area

↑ **Parent:** [Areal velocity](areal-velocity.md)

Signed swept area counts the [area](surface-area.md) traversed by a [position](position.md) [vector](vector.md), positively or negatively according to its direction of turning. For a continuously differentiable planar trajectory, its accumulated value relative to $t_0$ is the [line integral](line-integral.md)

$$
A(t)-A(t_0)=\frac12\int_{t_0}^t\mathbf n\cdot(\mathbf r(s)\times\dot{\mathbf r}(s))\,ds.
$$

A short segment contributes the oriented [triangle](triangle.md) [area](surface-area.md) $\tfrac12\mathbf n\cdot(\mathbf r\times d\mathbf r)$; taking its [time](time-in-physics.md) [derivative](derivative.md) gives [areal velocity](areal-velocity.md). Repeated turns count repeated [area](surface-area.md); a reversal subtracts it. Thus this quantity need not equal the [area](surface-area.md) of the union of all previously swept regions. The origin matters: the relevant origin for [Kepler's second law](kepler-s-second-law.md) is the attracting focus of the [ellipse](ellipse.md), rather than its geometric centre.

## ↑ Ancestors (7)

1. [Areal velocity](areal-velocity.md)
2. [Angular momentum](angular-momentum.md)
3. [Momentum](momentum.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Areal velocity](areal-velocity.md)
