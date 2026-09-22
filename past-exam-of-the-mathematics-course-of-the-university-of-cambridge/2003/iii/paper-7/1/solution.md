<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a nonempty [bounded set](../../../../../bounded-set.md), let $N_\delta(E)$ be the least number of radius-$\delta$ balls covering $E$. The lower and upper [Minkowski dimensions](../../../../../box-counting-dimension.md) are respectively

$$
\underline{\dim}_{\mathrm M}E=\liminf_{\delta\downarrow0}\frac{\log N_\delta(E)}{\log(1/\delta)},\qquad\overline{\dim}_{\mathrm M}E=\limsup_{\delta\downarrow0}\frac{\log N_\delta(E)}{\log(1/\delta)}.
$$

Using comparable cubes or ball diameters gives the same limits. For an unbounded set one must specify a local or bounded-piece convention; these are the usual bounded-set definitions used in the [Kakeya set](../../../../../kakeya-set.md) problem.

For the digit set, fixing the first $k$ digits gives exactly $3^k$ cylinders in intervals of length $9^{-k}$. They cover the set with at most $3^k$ balls of comparable radius. Their base-nine prefix integers are separated by at least two, so these containing intervals have gaps at least $9^{-k}$. Choosing one point in each cylinder shows that a radius-$9^{-k}$ ball meets at most a bounded number of chosen points. Hence $N_{9^{-k}}(Q)\asymp3^k$. For $9^{-(k+1)}<\delta\leq9^{-k}$, monotonicity sandwiches the [covering number](../../../../../metric-covering-number.md) between constant multiples of $3^k$ and $3^{k+1}$. This proves the [box-counting dimension of separated digit sets](../../../../../box-counting-dimension-of-separated-digit-sets.md) formula here:

$$
\boxed{\underline{\dim}_{\mathrm M}Q=\overline{\dim}_{\mathrm M}Q=\frac{\log3}{\log9}=\frac12.}
$$

A planar [Besicovitch set](../../../../../besicovitch-set.md) is a [bounded set](../../../../../bounded-set.md) of zero [Lebesgue measure](../../../../../lebesgue-measure.md) containing a unit line segment in every unoriented direction. The following proof in fact applies to every bounded planar [Kakeya set](../../../../../kakeya-set.md), whether its area is zero or positive.

Choose $M\asymp\delta^{-1}$ directions equally spaced in an angular interval of length, say, $\pi/2$, and one segment of the set in each direction. Let $T_j$ be its rectangle of length one and width comparable to $\delta$, lying in the $C\delta$ neighborhood $E_{C\delta}$. Put $F=\sum_j1_{T_j}$. Then $\int F\asymp M\delta\asymp1$. Two such [Kakeya tubes](../../../../../kakeya-tube.md) at angle $\alpha$ have overlap at most $C\delta^2/\alpha$, since the intersection of their supporting strips is a parallelogram of that area. The trivial bound $C\delta$ applies for nearly parallel tubes. Thus, uniformly over their translations,

$$
|T_j\cap T_k|\leq\frac{C\delta^2}{\delta+\alpha_{jk}}\lesssim\frac{\delta}{1+|j-k|}.
$$

Sum these intersections. Each row contributes at most $C\delta\log(2/\delta)$, so $\int F^2\lesssim\log(2/\delta)$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on the union now gives the [planar Kakeya neighborhood lower bound](../../../../../planar-kakeya-neighborhood-lower-bound.md)

$$
|E_{C\delta}|\geq\left|\bigcup T_j\right|\geq\frac{(\int F)^2}{\int F^2}\gtrsim\frac1{\log(2/\delta)}.
$$

A cover of $E$ by $N_\delta(E)$ radius-$\delta$ balls covers $E_{C\delta}$ by their fixed-factor enlargements. Hence $N_\delta(E)\gtrsim\delta^{-2}/\log(2/\delta)$. Boundedness gives the matching upper exponent $N_\delta(E)\lesssim_E\delta^{-2}$. Taking the lower and upper limits proves

$$
\boxed{\underline{\dim}_{\mathrm M}E=\overline{\dim}_{\mathrm M}E=2.}
$$

The logarithmic neighborhood loss is compatible with zero area; it still forces full dimension.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
