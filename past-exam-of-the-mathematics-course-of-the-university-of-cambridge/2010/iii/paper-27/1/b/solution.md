<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the following standard [planar Brownian motion](../../../../../../planar-brownian-motion.md) facts: its exit [probability distribution](../../../../../../probability-distribution.md) is [harmonic measure](../../../../../../harmonic-measure.md); [conformal maps](../../../../../../conformal-map.md) preserve that [probability distribution](../../../../../../probability-distribution.md) after an increasing time change; and the [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md) gives its real-boundary exit density. For rough hulls the [boundary](../../../../../../boundary-of-a-set.md) is interpreted through [prime ends](../../../../../../prime-end.md), with [boundary](../../../../../../boundary-of-a-set.md) correspondence at harmonic-measure-almost every exit point. This avoids imposing a smoothness or local-connectedness assumption on $K$.

Under $g_K$, the exit event through $K$ corresponds to a measurable set $E_K\subset\mathbb R$ of [boundary](../../../../../../boundary-of-a-set.md) images. It is bounded: the [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) extends by [Schwarz reflection](../../../../../../schwarz-reflection-principle.md) along the real line outside a sufficiently large interval enclosing $K$, and its [boundary](../../../../../../boundary-of-a-set.md) near infinity corresponds to the original real [boundary](../../../../../../boundary-of-a-set.md) near infinity. All [prime ends](../../../../../../prime-end.md) representing $K$ therefore have images in a bounded interval. The [boundary](../../../../../../boundary-of-a-set.md) correspondence assertion can equivalently be formulated using the almost-everywhere limits of $g_K^{-1}$; changing null sets does not change $E_K$'s measure.

Write $g_K(iy)=u_y+iv_y$. The [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md) gives $u_y=O(y^{-2})$ and $v_y=y-a_K/y+O(y^{-2})$. By [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) and the [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md),

$$
\mathbb P_{iy}(B_T\in K)=\frac1\pi\int_{E_K}\frac{v_y}{(s-u_y)^2+v_y^2}\,ds.
$$

On the bounded set $E_K$, the integrand multiplied by $y$ tends uniformly to one. Therefore the limit exists and is finite:

$$
\boxed{c(K)=\frac{|E_K|}{\pi}.}
$$

This is the [harmonic capacity from infinity in the upper half-plane](../../../../../../harmonic-capacity-from-infinity-in-the-upper-half-plane.md) with the normalization $c(K)=\operatorname{cap}(K)/\pi$; it is different from [half-plane capacity](../../../../../../half-plane-capacity.md). If real [boundary](../../../../../../boundary-of-a-set.md) points are retained in the definition of $K$, include their [boundary](../../../../../../boundary-of-a-set.md) images in $E_K$ as well; the argument is unchanged.

For the scaling statement, [Brownian scaling](../../../../../../brownian-scaling.md) says that $r^{-1}B_{r^2t}$ started from $iy/r$ is again standard [planar Brownian motion](../../../../../../planar-brownian-motion.md). The exit event scales with the hull, so

$$
\mathbb P_{iy}(B_T\in rK)
=\mathbb P_{i(y/r)}(B_T\in K).
$$

Set $v=y/r$, multiply by $y=rv$ and take the limit. It follows that

$$
\boxed{c(rK)=r\,c(K).}
$$

The same conclusion follows geometrically from $E_{rK}=rE_K$ and the formula above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
