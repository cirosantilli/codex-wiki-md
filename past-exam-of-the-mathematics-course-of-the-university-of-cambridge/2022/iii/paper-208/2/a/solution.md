<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $X_{-i}$ for all coordinates except $X_i$, let $X_i'$ be an [independent random variable](../../../../../../independent-random-variables.md) with the same distribution as $X_i$, and let $Z_i'=f(X_1,\ldots,X_i',\ldots,X_n)$. Three equivalent forms of the [Efron–Stein inequality](../../../../../../efron-stein-inequality.md) are

$$
\operatorname{Var}(Z)
\leq\sum_{i=1}^n\mathbb E\operatorname{Var}(Z\mid X_{-i}),
$$



$$
\operatorname{Var}(Z)
\leq\sum_{i=1}^n\mathbb E(Z-Z_i)^2
$$

for arbitrary square-integrable $Z_i$ measurable with respect to $X_{-i}$, and

$$
\operatorname{Var}(Z)
\leq\frac12\sum_{i=1}^n\mathbb E(Z-Z_i')^2.
$$

The first is the sharp choice within the second because [conditional expectation](../../../../../../conditional-expectation.md) is the least-squares projection. The first and third right sides are equal because two conditionally independent copies have expected squared difference twice their [conditional variance](../../../../../../conditional-variance.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
