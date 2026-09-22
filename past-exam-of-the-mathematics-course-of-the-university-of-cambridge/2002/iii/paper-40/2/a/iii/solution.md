<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $Y_i=\theta(X_i)f(X_i)/g(X_i)$. The independent summands have [expectation](../../../../../../../expected-value.md) $\mu$ and second moment

$$
\mathbb E_gY_i^2=\int\frac{f(x)^2\theta(x)^2}{g(x)}\,dx.
$$

When this [integral](../../../../../../../integral.md) is finite, independence gives

$$
\boxed{\operatorname{Var}(\widehat\mu_g)=\frac1n\left(\int\frac{f(x)^2\theta(x)^2}{g(x)}\,dx-\mu^2\right).}
$$

If the second-moment [integral](../../../../../../../integral.md) diverges, the [estimator](../../../../../../../estimator.md) can still be unbiased and consistent, but its [variance](../../../../../../../variance-split.md) is infinite; the finite-variance assumption cannot be omitted.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
