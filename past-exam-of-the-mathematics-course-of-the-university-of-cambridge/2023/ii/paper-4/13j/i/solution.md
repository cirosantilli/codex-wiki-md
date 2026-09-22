<h1 id="13j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Y_i$ be the first team's goal count in match $i$, let $x_i^T$ be row $i$ of the [design matrix](../../../../../../design-matrix.md), and let $\beta$ be the [regression coefficient](../../../../../../regression-coefficient.md) vector. The fitted [Poisson regression](../../../../../../poisson-regression.md) assumes that the $Y_i$ are [independent random variables](../../../../../../independent-random-variables.md) with

$$
Y_i\sim\operatorname{Pois}(\mu_i),
\qquad \log\mu_i=x_i^T\beta.
$$

The [likelihood function](../../../../../../likelihood-function.md) maximized by `glm` is therefore

$$
\boxed{L(\beta;y)
=\prod_{i=1}^{64}
 \frac{\mu_i^{y_i}e^{-\mu_i}}{y_i!}
=\prod_{i=1}^{64}
 \frac{\exp\{y_i x_i^T\beta-e^{x_i^T\beta}\}}{y_i!}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
