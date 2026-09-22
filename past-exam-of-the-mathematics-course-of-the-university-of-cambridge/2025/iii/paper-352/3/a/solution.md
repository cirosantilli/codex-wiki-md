<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At the final state of the [slump test for yield stress](../../../../../../slump-test-for-yield-stress.md), an axisymmetric deposit of height $h(r)$ is just able to support itself. [Hydrostatic pressure](../../../../../../hydrostatic-pressure.md) gives radial pressure gradient $\rho g h'(r)$, while [lubrication theory](../../../../../../lubrication-theory.md) makes the magnitude of the basal [shear stress](../../../../../../shear-stress.md)

$$
|\tau_b|=\rho g h\,|h'|.
$$

The marginally yielded final profile therefore satisfies

$$
\rho g h(-h')=\tau_y,
\qquad h(R)=0.
$$

Integration gives

$$
\boxed{
h(r)=\left[\frac{2\tau_y}{\rho g}(R-r)\right]^{1/2}}.
$$

Using [mass conservation](../../../../../../mass-conservation.md), the known volume is

$$
V=2\pi\int_0^Rrh(r)\,dr
=\frac{8\pi}{15}
\left(\frac{2\tau_y}{\rho g}\right)^{1/2}R^{5/2}.
$$

Solving for the yield stress produces the estimate

$$
\boxed{\tau_y=\frac{225\,\rho gV^2}{128\pi^2R^5}}.
$$

Thus one measures the final radius $R$ and inserts it with $V$ and $\rho$. The estimate assumes a thin deposit, negligible [surface tension](../../../../../../surface-tension.md), complete initial yielding, and a spatially uniform yield stress.

Dry sand is a [granular material](../../../../../../granular-material.md) governed primarily by frictional stability. Its final free surface reaches the [angle of repose](../../../../../../angle-of-repose.md) $\theta_r$, so the deposit is approximately a cone,

$$
\boxed{h(r)=(R-r)\tan\theta_r}.
$$

This constant-slope profile differs from the square-root edge of the yield-stress-fluid model.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
