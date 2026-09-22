<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The necessary and sufficient condition is

$$
\boxed{ku+\ell v\notin2\pi\mathbb Z\quad\text{for every }(k,\ell)\in\mathbb Z^2\setminus\{(0,0)\}.}
$$

Equivalently, $1,u/(2\pi),v/(2\pi)$ are linearly independent over $\mathbb Q$. This is the [equidistribution criterion for a torus translation](../../../../../../equidistribution-criterion-for-a-torus-translation.md).

For sufficiency, set $w=e^{i(ku+\ell v)}$. For a nonconstant [character](../../../../../../character-of-a-representation.md) of the torus the condition gives $w\ne1$, and the [geometric series](../../../../../../geometric-series.md) formula yields

$$
\left|\frac1n\sum_{r=1}^n e^{ir(ku+\ell v)}\right|=\left|\frac{w(1-w^n)}{n(1-w)}\right|\le\frac2{n|1-w|}\longrightarrow0.
$$

The constant [torus character](../../../../../../characters-of-a-real-torus.md) has average one. Thus orbit averages converge to integrals against normalized [Haar measure](../../../../../../haar-measure.md) for every [trigonometric polynomial](../../../../../../trigonometric-polynomial.md). Part (i) and a uniform approximation bound extend this to every [continuous function](../../../../../../continuous-function.md) $g$: the difference between the orbit average and the integral for $g$ differs from that for an approximating polynomial by at most twice their uniform distance.

For a nonempty half-open rectangle $R$, choose [continuous functions](../../../../../../continuous-function.md) $g_-\le\mathbf1_R\le g_+$ with values in $[0,1]$ and $\int(g_+-g_-)dm$ arbitrarily small. One can take distance cutoffs: $g_-$ vanishes at the boundary and rises to one inside, while $g_+$ is one on the closure and falls to zero outside a thin neighborhood. Their difference is supported in shrinking neighborhoods of the rectangle's finitely many boundary segments, which have [Haar measure](../../../../../../haar-measure.md) zero. Squeezing the orbit averages between the two continuous averages gives the normalized area $m(R)=(b-a)(d-c)/(2\pi)^2$. Empty rectangles are immediate, and full-circle coordinate intervals can be treated with the constant cutoff in that coordinate.

For necessity, if a nonzero pair is resonant, every orbit point lies in the closed set $H=\{(s,t):e^{i(ks+\ell t)}=1\}$. This is a proper subset because the [torus character](../../../../../../characters-of-a-real-torus.md) is nonconstant. Its open complement contains a rectangle of positive area in a coordinate chart, which can be chosen inside the standard coordinate square. That rectangle is never visited, contradicting the required positive limiting frequency. Hence the boxed condition is necessary as well as sufficient.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
