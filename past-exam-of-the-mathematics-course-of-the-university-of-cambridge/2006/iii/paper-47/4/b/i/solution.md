<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Calculate the observed [sample correlation coefficient](../../../../../../../sample-correlation-coefficient.md) $\widehat r$. In each [paired bootstrap](../../../../../../../paired-bootstrap.md), draw 100 indices independently with replacement from $1,\ldots,100$ and select the corresponding whole pairs. Compute the [bootstrap](../../../../../../../bootstrapping-statistics.md) correlation $r_b^*$ from each resample; do not resample the two margins independently, since that would destroy their empirical dependence.

Let $q_p$ be the empirical $p$-quantile of those [bootstrap](../../../../../../../bootstrapping-statistics.md) correlations. The [percentile bootstrap confidence interval](../../../../../../../percentile-bootstrap-confidence-interval.md) is

$$
\boxed{[q_{0.025},q_{0.975}].}
$$

This is the requested algorithmic interval; the actual endpoints require the observed pairs. Its coverage is approximate, based on the sampling law of the correlation being well approximated by the [bootstrap](../../../../../../../bootstrapping-statistics.md) law. Both sample variances must be positive. Resamples having a constant margin have undefined correlation and cannot be repaired by arbitrarily assigning correlation zero. One may regenerate these exceptional resamples, explicitly conditioning on well-defined correlations; under the usual nondegenerate large-sample conditions their probability is negligible. Frequent degeneracy instead indicates that this ordinary correlation-bootstrap construction is unsuitable.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
