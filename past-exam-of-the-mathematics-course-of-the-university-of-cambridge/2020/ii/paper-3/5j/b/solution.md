<h1 id="5j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [normal linear model](../../../../../../normal-linear-model.md), the [Gaussian likelihood](../../../../../../gaussian-likelihood.md) gives

$$
\ell(\beta,\sigma^2)
=-\frac n2\log(2\pi\sigma^2)
-\frac1{2\sigma^2}\|Y-X\beta\|^2.
$$

Maximization over $\beta$ gives the [ordinary least squares](../../../../../../ordinary-least-squares.md) estimator $\widehat\beta$, and maximization over the variance gives

$$
\widehat\sigma^2=\frac1n\|Y-X\widehat\beta\|^2.
$$

At this value the quadratic term in $-2\ell$ is $n$. There are $p$ [regression coefficients](../../../../../../regression-coefficient.md) and one variance parameter, so substitution into the [Akaike information criterion](../../../../../../akaike-information-criterion.md) yields

$$
\boxed{\operatorname{AIC}=n\bigl(1+\log(2\pi\widehat\sigma^2)\bigr)+2(p+1).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5J](../../5j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
