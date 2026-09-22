<h1 id="6h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [sufficient statistic](../../../../../../sufficient-statistic.md) $T$ is one for which the conditional distribution of the full sample $(X_1,\ldots,X_n)$ given $T$ does not depend on $p$. Take

$$
T=\sum_{i=1}^nX_i.
$$

For a binary sample $x$ with $\sum_i x_i=t$, its [likelihood function](../../../../../../likelihood-function.md) is

$$
p^t(1-p)^{n-t},
$$

which depends on the data only through $t$. By the [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md), $T$ is sufficient. Equivalently, conditionally on $T=t$, the sample is uniform over the $\binom nt$ binary vectors containing $t$ ones, independently of $p$.

## ↑ Ancestors (11)

1. [A](../a.md)
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
