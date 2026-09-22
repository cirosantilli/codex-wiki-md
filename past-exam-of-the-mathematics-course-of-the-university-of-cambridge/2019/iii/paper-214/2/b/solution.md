<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [Tonelli theorem](../../../../../../tonelli-theorem.md),

$$
\chi(p)=\mathbb E_p|\mathcal C|
=\sum_{x\in\mathbb Z^d}\mathbb P_p(0\leftrightarrow x).
$$

If $p<p_c$, part (a) bounds the summand by $e^{-c\lVert x\rVert_\infty}$. There are only polynomially many vertices at each radius, so the series converges and $\chi(p)<\infty$.

Conversely, suppose $\chi(p)<\infty$. Then $p<1$. Choose $q>p$ so close to $p$ that

$$
2d\,\frac{q-p}{1-p}\,\chi(p)<1.
$$

Use the standard [sprinkling coupling for Bernoulli percolation](../../../../../../sprinkling-coupling-for-bernoulli-percolation.md): first expose the $p$-open clusters, then independently open each remaining edge with probability $\alpha=(q-p)/(1-p)$. Explore the $q$-cluster of the origin cluster by following sprinkled edges. Each discovered $p$-cluster has at most $2d$ times its number of vertices as many incident edges, so the exploration is dominated by a [Galton-Watson process](../../../../../../galton-watson-process.md) of mean at most $2d\alpha\chi(p)<1$. This process dies out almost surely, and hence there is no infinite $q$-open cluster. Thus $q\leq p_c$, and $p<q$ implies $p<p_c$. Therefore

$$
\boxed{\chi(p)<\infty\iff p<p_c.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
