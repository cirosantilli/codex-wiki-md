<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The three [Poisson regression](../../../../../../poisson-regression.md) models have independent counts and a logarithmic [link function](../../../../../../link-function.md): their mean predictors include both `pc` and `urban` in `m1`, only `urban` in `m2`, and only `pc` in `m3`. Nested comparisons through the full model are preferable to a direct comparison of the two nonnested one-predictor models.

To remove `urban` from `m1`, test $H_0:\beta_{\rm urban}=0$ against $H_1:\beta_{\rm urban}\ne0$. The [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) statistic is the deviance difference

$$
D_{m3}-D_{m1}=290.93-290.64=0.29,
$$

with approximate null distribution $\chi^2_1$. It is below $3.84$, so do not reject at 5%. The corresponding Wald [p-value](../../../../../../p-value.md) $0.588$ is consistent with this decision. To remove `pc` from `m1`, test $H_0:\beta_{\rm pc}=0$ against a nonzero coefficient, giving $559.17-290.64=268.53$ with approximate null distribution $\chi^2_1$; reject decisively. The [Akaike information criterion](../../../../../../akaike-information-criterion.md) also prefers `m3`, whose value $710.94$ is smaller than $712.65$ and $979.19$.

**Among these three models choose `m3`, retaining building cover and omitting the urban indicator.** This is a comparison within the stated Poisson family; its absolute fit must still be checked, as the next part does.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
