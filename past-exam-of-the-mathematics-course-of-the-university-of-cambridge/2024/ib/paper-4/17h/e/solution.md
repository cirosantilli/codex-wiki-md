<h1 id="17h/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the residual variance estimator

$$
s^2=\frac1{n-2}\sum_{i=1}^n
\{Y_i-\hat\alpha'-\hat\beta'(x_i-\bar x)\}^2.
$$

Under the Gaussian linear model, $\bar Y$ is independent of $s^2$ and

$$
\frac{(n-2)s^2}{\sigma^2}\sim\chi^2_{n-2}.
$$

Consequently the [Student t confidence interval for a centered regression intercept](../../../../../../student-t-confidence-interval-for-a-centered-regression-intercept.md) follows from

$$
\frac{\bar Y-\alpha'}{s/\sqrt n}\sim t_{n-2}.
$$

It is

$$
\boxed{\bar Y\pm t_{n-2,0.975}\frac{s}{\sqrt n}}.
$$

The displayed pivotal quantity lies between its 2.5% and 97.5% quantiles with probability $0.95$, which proves the stated coverage.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
