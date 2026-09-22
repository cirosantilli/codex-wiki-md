<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The solid [Poisson regression](../../../../../../poisson-regression.md) profile and dashed [negative binomial regression](../../../../../../negative-binomial-regression.md) profile peak at essentially the same $\beta\simeq0.69$. The dashed profile is slightly wider and has heavier shoulders: it gives larger relative [likelihood](../../../../../../likelihood-function.md) to values farther from the common maximizer. Thus **the estimated [mean](../../../../../../expected-value.md) ratio is stable, while the negative binomial model expresses slightly greater uncertainty**.

The [Poisson distribution](../../../../../../poisson-distribution.md) constrains [variance](../../../../../../variance-split.md) to equal the [mean](../../../../../../expected-value.md). A common negative binomial parametrization instead has $\operatorname{Var}(Y)=\mu+\mu^2/k$, with additional shape $k>0$; it permits [overdispersion](../../../../../../overdispersion.md) due, for example, to unexplained between-physician heterogeneity. Profiling this extra parameter lets the data support greater count variability and usually reduces information about the [mean](../../../../../../expected-value.md) contrast. In this two-group model, the fitted group [means](../../../../../../expected-value.md) remain the [sample means](../../../../../../sample-mean.md) for fixed $k$, which explains the nearly identical maximizers. The small separation of the profiles indicates a modest effect here, not overwhelming evidence for strong [overdispersion](../../../../../../overdispersion.md). The comparison concerns the original PDF figure; no figure is reproduced.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
