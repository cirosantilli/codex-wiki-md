<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

For $s\ge0$ and $\delta>0$, define the [scale-restricted Hausdorff content](../../../../../scale-restricted-hausdorff-content.md) at scale $\delta$ by

$$
\mathcal H_\delta^s(F)=\inf\left\{\sum_j(\operatorname{diam}U_j)^s:
F\subset\bigcup_jU_j,\ \operatorname{diam}U_j\le\delta\right\},
$$

using countable covers. The [Hausdorff measure](../../../../../hausdorff-measure.md) is $\mathcal H^s(F)=\lim_{\delta\downarrow0}\mathcal H_\delta^s(F)$; the limit exists by monotonicity. A conventional dimension-dependent normalizing constant does not change the [Hausdorff dimension](../../../../../hausdorff-dimension.md)

$$
\dim_HF=\inf\{s:\mathcal H^s(F)=0\}
=\sup\{s:\mathcal H^s(F)=\infty\}.
$$

At $s=0$, a nonempty singleton has contribution one, so the measure counts points.

Let $\mathcal T(K)=\bigcup_{i=1}^kS_i(K)$ and $c=\max_i c_i<1$. For [compact](../../../../../compact-space.md) nonempty $K,L$, matching a point of $S_i(K)$ with the image of a nearby point of $L$ gives $d_H(\mathcal T K,\mathcal T L)\le c\,d_H(K,L)$. Choose a sufficiently large closed ball $B$ with every $S_i(B)\subset B$. The nonempty [compact sets](../../../../../compact-space.md) $\mathcal T^m(B)$ are nested, so their intersection $I$ is nonempty and [compact](../../../../../compact-space.md). The finite union of similarity images commutes with this decreasing [compact](../../../../../compact-space.md) intersection: a point lying in all unions has some repeated branch index, and compactness supplies a preimage in all the nested sets. Consequently $\mathcal T(I)=I$. If $J$ is another invariant [compact set](../../../../../compact-space.md), the contraction estimate gives $d_H(I,J)\le c\,d_H(I,J)$, hence $I=J$. This proves existence and uniqueness of the invariant set of a [finite similarity iterated function system](../../../../../finite-similarity-iterated-function-system.md).

Under the [open set condition](../../../../../open-set-condition.md), there is a nonempty bounded open set $O$ such that the $S_i(O)$ lie inside $O$ and are pairwise disjoint. The dimension formula is

$$
\boxed{\dim_H I=s,\qquad\sum_i c_i^s=1}.
$$

Overlaps can invalidate this formula if that assumption is omitted.

For the printed template, subdivide the central straight run of length two into its two collinear unit steps. The eight directed steps, before dividing all coordinates by four, have successive vertices

$$
(0,0),(1,0),(1,1),(2,1),(2,0),(2,-1),(3,-1),(3,0),(4,0).
$$

Each step defines a similarity with ratio $1/4$, with rotation matching its direction. The open diamond $O=\{|x-1/2|+|y|<1/2\}$ is an explicit witness for the [open set condition](../../../../../open-set-condition.md). Its eight image diamonds have radius $1/8$ in the $\ell^1$ metric, lie in $O$, and their centres have pairwise $\ell^1$ distance at least $1/4$; their interiors are therefore disjoint. The [Minkowski sausage](../../../../../minkowski-sausage.md) dimension is consequently

$$
8(1/4)^s=1,\qquad\boxed{s=\frac32}.
$$

This makes the subdivision convention explicit. If the length-two run were instead treated as one unsplit edge replaced at scale $1/2$, there would be six maps of ratio $1/4$ and one of ratio $1/2$. The same diamond separation works, but the equation becomes $6\,4^{-s}+2^{-s}=1$, giving $s=\log_2 3$, a different fractal. The requested $3/2$ corresponds to the eight-unit-step interpretation.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
