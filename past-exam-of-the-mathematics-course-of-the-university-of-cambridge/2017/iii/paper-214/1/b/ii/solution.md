<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The strips are nested. Every connection permitted inside $T_k$ is also permitted inside $T_{k+1}$, so $q_k(n)\leq q_{k+1}(n)$ for every fixed separation. Consequently

$$
f_{k+1}(p)=\inf_{n\geq1}\frac{-\log q_{k+1}(n)}n\leq\inf_{n\geq1}\frac{-\log q_k(n)}n=f_k(p).
$$

The preceding nonnegative bound makes this a decreasing [sequence](../../../../../../../sequence.md) bounded below. By monotone convergence of real [sequences](../../../../../../../sequence.md),

$$
\boxed{\lim_{k\to\infty}f_k(p)=\inf_{k\geq1}f_k(p)\in[0,-\log p].}
$$

There is no assertion that this [limit of a sequence](../../../../../../../limit-of-a-sequence.md) is strictly positive: positivity at each fixed width need not survive an increasing-width [limit of a sequence](../../../../../../../limit-of-a-sequence.md).

One can also identify the [limit of a sequence](../../../../../../../limit-of-a-sequence.md). Let $q(n)$ be the [percolation two-point connection probability](../../../../../../../percolation-two-point-connection-probability.md) in the whole [square lattice](../../../../../../../square-lattice.md). Every finite connecting [graph path](../../../../../../../path-in-a-graph.md) has a bounded vertical extent, so $q_k(n)\uparrow q(n)$. Commuting infima gives the [strip approximation to the planar connection decay rate](../../../../../../../strip-approximation-to-the-planar-connection-decay-rate.md):

$$
\inf_k f_k(p)=\inf_k\inf_{n\geq1}\frac{-\log q_k(n)}n=\inf_{n\geq1}\inf_k\frac{-\log q_k(n)}n=\inf_{n\geq1}\frac{-\log q(n)}n.
$$

The same positive-association argument identifies the final [infimum](../../../../../../../infimum.md) with the whole-plane normalized logarithmic [limit of a sequence](../../../../../../../limit-of-a-sequence.md). This is an interchange of infima justified by monotonicity at fixed $n$. For example, when $p>1/2$, the threshold proved in question 2 and uniqueness give an [infinite percolation cluster](../../../../../../../infinite-percolation-cluster.md) with root [probability](../../../../../../../probability.md) $\theta(p)>0$. The [Harris-FKG inequality](../../../../../../../harris-fkg-inequality.md) makes the [probability](../../../../../../../probability.md) that both endpoints belong to it at least $\theta(p)^2$, so $q(n)\geq\theta(p)^2$. The whole-plane rate, and hence $\lim_k f_k(p)$, is then zero, despite the strict positivity of every finite-strip rate.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
