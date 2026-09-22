<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Model the count relative to exposure, for example

$$
y_i\mid b_i\sim\operatorname{Poisson}(E_i e^{x_i^T\beta+b_i}),\qquad b_i\mid\tau\sim N(0,\tau^2).
$$

Here $E_i$ is a measured exposure such as patient-days, $x_i$ contains hospital predictors, and $b_i$ is a [random effect](../../../../../../random-effect.md). This [Poisson regression](../../../../../../poisson-regression.md) separates hospital size from rate variation and supplies [partial pooling](../../../../../../partial-pooling.md). Use proper, scale-appropriate priors on coefficients and variation; add regional or temporal effects if the data demand them. A gamma mixing law with an estimated shape is another way to allow more flexible [overdispersion](../../../../../../overdispersion.md). Compare the fitted model's counts and dispersion through [posterior predictive checks](../../../../../../posterior-predictive-check.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
