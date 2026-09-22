<h1 id="17g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [binomial random graph](../../../../../../binomial-random-graph.md) $G(n,p)$ has vertex set $[n]=\{1,\ldots,n\}$, and each unordered pair of distinct vertices is included as an [edge](../../../../../../edge-of-a-graph.md) independently with probability $p$.

Let $X_t$ count copies of the [complete graph](../../../../../../complete-graph.md) $K_t$. Each $t$-element vertex set forms a copy with probability $p^{\binom t2}$, so [linearity of expectation](../../../../../../linearity-of-expectation.md) gives

$$
\mathbb EX_t=\binom ntp^{\binom t2}.
$$

The event $E_t$ is $\{X_t\geq1\}$. By the [first moment method](../../../../../../first-moment-method.md),

$$
\begin{aligned}
\mathbb P(E_t)
&\leq\mathbb EX_t\\
&\leq\frac{n^t}{t!}p^{t(t-1)/2}\\
&=\frac1{t!}
\left(pn^{2/(t-1)}\right)^{t(t-1)/2}
\longrightarrow0.
\end{aligned}
$$

This is the [clique count in a binomial random graph](../../../../../../clique-count-in-a-binomial-random-graph.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
