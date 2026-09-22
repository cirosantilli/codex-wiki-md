<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the constant-density model, $m(r)=4\pi\rho r^3/3=Mr^3/R^3$. This is the incompressible [Interior Schwarzschild metric](../../../../../../../interior-schwarzschild-metric.md), replacing the earlier finite-slope [barotropic stellar equation of state](../../../../../../../barotropic-stellar-equation-of-state.md). The [Tolman–Oppenheimer–Volkoff equation](../../../../../../../tolman-oppenheimer-volkoff-equation.md) separates as

$$
\frac{dp}{(p+\rho)(p+\rho/3)}=-\frac{4\pi r\,dr}{1-8\pi\rho r^2/3}.
$$

On the left, partial fractions give

$$
\int\frac{dp}{(p+\rho)(p+\rho/3)}=\frac{3}{2\rho}\log\frac{p+\rho/3}{p+\rho}.
$$

On the right the antiderivative is $\tfrac3{4\rho}\log(1-8\pi\rho r^2/3)$. Applying the surface condition $p(R)=0$, and writing $s(r)=\sqrt{1-2Mr^2/R^3}$, $s_R=\sqrt{1-2M/R}$, gives

$$
\frac{p+\rho/3}{p+\rho}=\frac{s(r)}{3s_R}.
$$

Solving for the [pressure](../../../../../../../pressure.md) recovers the [Interior Schwarzschild solution](../../../../../../../interior-schwarzschild-metric.md):

$$
p(r)=\rho\frac{s(r)-s_R}{3s_R-s(r)}.
$$

In particular the [central pressure of a constant-density relativistic star](../../../../../../../central-pressure-of-a-constant-density-relativistic-star.md) is

$$
\boxed{p_c=\rho\frac{1-\sqrt{1-2M/R}}{3\sqrt{1-2M/R}-1}.}
$$

The denominator must be positive for a regular positive-pressure centre, requiring $M/R<4/9$. As that limiting compactness is approached, the central [pressure](../../../../../../../pressure.md) diverges, in agreement with [Buchdahl's theorem](../../../../../../../buchdahl-s-theorem.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 54](../../../../paper-54-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
