<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [intrinsic boundary of a simply connected domain](../../../../../../intrinsic-boundary-of-a-simply-connected-domain.md), so different approaches to the two sides of a slit remain distinct. The [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) $g_K$ extends as a [homeomorphism](../../../../../../homeomorphism.md) from this intrinsic compactification to that of the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). Set $T=T(H)$. The imaginary coordinate of [planar Brownian motion](../../../../../../planar-brownian-motion.md) hits zero in finite time almost surely, and $T$ is no larger than that time. Thus $T<\infty$ and continuity gives a finite Euclidean exit point.

By [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md), $g_K(B_t)$ is a [planar Brownian motion](../../../../../../planar-brownian-motion.md) in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md), run with clock

$$
A(t)=\int_0^t|g_K'(B_s)|^2\,ds.
$$

The terminal clock cannot be infinite: that would make the transformed Brownian motion stay in the upper half-plane forever. It cannot stop while the transformed path is in the interior either, since continuity of $g_K^{-1}$ would then put the original exit point inside $H$. Hence the terminal clock is precisely the transformed [Brownian exit time](../../../../../../brownian-exit-time.md). The transformed path converges to a real boundary point, and applying the extended inverse proves **almost sure convergence to a point of the intrinsic boundary**.

Write $g_K(x+iy)=u+iv$, and let $E=g_K(S)\cap\mathbb R$. The point at infinity has zero [harmonic measure](../../../../../../harmonic-measure.md). [Conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) and the [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md) give

$$
\mathbb P_{x+iy}(\widehat B_T\in S)
=\int_E\frac{v}{\pi((t-u)^2+v^2)}\,dt.
$$

The [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md) gives $g_K(z)=z+O(1/z)$, so along the specified approach $v/y\to1$ and $u/y\to0$. For each fixed real $t$,

$$
\frac{yv}{(t-u)^2+v^2}\longrightarrow1,
\qquad
0\le\frac{yv}{(t-u)^2+v^2}\le\frac yv.
$$

If $\operatorname{Leb}(E)<\infty$, [dominated convergence](../../../../../../dominated-convergence-theorem.md) applies because $y/v$ is eventually bounded. If $\operatorname{Leb}(E)=\infty$, [Fatou's lemma](../../../../../../fatou-s-lemma.md) makes the limit infinite. This proves the [harmonic-measure asymptotic at infinity](../../../../../../harmonic-measure-asymptotic-at-infinity.md)

$$
\boxed{\lim_{y\to\infty,\ x/y\to0}
\pi y\,\mathbb P_{x+iy}(\widehat B_T\in S)
=\operatorname{Leb}(g_K(S)),}
$$

with the equality understood in the extended nonnegative reals.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
