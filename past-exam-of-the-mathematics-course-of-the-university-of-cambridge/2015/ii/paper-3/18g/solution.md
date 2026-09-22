<h1 id="18g/solution">Solution</h1>

↑ **Parent:** [18G](../18g.md)

The [Baire category theorem](../../../../../baire-category-theorem.md) in the needed version states that a nonempty complete [metric space](../../../../../metric-space.md) cannot be a countable union of closed sets with empty interior. To prove it, suppose $F_1,F_2,\ldots$ are such sets and start with a nonempty open set $U$. Inductively choose closed balls $\overline B_j$ of positive radius at most $2^{-j}$, with $\overline B_1\subset U\setminus F_1$ and $\overline B_{j+1}\subset B_j\setminus F_{j+1}$. This is possible because each complement is open and dense. The centres form a [Cauchy sequence](../../../../../cauchy-sequence.md); completeness supplies a limit in every closed ball. It lies in $U$ and outside every $F_j$, proving the theorem.

Here the sequence spaces are over the real scalars, as required by the Euclidean-plane assertion. Suppose an [isometry](../../../../../isometry.md) $\varphi:\mathbb R^2\to c_0$ existed. On the compact complete space $S^1\times S^1$, the sets

$$
F_n=\{(x,y):|\varphi_n(x)-\varphi_n(y)|=\|x-y\|_2\}
$$

are closed. They cover that space: for a nonzero sequence in $c_0$, the [supremum norm](../../../../../supremum-norm.md) is attained at a coordinate; for $x=y$ every coordinate works. By the [Baire category theorem](../../../../../baire-category-theorem.md), one $F_n$ contains a product of open arcs. Shrink the arcs to be disjoint. The real coordinate difference is then continuous and nonzero, so its sign is constant on the product. Thus the chord distance has the separated form

$$
\|x-y\|_2=\pm(\varphi_n(x)-\varphi_n(y)).
$$

In particular its alternating sum on every four-point rectangle is zero. Parametrize the arcs by angles $s,t$ with $0<t-s<2\pi$. Their chord distance is $D(s,t)=2\sin((t-s)/2)$, whose mixed derivative is

$$
\partial_s\partial_tD=\tfrac12\sin((t-s)/2)>0.
$$

The zero rectangle identity would force this mixed derivative to vanish, a contradiction. Therefore **no such isometry exists**.

For a real vector $x\in\ell_1^n$, list its signed sums over all $2^n$ choices $\varepsilon\in\{-1,1\}^n$, followed by infinitely many zero coordinates:

$$
Tx=(\varepsilon\cdot x)_{\varepsilon\in\{-1,1\}^n}\oplus(0,0,\ldots).
$$

This is linear, has finite support and lies in $c_0$. Choosing the signs of the components gives $\max_\varepsilon|\varepsilon\cdot x|=\sum_j|x_j|$. Thus **$\boxed{\|Tx\|_\infty=\|x\|_1}$**, the required linear isometry.

## ↑ Ancestors (10)

1. [18G](../18g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
