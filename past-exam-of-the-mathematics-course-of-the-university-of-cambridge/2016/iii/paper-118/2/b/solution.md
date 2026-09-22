<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The real coordinate functions are real and imaginary parts of the [holomorphic coordinates](../../../../../../holomorphic-coordinate.md) $z_j$. Part (a), together with the real coefficients of the [Laplace-Beltrami operator](../../../../../../laplace-beltrami-operator.md), therefore shows that every $x_l$ is a [harmonic function](../../../../../../harmonic-function.md). For the given divergence-of-gradient convention, applying the operator to $x_l$ gives

$$
0=\Delta_dx_l=\frac1{\sqrt{\det g}}\sum_{k=1}^{2n}\frac{\partial}{\partial x_k}\left(\sqrt{\det g}\,g^{kl}\right).
$$

These are the [harmonic coordinate](../../../../../../harmonic-coordinate.md) identities. Expanding the operator on an arbitrary smooth function now gives

$$
\Delta_du=\sum_{k,l=1}^{2n}g^{kl}\frac{\partial^2u}{\partial x_k\partial x_l}
+\sum_{l=1}^{2n}\left[\frac1{\sqrt{\det g}}\sum_{k=1}^{2n}\frac{\partial}{\partial x_k}\left(\sqrt{\det g}\,g^{kl}\right)\right]\frac{\partial u}{\partial x_l}.
$$

The bracketed coefficients vanish. Hence **there is no first-derivative term in these coordinates**:

$$
\boxed{\Delta_du=\sum_{k,l=1}^{2n}g^{kl}\frac{\partial^2u}{\partial x_k\partial x_l}.}
$$

The reason is that the real components of [holomorphic coordinates](../../../../../../holomorphic-coordinate.md) are [harmonic coordinates](../../../../../../harmonic-coordinate.md) for a [Kähler metric](../../../../../../kahler-metric.md); a general real coordinate change need not retain this simplification.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
