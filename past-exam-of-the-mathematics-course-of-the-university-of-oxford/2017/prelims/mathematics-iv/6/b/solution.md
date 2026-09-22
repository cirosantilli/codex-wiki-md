<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

The [linearization](../../../../../../linearization.md) at rest at $r=0$ is

$$
\ddot r=\left(\omega^2-\frac ga\right)r.
$$

For $\omega^2<g/a$, small disturbances oscillate. To verify nonlinear [stability](../../../../../../stability-of-a-numerical-method.md), multiply the full [equation of motion](../../../../../../equation-of-motion.md) by $\dot r/a^2$ and integrate to obtain the [first integral](../../../../../../first-integral.md)

$$
J=\frac12\left(1+\frac{r^2}{a^2}\right)\dot r^2+\frac12\left(\frac ga-\omega^2\right)r^2.
$$

For $\omega^2<g/a$, $J$ is positive away from the [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) in a sufficiently small [neighborhood](../../../../../../neighbourhood-mathematics.md) of $(r,\dot r)=(0,0)$; its small [level sets](../../../../../../level-set.md) confine the motion. Thus

$$
\boxed{r=0\text{ is stable if }\omega^2<g/a,\text{ and unstable if }\omega^2>g/a.}
$$

At equality, every resting location on the wire is an [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md), so a displacement at zero relative [velocity](../../../../../../velocity.md) simply remains there: the equilibrium is **neutral with respect to resting displacements**. It is **unstable with respect to general perturbations in [phase space](../../../../../../phase-space.md)**, however. An arbitrarily small outward initial [velocity](../../../../../../velocity.md) $v_0>0$ gives $\dot r=v_0/\sqrt{1+r^2/a^2}>0$ from the [first integral](../../../../../../first-integral.md), eventually taking the bead outside any prescribed small [neighborhood](../../../../../../neighbourhood-mathematics.md). Thus strict [phase space](../../../../../../phase-space.md) [stability](../../../../../../stability-of-a-numerical-method.md) holds only for $\omega^2<g/a$.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [6](../../6.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
