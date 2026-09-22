# Point-vortex drift under a conformal map

↑ **Parent:** [Line vortex](line-vortex.md)

Let $\zeta=g(z)$ be a [conformal map](conformal-map.md), and let a [point vortex](line-vortex.md) of [circulation](circulation-physics.md) $\Gamma$ lie at $z=c$. Suppose the mapped [complex potential of a two-dimensional potential flow](complex-potential-of-a-two-dimensional-potential-flow.md) is

$$
W(\zeta)=\frac\Gamma{2\pi i}\log(\zeta-g(c))+R(\zeta),
$$

where $R$ is a [holomorphic function](holomorphic-function-split.md) near $g(c)$ and represents the other [point vortices](line-vortex.md), boundaries, and any imposed flow. The physical [complex velocity](complex-velocity.md) is $w'=g'W'$. The [point vortex](line-vortex.md) follows its regular [velocity](velocity.md), found by removing $\Gamma/[2\pi i(z-c)]$ before taking the limit. A [Taylor expansion](taylor-expansion.md) proves

$$
\frac{g'(z)}{g(z)-g(c)}=\frac1{z-c}+\frac{g''(c)}{2g'(c)}+O(z-c),
$$

which gives the title formula. The [complex conjugate](complex-conjugate.md) occurs because the [complex velocity](complex-velocity.md) convention is $w'=u-iv$, whereas $\dot c=u+iv$.

For a mapped [upper half-plane](upper-half-plane-complex-analysis.md) with no imposed flow, the [method of images](method-of-images.md) gives $R(\zeta)=-\Gamma\log(\zeta-\overline{g(c)})/(2\pi i)$, hence

$$
\overline{\dot c}=\frac\Gamma{2\pi i}
\left[\frac{g''(c)}{2g'(c)}-\frac{g'(c)}{g(c)-\overline{g(c)}}\right].
$$

The first term is essential: excluding a mapped singularity and then transforming its regular [velocity](velocity.md) does not in general equal subtracting the physical singularity after transformation.

## ↑ Ancestors (7)

1. [Line vortex](line-vortex.md)
2. [Vortex (fluid mechanics)](vortex-fluid-mechanics.md)
3. [Vorticity](vorticity-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-fluids-and-waves-course-of-the-university-of-oxford/2021/2/c/ii/solution.md)
