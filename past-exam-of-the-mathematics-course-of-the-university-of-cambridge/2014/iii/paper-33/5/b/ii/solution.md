<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The first model's [residual deviance](../../../../../../../residual-deviance.md) is $671.27$ on $197$ [residual degrees of freedom](../../../../../../../residual-degrees-of-freedom.md), a ratio of about $3.41$. This is far above the scale expected from a well-fitting dispersion-one grouped [binomial regression](../../../../../../../binomial-regression.md). It suggests an inadequate mean function, [overdispersion](../../../../../../../overdispersion.md), or both. The linear age and exposure restrictions may miss nonlinear associations; the [generalized additive model](../../../../../../../generalized-additive-model.md) allows those shapes to be estimated through penalized [cubic regression splines](../../../../../../../cubic-regression-spline.md) rather than assumed.

The very small exposure Wald [p-value](../../../../../../../p-value.md) in the first fit suggests an association, but does not establish that a linear logit effect is adequate. Nor does the nonsignificant linear age term exclude every possible nonlinear age effect. Allowing estimated scale also addresses the excessive residual variation, which can arise from [clustered data](../../../../../../../clustered-data.md) because several births belong to the same woman. The second model's estimated scale $3.3506$ confirms that permitting smooth means has not removed all extra variation. **The reason to proceed is poor initial fit and possible nonlinear effects, with dispersion-aware inference**, not merely the wish to obtain more significant tests. These observational fits alone do not establish causation by the disaster.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
