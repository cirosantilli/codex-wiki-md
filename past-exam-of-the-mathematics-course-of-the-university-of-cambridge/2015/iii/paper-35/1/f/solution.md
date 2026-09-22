<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Treat the extra measurements as [auxiliary variables for multiple imputation](../../../../../../auxiliary-variable-for-multiple-imputation.md). Include alcohol consumption and disease history as predictors in both the $C$ and $P$ [conditional distributions](../../../../../../conditional-distribution.md), together with age, sex and the other incomplete response. If these auxiliary variables themselves have missing entries, give them appropriate models and update them within the same [multiple imputation by chained equations](../../../../../../multiple-imputation-by-chained-equations.md) sweeps. Preserve observed entries throughout.

**Useful auxiliary measurements can improve predictions, precision and the plausibility of missing at random.** Their association with the missing responses reduces uncertainty in the imputed values; association with nonresponse may explain some selection that otherwise depends on unobserved values. This can reduce [selection bias](../../../../../../selection-bias.md) under the enlarged [missing at random](../../../../../../missing-at-random.md) model and reduce between-imputation [variance](../../../../../../variance-split.md). It does not guarantee elimination of [missing not at random](../../../../../../missing-not-at-random.md) dependence. They need not be added to the final substantive [logistic regression](../../../../../../logistic-regression.md) merely because they help imputation: the final analysis should still estimate its intended association.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
