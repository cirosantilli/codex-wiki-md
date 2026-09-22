<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
g(a,c,b)=\frac{c}{\sqrt{ab}}=\rho.
$$

Its gradient, in the coordinate order $(a,c,b)$, is

$$
\nabla g=
\left(-\frac{\rho}{2a},\frac1{\sqrt{ab}},-\frac{\rho}{2b}\right)^T.
$$

Apply the [Delta method](../../../../../../delta-method.md) to the limit in part (c). Multiplying the displayed covariance matrix there on both sides by this gradient gives

$$
(\nabla g)^TV\nabla g=(1-\rho^2)^2.
$$

Consequently the [asymptotic distribution of the Gaussian sample correlation](../../../../../../asymptotic-distribution-of-the-gaussian-sample-correlation.md) is

$$
\boxed{
\sqrt n(\widehat\rho-\rho_{X,Y})
\xrightarrow d
N\!\left(0,
\left(1-\frac{\Sigma_{12}^2}{\Sigma_{11}\Sigma_{22}}\right)^2
\right).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
