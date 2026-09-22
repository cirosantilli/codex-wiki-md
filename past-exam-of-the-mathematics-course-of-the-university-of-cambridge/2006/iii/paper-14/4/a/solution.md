<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Y$ be the number of [isolated vertices](../../../../../../isolated-vertex.md) and set $\lambda=e^{-c}$. For fixed $k\geq1$, the [falling factorial](../../../../../../falling-factorial.md) $(Y)_k$ counts ordered $k$-tuples of distinct [isolated vertices](../../../../../../isolated-vertex.md). A specified tuple is isolated exactly when all [edges](../../../../../../edge-of-a-graph.md) incident to its vertices are absent. There are $k(n-k)+\binom k2$ such [edges](../../../../../../edge-of-a-graph.md), so

$$
\mathbb E(Y)_k=(n)_k(1-p)^{k(n-k)+\binom k2}.
$$

Since $np=\log n+c$ and $np^2=o(1)$, taking [logarithms](../../../../../../logarithm.md) gives

$$
\log\mathbb E(Y)_k=k\log n-k(\log n+c)+o(1)=-kc+o(1).
$$

Thus every fixed [factorial moment](../../../../../../factorial-moment.md) tends to $\lambda^k$. We use the standard [factorial-moment criterion for Poisson convergence](../../../../../../factorial-moment-criterion-for-poisson-convergence.md): nonnegative integer-valued [random variables](../../../../../../random-variable-split.md) whose [factorial moments](../../../../../../factorial-moment.md) converge, for every fixed order, to $\lambda^k$ converge in distribution to $\operatorname{Poisson}(\lambda)$. Consequently $Y$ has that limiting distribution, and its mass at each fixed integer converges. In particular,

$$
\boxed{\mathbb P(Y\geq1)\longrightarrow1-e^{-e^{-c}}.}
$$

This establishes the limiting [probability](../../../../../../probability.md) of at least one [isolated vertex](../../../../../../isolated-vertex.md), rather than merely a bound based on its [expectation](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
