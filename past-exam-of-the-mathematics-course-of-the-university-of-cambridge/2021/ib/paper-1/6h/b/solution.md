<h1 id="6h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md) states that if $T$ is sufficient and $U$ is an estimator with finite variance, then

$$
U^*=\mathbb E[U\mid T]
$$

has the same expectation as $U$ and no larger variance; it preserves unbiasedness. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives

$$
\mathbb E U^*=\mathbb E U.
$$

The [law of total variance](../../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}(U)
=\operatorname{Var}(\mathbb E[U\mid T])
+\mathbb E[\operatorname{Var}(U\mid T)]
\geq\operatorname{Var}(U^*).
$$

Sufficiency ensures that $U^*$ is a statistic whose definition does not depend on the unknown parameter. The inequality is strict exactly when the conditional variance is positive with positive probability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6H](../../6h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
