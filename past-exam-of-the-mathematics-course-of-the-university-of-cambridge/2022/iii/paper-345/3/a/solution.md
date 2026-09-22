<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\widehat\rho(z)$ for the ambient density far from the wall and $\rho(z)$ for the density at the wall. Across the plume, let $y=x/b$ and use the prescribed triangular profiles

$$
w=W(1-y),
\qquad
\rho_p=\widehat\rho-(\widehat\rho-\rho)(1-y),
\qquad 0\leq y\leq1.
$$

Direct integration gives the [volume flux](../../../../../../volumetric-flow-rate.md), [mass flux](../../../../../../mass-flux.md), [momentum flux](../../../../../../momentum-flux.md), and density-weighted [buoyancy flux](../../../../../../buoyancy-flux.md), all per unit radiator length:

$$
\boxed{V=\int_0^b w\,dx=\frac{bW}{2},}
$$



$$
\boxed{Q=\int_0^b\rho_pw\,dx
=\frac{bW}{6}(\widehat\rho+2\rho),}
$$



$$
\boxed{M=\int_0^b\rho_pw^2\,dx
=\frac{bW^2}{12}(\widehat\rho+3\rho),}
$$



$$
\boxed{F=\int_0^b g(\widehat\rho-\rho_p)w\,dx
=\frac{gbW}{3}(\widehat\rho-\rho).}
$$

These coefficients distinguish the [triangular-profile wall line plume](../../../../../../triangular-profile-wall-line-plume.md) from a [top-hat plume model](../../../../../../top-hat-plume-model.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
