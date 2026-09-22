<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $G=c=1$, select the retarded source field with no added homogeneous radiation, and work to leading order in the [weak-field approximation](../../../../../../weak-field-approximation.md) and [long-wavelength source approximation](../../../../../../long-wavelength-source-approximation.md). The [retarded fundamental solution](../../../../../../retarded-fundamental-solution.md) of the [Linearized Einstein equations](../../../../../../linearized-einstein-equations.md) in [Lorenz gauge in linearized gravity](../../../../../../lorenz-gauge-in-linearized-gravity.md) is

$$
\bar h_{ij}(t,\mathbf x)=4\int\frac{T_{ij}(t-|\mathbf x-\mathbf x'|,\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x'.
$$

For $r\gg d$, the denominator is $r$ to leading order. The delay is $t-r+\mathbf n\cdot\mathbf x'+O(d^2/r)$, where $\mathbf n=\mathbf x/r$. In the usual slowly evolving source regime, its characteristic time $\tau$ obeys $d/\tau\ll1$, so the source-size part of the delay is negligible:

$$
\bar h_{ij}(t,\mathbf x)\simeq\frac4r\int T_{ij}(t-r,\mathbf x')\,d^3x'.
$$

The [stress-energy conservation](../../../../../../stress-energy-conservation.md) equation $\partial_\mu T^{\mu\nu}=0$ is required at the approximation order used; it follows from the divergence of the gauge-fixed field equation. [Compact support](../../../../../../compact-support.md) removes the [integration by parts](../../../../../../integration-by-parts.md) surface terms. Since $T^{00}=T_{00}$ and $T^{ij}=T_{ij}$ in this signature,

$$
\dot I_{ij}=\int(T^{0i}x^j+T^{0j}x^i)\,d^3x,
\qquad
\ddot I_{ij}=\int(T^{ji}+T^{ij})\,d^3x=2\int T_{ij}\,d^3x.
$$

Combining these identities gives the [retarded quadrupole field](../../../../../../retarded-quadrupole-field.md)

$$
\boxed{\bar h_{ij}(t,\mathbf x)\simeq\frac2r\ddot I_{ij}(t-r).}
$$

For an ordinary nonrelativistic bound source, $\tau\sim d/v$ makes $d/\tau\sim v\ll1$. More generally the size relative to the variation timescale must also be small; speed alone does not exclude a rapidly varying small-amplitude motion.

The [radiation boundary condition for linearized gravity](../../../../../../radiation-boundary-condition-for-linearized-gravity.md) is essential for a statement about the full field. Without it, the displayed implication is false: take $T_{\mu\nu}=0$ and add $\bar h_{11}=A\cos(k(t-z))$, $\bar h_{22}=-\bar h_{11}$, all other components zero. This weak plane [gravitational wave](../../../../../../gravitational-wave.md) satisfies both the homogeneous wave equation and [Lorenz gauge in linearized gravity](../../../../../../lorenz-gauge-in-linearized-gravity.md), while every $I_{ij}$ is zero. The proved formula is for the retarded source contribution, with the standard slow-source qualification. Its transverse–traceless projection gives the physical radiative strain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
