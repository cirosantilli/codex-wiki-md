<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For subject $i=1,\ldots,100$ and $t_j\in\{0,2,4,6,8,10\}$, the [random-intercept linear mixed model](../../../../../../random-intercept-linear-mixed-model.md) is

$$
Y_{ij}=\beta_0+\beta_1t_j+b_i+\varepsilon_{ij},\qquad
b_i\overset{\mathrm{iid}}\sim N(0,\tau^2),\qquad
\varepsilon_{ij}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

All subject [random effects](../../../../../../random-effect.md) and measurement errors are mutually independent. The [fixed effects](../../../../../../fixed-effect.md) $\beta_0,\beta_1$ describe the population mean baseline and weekly gain. Conditional on $b_i$, a person's observations have independent [normal distributions](../../../../../../normal-distribution.md); after integrating out $b_i$, their [covariance](../../../../../../covariance.md) is $\tau^2$ at distinct weeks and their common [variance](../../../../../../variance-split.md) is $\tau^2+\sigma^2$. Therefore their [correlation](../../../../../../pearson-correlation-coefficient.md) is $\tau^2/(\tau^2+\sigma^2)$.

This [Gaussian linear mixed model](../../../../../../gaussian-linear-mixed-model.md) permits correlated repeated readings while keeping different subjects independent. The fitted [standard deviations](../../../../../../standard-deviation.md) are $\widehat\tau=21.67593$ kg and $\widehat\sigma=14.23496$ kg, giving within-person [correlation](../../../../../../pearson-correlation-coefficient.md) about $0.699$. All persons still have the same latent weekly slope in this model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
