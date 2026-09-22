<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

The [posterior distribution](../../../../../../bayesian-posterior.md) has a long right tail. Its [posterior mean](../../../../../../posterior-mean.md) is pulled upward by relatively rare large endpoints and is sensitive to the artificial upper cutoff; its untruncated [posterior mean](../../../../../../posterior-mean.md) does not exist. The median is a central [quantile](../../../../../../quantile-function.md) that stays finite as the cutoff is removed and is much less sensitive to extreme draws. It is also the [Bayes estimator](../../../../../../bayes-estimator.md) under absolute-error loss, whereas a mean corresponds to squared-error loss when the relevant expectation exists.

**The median better represents the typical posterior endpoint in this strongly right-skewed distribution.** It need not be preferable for every decision problem, since the loss function matters. For comparison, exact summation of the truncated kernel at cutoff $5000$ gives median $195$ and mean about $397.67$; the displayed simulation summaries are Monte Carlo estimates, not exact posterior calculations.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
