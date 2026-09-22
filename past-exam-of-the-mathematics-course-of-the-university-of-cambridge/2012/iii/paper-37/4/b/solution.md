<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The saturated model estimates each Poisson mean separately as $Y_i$, permitting the boundary value zero when $Y_i=0$. Subtracting fitted from saturated [log-likelihood](../../../../../../log-likelihood.md) gives the [Poisson deviance](../../../../../../poisson-deviance.md)

$$
\boxed{D=2\sum_i\left[Y_i\log\frac{Y_i}{\widehat\mu_i}-(Y_i-\widehat\mu_i)\right],}
$$

with $0\log(0/\widehat\mu_i)=0$. A zero observation contributes $2\widehat\mu_i$. If the model includes an intercept, the score equation gives $\sum_iY_i=\sum_i\widehat\mu_i$, so the summed linear terms cancel; the unsimplified expression applies generally.

For [goodness of fit](../../../../../../goodness-of-fit.md), the [null hypothesis](../../../../../../null-hypothesis.md) is that the specified independent Poisson mean model is correct; the alternative is an unrestricted collection of means. When a quadratic likelihood approximation is valid, for example with fixed $n$ and large expected counts, $D$ has approximately a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $n-p$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md). Reject for a large upper-tail deviance. Merely increasing the number of sparse observations does not make this saturated-model reference reliable: the alternative dimension also increases. With small fitted means, replication-based checks or a [parametric bootstrap](../../../../../../parametric-bootstrap.md) are more defensible. This qualification concerns the absolute goodness-of-fit deviance; a fixed-dimensional nested likelihood-ratio comparison can have a better chi-squared approximation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
