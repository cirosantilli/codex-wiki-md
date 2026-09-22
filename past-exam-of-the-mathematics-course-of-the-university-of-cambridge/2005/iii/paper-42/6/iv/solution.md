<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $W=2[\ell(\widehat\theta)-\ell(\widetilde\theta)]$ be a regular [likelihood-ratio test statistic](../../../../../../likelihood-ratio-test-statistic.md) for $r$ smooth restrictions, so its leading null law is $\chi_r^2$. Suppose a higher-order calculation gives $\mathbb E_0W=r+a/n+O(n^{-2})$. The [Bartlett correction](../../../../../../bartlett-correction.md) rescales the statistic:

$$
\boxed{W_B=\frac{W}{1+a/(rn)}.}
$$

Its mean is $r+O(n^{-2})$, eliminating the first-order mean error. In regular [likelihood](../../../../../../likelihood-function.md) models satisfying the usual Bartlett expansion, the same scaling removes the leading $n^{-1}$ distributional error against the chi-square reference law, leaving an $O(n^{-2})$ error for fixed tail probabilities. Matching a mean alone would not establish this distributional conclusion for an arbitrary statistic.

The coefficient depends on the model, null restrictions and [nuisance parameters](../../../../../../nuisance-parameter.md); it can be obtained from higher derivatives and [cumulants](../../../../../../cumulant.md) of the [log-likelihood](../../../../../../log-likelihood.md), or estimated by null simulation when an analytic expression is inconvenient. [Nuisance parameters](../../../../../../nuisance-parameter.md) require their appropriate null values or estimates. A correction improves finite-sample calibration within regular asymptotic theory; it does not turn a boundary-parameter or unidentifiable problem into a regular chi-square problem.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
