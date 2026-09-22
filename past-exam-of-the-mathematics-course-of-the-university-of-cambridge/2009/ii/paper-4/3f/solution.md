<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Let $C$ be the middle-third [Cantor set](../../../../../cantor-set.md) and choose a positive integer $d$ with $d\log2/\log3\ge k$; this is possible for every real $k$, including negative $k$. Set $X=C^d\subset\mathbb R^d$. It is closed and bounded since each factor is compact. If a subset of $X$ is connected, each coordinate projection is a [connected subset](../../../../../connected-subset.md) of $C$ and hence a singleton; therefore the subset itself is a singleton. Thus $X$ is [totally disconnected](../../../../../totally-disconnected-space.md).

For completeness, the dimension of these [Cartesian powers of the Cantor set](../../../../../cartesian-powers-of-the-cantor-set.md) can be checked directly. At stage $n$ there are $2^{dn}$ cubes of side $3^{-n}$, giving vanishing $s$-dimensional cover cost whenever $s>d\log2/\log3$. Conversely put independent equiprobable zero-or-two ternary digits on every coordinate. Each stage-$n$ cube has probability $2^{-dn}$. If $3^{-n}\le r<3^{-n+1}$, a Euclidean ball of radius $r$ meets at most a constant depending on $d$ such cubes. Hence its probability is at most $C_dr^{d\log2/\log3}$. For any sufficiently fine cover, summing this bound over covering sets shows that its cost at exponent $d\log2/\log3$ is bounded below by a positive constant, since total probability is one. These upper and lower [Hausdorff measure](../../../../../hausdorff-measure.md) bounds prove

$$
\boxed{\dim_HX=d\frac{\log2}{\log3}\ge k.}
$$

The construction does not claim arbitrarily large [Hausdorff dimension](../../../../../hausdorff-dimension.md) in one fixed ambient Euclidean dimension.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
