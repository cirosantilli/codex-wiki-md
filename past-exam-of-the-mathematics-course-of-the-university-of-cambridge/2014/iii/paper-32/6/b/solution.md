<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When the event comes from the one-covariate subject, the [Schoenfeld function for a three-person binary risk set](../../../../../../schoenfeld-function-for-a-three-person-binary-risk-set.md) is

$$
\boxed{s(\beta)=1-\frac{e^\beta}{2+e^\beta}=\frac2{2+e^\beta}.}
$$

Hence

$$
\boxed{s(-\infty)=1,\qquad s(0)=\frac23,\qquad s(\infty)=0.}
$$

These are limits where necessary. At a very negative coefficient the model assigns almost no event [probability](../../../../../../probability.md) to the observed one-covariate subject, producing the largest positive discrepancy. At zero coefficient all three subjects have equal [hazard functions](../../../../../../hazard-function.md), so the expected event covariate is $1/3$ and the discrepancy is $2/3$. At a very positive coefficient the observed subject is predicted to have the event almost surely, so the discrepancy tends to zero. The function decreases strictly and stays positive at every finite coefficient: this one event alone favors increasing $\beta$, while the other events in the complete [Cox partial likelihood](../../../../../../cox-partial-likelihood.md) determine its overall estimate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
