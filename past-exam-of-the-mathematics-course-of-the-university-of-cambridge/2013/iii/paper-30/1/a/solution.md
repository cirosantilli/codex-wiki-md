<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [normal linear model](../../../../../../normal-linear-model.md)

$$
\boxed{Y=X\beta+\varepsilon,\qquad \varepsilon\sim N_n(0,\sigma^2I_n).}
$$

Here $Y$ is the response [random vector](../../../../../../random-vector.md), $X$ is the known [design matrix](../../../../../../design-matrix.md), $\beta\in\mathbb R^p$ contains the unknown [regression coefficients](../../../../../../regression-coefficient.md), and $\sigma^2>0$ is the common error [variance](../../../../../../variance-split.md). Conditional on $X$, the errors have [normal distributions](../../../../../../normal-distribution.md) and are [independent random variables](../../../../../../independent-random-variables.md). Require $\operatorname{rank}X=p\leq n$ for [identifiability](../../../../../../identifiability.md) of $\beta$ and invertibility of $X^TX$. Usually $n>p$ is needed to estimate the error [variance](../../../../../../variance-split.md) from the [regression residuals](../../../../../../regression-residual.md). An intercept, when included, is represented by a column of ones in $X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
