<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

One method breaks a tied group into a sequence of distinct artificial times, by a specified or random ordering. Process tied events before tied censorings if their common recorded time means the censored individuals were still under observation when the events occurred. At each artificial event, add the reciprocal of the current [risk set](../../../../../../risk-set.md) size and then remove that individual. This applies the untied [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) to the resulting grid. For example, two tied failures among two individuals give successive increments $1/2$ and $1$.

On that expanded grid there is one observation time per individual. The cancellation argument in (b) is unchanged, so **breaking ties preserves the identity when the sum includes every artificially separated observation**. The chosen ordering can affect the estimated curve within a tied group and must not be presented as an observed event order.

A second method retains the recorded tied times. For a group with $d_j$ events and pre-time [risk set](../../../../../../risk-set.md) size $r_j$, the grouped [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) adds $d_j/r_j$ once. All events in the group use the same denominator; censorings in the group are removed afterwards. If two individuals fail at the same time and there are no other observations, the curve has one jump of $2/2=1$. Its sum over the one distinct time is $1$, whereas the event count is $2$. Hence **the unweighted distinct-time identity does not generally survive grouping ties**. On the artificially separated grid in the first method, the two post-observation values would instead be $1/2$ and $3/2$, whose sum is $2$.

There is nevertheless an exact weighted version for the grouped method. Let $n_j$ count all observations, event or [censoring](../../../../../../censoring-statistics.md), at distinct time $t_j$. With everyone entering at zero, $r_k=\sum_{j\geq k}n_j$. Therefore

$$
\boxed{\sum_j n_j\widehat H(t_j)
=\sum_k\frac{d_k}{r_k}\sum_{j\geq k}n_j
=\sum_kd_k.}
$$

This [grouped Nelson–Aalen event-count identity](../../../../../../grouped-nelson-aalen-event-count-identity.md) sums over individuals, with repeated values for tied times, rather than once per distinct time. Keeping that distinction resolves the apparent conflict between a valid grouped estimator and failure of the literal unweighted formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
