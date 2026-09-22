<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Empirical likelihood](../../../../../../empirical-likelihood.md) assigns unknown probability masses $p_j\geq0$ to data-supported event times or intervals, imposes $\sum_jp_j=1$, and maximizes the product of each observation's probability. For event-time data, write $F(t)=\mathbb P(T\leq t)$ and $S(t)=1-F(t)$ for the [survivor function](../../../../../../survival-function.md). Exact, right-censored, left-censored, interval-censored, and truncated observations contribute the probability of their respective compatible sets.

The maximization uses that $S$ is nonincreasing and right-continuous, $S(0)=1$, and $S(t)\to0$ as $t\to\infty$. Probability mass need only be placed at endpoints that change an observation's compatible set; moving mass within any observationally indistinguishable interval leaves the likelihood unchanged. Maximizing over those masses gives the [nonparametric maximum-likelihood estimator](../../../../../../nonparametric-maximum-likelihood-estimator.md) of the survivor function.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
