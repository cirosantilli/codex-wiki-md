<h1 id="7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose candidate variables from subject-matter knowledge, measurement quality and the target question before screening on outcomes. For an adjusted-effect analysis, retain prespecified [confounders](../../../../../../confounder.md) and essential design variables even when their individual $P$ values are large. For prediction, consider reliable predictors available at the intended prediction time; do not include future information. Handle missingness transparently, using a justified [multiple imputation](../../../../../../multiple-imputation.md) strategy where appropriate rather than changing the analyzed population unpredictably as variables enter.

Encode a categorical variable with $K-1$ indicators relative to a stated reference category, and assess it as a group. Check [multicollinearity](../../../../../../multicollinearity.md), sparse categories and plausible interactions. The relevant information is chiefly the number and distribution of events, not merely the number of enrolled subjects: hundreds of correlated or rarely varying predictors cannot be supported by a small event count.

Compare prespecified nested models by a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) based on the partial [log-likelihood](../../../../../../log-likelihood.md) and the change in parameter dimension. Penalized methods such as [ridge regression](../../../../../../ridge-regression.md) or [Lasso regression](../../../../../../lasso.md) applied to the Cox likelihood can stabilize many-variable models; choose tuning by suitable validation and account for mandatory variables. The [Akaike information criterion](../../../../../../akaike-information-criterion.md) or a limited, documented model-selection procedure can help balance fit and complexity. Unrestricted stepwise searches and repeated univariable screening invite unstable choices, omit joint confounding effects, and make naive post-selection intervals misleading. **Prefer a defensible, validated covariate set to a collection chosen only for small $P$ values.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7](../../7.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
