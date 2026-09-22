<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [bootstrapping](../../../../../../bootstrapping-statistics.md), repeatedly sample $X_1^*,\ldots,X_n^*$ with replacement from the empirical distribution of the observations and compute $\widehat β^*=α/\overline X^*$. Conditional on the data, estimate the $γ/2$ and $1-γ/2$ quantiles $q_l,q_u$ of $\sqrt n(\widehat β^*-\widehat β)$. The basic bootstrap interval is

$$
[\widehat β-q_u/\sqrt n,\widehat β-q_l/\sqrt n].
$$

As the number of resamples tends to infinity it estimates the conditional quantiles; bootstrap consistency and the continuous mapping theorem then give asymptotic coverage $1-γ$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28J](../../28j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
