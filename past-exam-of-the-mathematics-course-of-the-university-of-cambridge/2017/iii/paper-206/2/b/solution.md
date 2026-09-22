<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There are $120$ observations, since the intercept-only model has $119$ [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md). Adding price introduces one coefficient and decreases the [binomial deviance](../../../../../../binomial-deviance.md) by $148.263-101.920=46.343$. Adding a three-level factor introduces two coefficients and decreases it by $101.920-97.571=4.349$. Thus the missing entries are

$$
\boxed{1,\ 46.343;\qquad 2,\ 4.349,\ 116.}
$$

The [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) comparing the smaller and full [logistic regression](../../../../../../logistic-regression.md) tests $H_0:\beta_B=\beta_C=0$ against at least one nonzero layout contrast. Its statistic is $2(\widehat\ell_1-\widehat\ell_2)=4.349$. Under ordinary interior-parameter, full-rank and finite-estimate regularity conditions, [Wilks theorem](../../../../../../wilks-theorem.md) gives an asymptotic [chi-squared distribution](../../../../../../chi-squared-distribution.md) with two degrees of freedom. The reported [p-value](../../../../../../p-value.md) $0.1136$ exceeds $0.05$, so at that level retain the simpler price-only model.

The table is an [analysis of deviance for nested generalized linear models](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md): price is entered before layout. Thus its price row tests the price-only model against an intercept, whereas the layout row tests layout after allowing for price. The latter is the relevant comparison of model1 and model2. Failing to reject a layout effect is not proof that layouts have identical effects; it means these data do not justify the extra two parameters under this test.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
