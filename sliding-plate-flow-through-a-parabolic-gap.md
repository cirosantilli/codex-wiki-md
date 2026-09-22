# Sliding-plate flow through a parabolic gap

↑ **Parent:** [Parabolic lubrication gap](parabolic-lubrication-gap.md)

A stationary upper wall $z=h_0+x^2/(2R)$ and a flat lower wall moving at [velocity](velocity.md) $-U$ generate a [Couette-Poiseuille flow](couette-poiseuille-flow.md) in the [lubrication approximation](lubrication-theory.md). Write $L=\sqrt{Rh_0}$, $X=x/L$, $H=1+X^2/2$ and $p=(\mu UL/h_0^2)\Pi$. Equal endpoint [gauge pressures](gauge-pressure.md) give

$$
\Pi(X)=\frac{2X}{H^2},\qquad
Q=-\frac{Uh}{2}-\frac{h^3}{12\mu}\frac{dp}{dx}
=-\frac23Uh_0,
$$

where $Q$ is the signed [volume flux per unit width](volume-flux-per-unit-width.md). To determine its constant value, the [Reynolds equation](reynolds-equation.md) gives $H^3\Pi_X/12+H/2=C$. Integrating $\Pi_X$ over the real line gives $C=I_2/(2I_3)=2/3$, where $I_m=\int_{-\infty}^{\infty}H^{-m}\,dX$ and the substitution $X=\sqrt2\tan\theta$ evaluates the ratio. The [plane Poiseuille flow](plane-poiseuille-flow.md) and [Couette flow](couette-flow.md) contributions both point towards negative $x$ exactly for $|x|<\sqrt{2Rh_0/3}$. This is a full-film model with matched equal outer [pressures](pressure-split.md).

## ↑ Ancestors (7)

1. [Parabolic lubrication gap](parabolic-lubrication-gap.md)
2. [Lubrication theory](lubrication-theory.md)
3. [Viscous fluid flow](viscous-fluid-flow-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-viscous-flow-course-of-the-university-of-oxford/2023/3/c/solution.md)
