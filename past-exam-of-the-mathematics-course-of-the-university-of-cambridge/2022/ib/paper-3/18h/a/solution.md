<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The log likelihood, up to constants, is

$$
-\frac n2\log\sigma^2
-\frac1{2\sigma^2}(Y-X\beta)^T\Sigma_0^{-1}(Y-X\beta).
$$

Differentiation gives the [generalized least squares estimator](../../../../../../generalized-least-squares.md)

$$
\boxed{
\widehat\beta=(X^T\Sigma_0^{-1}X)^{-1}X^T\Sigma_0^{-1}Y},
$$

and maximizing over the scale gives

$$
\boxed{
\widehat\sigma^2
=\frac1n(Y-X\widehat\beta)^T\Sigma_0^{-1}(Y-X\widehat\beta)}.
$$

The divisor $n$ is appropriate for maximum likelihood rather than unbiased estimation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
