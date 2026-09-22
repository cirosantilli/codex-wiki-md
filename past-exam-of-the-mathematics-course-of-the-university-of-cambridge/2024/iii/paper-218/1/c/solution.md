<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The Pearson [goodness-of-fit test](../../../../../../goodness-of-fit-test.md) has null hypothesis that the independent counts follow the fitted [Poisson regression](../../../../../../poisson-regression.md), in particular $\operatorname{Var}(Y_i\mid d_i)=\mu_i$, against the alternative that the model does not fit; in this setting the scientifically relevant direction is [overdispersion](../../../../../../overdispersion.md), $\operatorname{Var}(Y_i\mid d_i)>\mu_i$. Under the null, $X_P^2$ is approximately [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $16$ degrees of freedom. Its tiny $p$-value decisively rejects the Poisson variance assumption.

The [negative binomial regression](../../../../../../negative-binomial-regression.md) keeps the logarithmic mean model but allows $\operatorname{Var}(Y_i\mid d_i)=\mu_i+\mu_i^2/\theta$. It improves the residual deviance from $75.806$ to $18.011$, close to its $16$ residual degrees of freedom, and lowers the [Akaike information criterion](../../../../../../akaike-information-criterion.md) from $172.34$ to $141.66$. Both comparisons strongly favour the negative-binomial fit, although its dose coefficient remains statistically insignificant.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
