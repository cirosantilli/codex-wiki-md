<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First derive the [Brownian representation of half-plane capacity](../../../../../../brownian-representation-of-half-plane-capacity.md) with the chosen normalization. Set

$$
h(z)=\operatorname{Im}(z-g_K(z)),\qquad z\in\mathbb H\setminus K.
$$

The height comparison from part (a), applied to $f_K=g_K^{-1}$, gives $h\geq0$. On the [boundary](../../../../../../boundary-of-a-set.md), $\operatorname{Im}g_K$ tends to zero; on $K$ the limiting value of $h$ is therefore $\operatorname{Im}z$, and on the real [boundary](../../../../../../boundary-of-a-set.md) it is zero. To see the asserted boundary-height limit without assuming a smooth hull, suppose a bounded sequence approaching the [boundary](../../../../../../boundary-of-a-set.md) had mapped images with imaginary part bounded away from zero. The inverse's expansion near infinity prevents these images from being unbounded, and an interior subsequential limit would map back to an interior point of $D$, a contradiction.

At infinity $h$ tends to zero by the [Laurent series](../../../../../../laurent-series.md). The [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md) now bounds $h$ between zero and $R=\operatorname{rad}(K)$, since every point of $K$ has imaginary part at most $R$. Apply the [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to the bounded [harmonic function](../../../../../../harmonic-function.md) $h(B_{t\wedge T})$. The exit time $T$ is almost surely finite because it is no larger than the first time the imaginary coordinate of [planar Brownian motion](../../../../../../planar-brownian-motion.md) reaches zero. Taking $t\to\infty$ gives

$$
h(z)=\mathbb E_z[\operatorname{Im}B_T].
$$

This uses the bounded harmonic difference, not optional sampling of the unbounded imaginary coordinate at an unbounded [stopping time](../../../../../../stopping-time.md).

At $z=iy$, the expansion gives $yh(iy)\to a_K$. Since

$$
0\leq\operatorname{Im}B_T\leq R\,\mathbf1_{\{B_T\in K\}},
$$

we obtain

$$
\boxed{\operatorname{hcap}(K)=\lim_{y\to\infty}y\mathbb E_{iy}[\operatorname{Im}B_T]
\leq\operatorname{rad}(K)c(K).}
$$

Thus the quadratic [half-plane capacity](../../../../../../half-plane-capacity.md) is controlled by a length times the linearly scaling [harmonic capacity from infinity in the upper half-plane](../../../../../../harmonic-capacity-from-infinity-in-the-upper-half-plane.md). The factor $1/\pi$ is essential if the alternative normalization $\operatorname{cap}(K)=\pi c(K)$ is used.

## ↑ Ancestors (11)

1. [C](../c.md)
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
