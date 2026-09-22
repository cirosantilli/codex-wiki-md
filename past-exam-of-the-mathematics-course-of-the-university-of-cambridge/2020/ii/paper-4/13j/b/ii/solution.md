<h1 id="13j/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Writing $B_i$ for block $i$ and using $\sum_{j\in B_i}\tilde y_j=\bar y_i/\sigma^2$, the replicated likelihood factors as

$$
f(\tilde y;\tilde\mu,\tilde\sigma^2)
=\underbrace{
\exp\!\left\{
\sum_{i=1}^n\frac{\bar y_i\theta_i-b(\theta_i)}{a_i\sigma^2}
\right\}}_{g_1(\bar y;\beta)}
\underbrace{
\exp\!\left\{
\sum_i\sum_{j\in B_i}c(\tilde y_j,a_i)
\right\}}_{g_2(\tilde y)}.
$$

The second factor is independent of $\beta$, while the first depends on the data only through $\bar y$. The [Fisher-Neyman factorization theorem](../../../../../../../fisher-neyman-factorization-theorem.md) therefore makes $\bar Y$ a [sufficient statistic](../../../../../../../sufficient-statistic.md) for $\beta$ in the replicated experiment.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [13J](../../../13j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
