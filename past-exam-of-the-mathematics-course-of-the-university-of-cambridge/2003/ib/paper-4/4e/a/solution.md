<h1 id="4e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Morera's theorem](../../../../../../morera-s-theorem.md) states that a continuous complex-valued function on an open set is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) if its integral around every triangle whose closed interior lies in the set is zero. It is enough to impose this condition locally on disks.

Fix a [disk](../../../../../../disk-mathematics.md) $B$ contained in the open set and a base point $z_0\in B$. Define $F(z)$ as the integral of $f$ along the straight segment from $z_0$ to $z$. The zero triangle integral gives, for sufficiently small $h$,

$$
F(z+h)-F(z)=\int_{[z,z+h]}f(w)\,dw
=h\int_0^1 f(z+th)\,dt.
$$

[Continuity](../../../../../../continuous-function.md) makes the quotient by $h$ tend to $f(z)$, so $F$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) and $F'=f$. To justify that its derivative is [holomorphic](../../../../../../complex-differentiability-at-a-point.md), apply the [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) for $F$ on a smaller [circle](../../../../../../circle.md):

$$
F'(z)=\frac1{2\pi i}\int_{\Gamma}\frac{F(w)}{(w-z)^2}\,dw.
$$

The right side may be differentiated again inside the [circle](../../../../../../circle.md) because its denominator stays uniformly away from zero on the [contour](../../../../../../complex-integration-contour.md). Thus $F'=f$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on $B$. Such disks cover the open set, proving the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4E](../../4e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
