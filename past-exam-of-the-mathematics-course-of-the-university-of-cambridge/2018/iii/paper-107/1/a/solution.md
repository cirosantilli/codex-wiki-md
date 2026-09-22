<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the spherical average $M(r)$, rescaling the sphere and applying the [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
M(r)=\frac1{n\omega_n}\int_{S^{n-1}}u(y+r\theta)\,dS_\theta,\qquad
M'(r)=\frac1{n\omega_n r^{n-1}}\int_{\partial B_r(y)}\partial_\nu u
=\frac1{n\omega_n r^{n-1}}\int_{B_r(y)}\Delta u=0.
$$

By [continuity](../../../../../../continuous-function.md), $M(r)\to u(y)$ as $r\downarrow0$. Integrating these spherical averages in radius proves the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md):

$$
\boxed{u(y)=\frac1{n\omega_n r^{n-1}}\int_{\partial B_r(y)}u
=\frac1{\omega_n r^n}\int_{B_r(y)}u.}
$$

For the [strong maximum principle for harmonic functions](../../../../../../strong-maximum-principle-for-harmonic-functions.md), suppose an interior point attains the maximum $m$ on a connected domain. The continuous nonnegative function $m-u$ has zero average on each sufficiently small ball around that point, so it vanishes there. The maximum set is therefore open as well as closed, and [connectedness](../../../../../../connected-space.md) makes it the entire domain. Apply the same argument to $-u$ for a minimum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
