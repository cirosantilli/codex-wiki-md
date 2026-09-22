<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [likelihood function](../../../../../../likelihood-function.md) and [prior distribution](../../../../../../prior-probability.md) give the [posterior density](../../../../../../posterior-density.md)

$$
\pi(\beta\mid Y)\propto
\exp\left\{-\frac12(Y-X\beta)^T\Sigma_e^{-1}(Y-X\beta)
-\frac12\beta^T\Sigma^{-1}\beta\right\}.
$$

Completing the square in the [quadratic form](../../../../../../quadratic-form.md) gives

$$
C=\left(X^T\Sigma_e^{-1}X+\Sigma^{-1}\right)^{-1},
\qquad
m=CX^T\Sigma_e^{-1}Y.
$$

Thus [Gaussian conjugacy for a normal linear model](../../../../../../gaussian-conjugacy-for-a-normal-linear-model.md) yields

$$
\boxed{\beta\mid Y\sim N(m,C).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
