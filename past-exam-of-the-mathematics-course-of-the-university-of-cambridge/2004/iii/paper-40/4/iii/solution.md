<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $H_i=f(x_i)\theta(x_i)/g(x_i)$. [Independence](../../../../../../independent-random-variables.md) gives $\operatorname{Var}(n^{-1}\sum_iH_i)=\operatorname{Var}(H_1)/n$, while part (i) gives $\mathbb E_gH_1=\mu$. Its [second moment](../../../../../../second-moment.md) is

$$
\mathbb E_gH_1^2=\int\frac{f(x)^2\theta(x)^2}{g(x)}\,dx.
$$

Consequently

$$
\boxed{\operatorname{Var}(\widehat\mu_g)
=\frac1n\int\frac{f(x)^2\theta(x)^2}{g(x)}\,dx-\frac{\mu^2}n.}
$$

The [variance](../../../../../../variance-split.md) is finite exactly when the displayed second-moment [integral](../../../../../../integral.md) is finite, assuming $\mu$ exists. An infinite [integral](../../../../../../integral.md) [means](../../../../../../expected-value.md) infinite [variance](../../../../../../variance-split.md), not failure of the change-of-density identity.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
