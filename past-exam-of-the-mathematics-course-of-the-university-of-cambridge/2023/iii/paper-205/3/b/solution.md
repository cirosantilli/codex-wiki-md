<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditional on the covariates and all responses used to construct $\widehat g$, the residual $\varepsilon_i$ has conditional second moment at most $C$; [conditional independence](../../../../../../conditional-independence.md) under the null is what permits this conditioning. Consequently

$$
\mathbb E\!\left[\frac1n\sum_{i=1}^n\varepsilon_i^2G_i^2\right]
\leq C\,\mathbb E\!\left[\frac1n\sum_{i=1}^nG_i^2\right]\longrightarrow0.
$$

The [Markov inequality](../../../../../../markov-inequality.md) proves

$$
\frac1n\sum_i\varepsilon_i^2G_i^2\xrightarrow{p}0.
$$

Next, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\left|\frac1n\sum_i\xi_i\varepsilon_i^2G_i\right|
\leq
\left(\frac1n\sum_i\varepsilon_i^2G_i^2\right)^{1/2}
\left(\frac1n\sum_i\varepsilon_i^2\xi_i^2\right)^{1/2}.
$$

The first factor converges to zero in probability. The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) and part a make the second $O_p(1)$, so the product converges to zero in probability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
