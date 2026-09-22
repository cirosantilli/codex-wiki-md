<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat the supplied uniform variates as [independent](../../../../../../independent-random-variables.md) $U(0,1)$ draws, as required for Monte Carlo simulation. Use $n$ of them and return

$$
\boxed{X=\sum_{j=1}^n\mathbf1_{\{U_j\leq p\}}.}
$$

Each indicator has a [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $p$, and the indicators are [independent](../../../../../../independent-random-variables.md). For any subset of $r$ successes the [probability](../../../../../../probability.md) is $p^r(1-p)^{n-r}$; there are $\binom nr$ such subsets. Thus $\mathbb P(X=r)=\binom nrp^r(1-p)^{n-r}$, the [binomial distribution](../../../../../../binomial-distribution.md). The construction includes the cases $p=0,1$ and $n=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
