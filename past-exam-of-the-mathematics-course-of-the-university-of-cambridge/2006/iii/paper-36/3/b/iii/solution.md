<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Two distinct [triangles in a graph](../../../../../../../triangle-in-a-graph.md) with at most one common [vertex](../../../../../../../vertex-graph-theory.md) use disjoint [edges](../../../../../../../edge-of-a-graph.md), so their [indicator random variables](../../../../../../../indicator-random-variable.md) are independent and have zero [covariance](../../../../../../../covariance.md). A pair sharing an edge has covariance $p^5-p^6$. The count from part (i) gives

$$
\operatorname{Var}(X)
=\binom n3p^3(1-p^3)
+3\binom n3(n-3)p^5(1-p).
$$

With $\mu=\binom n3p^3$, the [triangle variance in a binomial random graph](../../../../../../../triangle-variance-in-a-binomial-random-graph.md) therefore satisfies

$$
\frac{\operatorname{Var}(X)}{\mu^2}
\leq\frac1{\binom n3p^3}
+\frac{3(n-3)}{\binom n3p}
=O((np)^{-3})+O((n^2p)^{-1}).
$$

Both terms tend to zero when $np\to\infty$, because $n^2p=n(np)\to\infty$. Applying part (ii) proves

$$
\boxed{\mathbb P(X>0)\longrightarrow1},
$$

completing the [triangle-existence threshold in a binomial random graph](../../../../../../../triangle-existence-threshold-in-a-binomial-random-graph.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 36](../../../../paper-36-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
