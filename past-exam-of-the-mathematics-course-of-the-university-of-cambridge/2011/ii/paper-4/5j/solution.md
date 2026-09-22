<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Model each person's infections over the fixed exposure period as an independent [Poisson random variable](../../../../../poisson-distribution.md) with mean $\mu_j$, conditional on the explanatory variables. The sum over $n_j$ people is then [Poisson distributed](../../../../../poisson-distribution.md) with mean $n_j\mu_j$, because independent Poisson counts add. This is reasonable for repeatable events occurring at an approximately constant rate without substantial clustering; the count need not be at most $n_j$, so a binomial model would not describe repeated infections.

The [Poisson regression](../../../../../poisson-regression.md) uses a [log link](../../../../../logarithmic-link-function.md) and the known [offset](../../../../../generalized-linear-model-offset.md) $\log n_j$. The omitted factor levels are the reference categories under [treatment contrasts](../../../../../treatment-contrast.md): their effects are absorbed into the intercept. Including all levels together with an intercept would make the [design matrix](../../../../../design-matrix.md) linearly dependent. For the proposed new group, the relevant predictor uses the intercept, the infrequent-swimmer coefficient and the age-20–24 coefficient; beach and female are reference levels. Hence

$$
\boxed{\widehat{\mathbb E}(\text{count})=20\exp(0.48887-0.61149-0.37442)\simeq12.17.}
$$

To add the age-by-sex interaction, one possible R command is
```
glm(count ~ freq + loc + age * sex, family = poisson, offset = log(n), data = swimmers)
```
where `swimmers` denotes the data frame. The product expands to both main effects and their interaction. There are two additional interaction coefficients because age has three levels and sex has two.

The nested-model comparison is a [likelihood-ratio test](../../../../../likelihood-ratio-test.md). The reduction in [Poisson deviance](../../../../../poisson-deviance.md) is $51.714-44.319\simeq7.3948$, asymptotically $\chi^2_2$ under the null hypothesis that both interaction coefficients are zero. Its reported $p$-value $0.02479$ gives evidence for an age-by-sex interaction at the five-percent level, though not at the one-percent level.

**Neither fitted Poisson model fits well in an absolute sense.** Comparing residual deviances with $\chi^2_{18}$ and $\chi^2_{16}$ respectively gives small tail probabilities: the deviance-to-degree-of-freedom ratios are about $2.87$ and $2.77$. Improvement relative to the simpler model does not establish goodness of fit. Omitted structure, dependence or [overdispersion](../../../../../overdispersion.md) could account for the remaining lack of fit; if the Poisson [variance](../../../../../variance-split.md) assumption is false, the nominal interaction-test calibration also needs reconsideration. The age label in the introductory legend is inconsistent with the actual model levels; the prediction uses the unambiguous age-20–24 row.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
