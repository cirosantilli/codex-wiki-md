<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [fractional event imputation](../../../../../../fractional-event-imputation.md), let $q_j$ be the fractional event weight assigned to the seventh individual at $t_j$. Its event contribution at $t_j$ is $q_j$. It belongs to the [risk set](../../../../../../risk-set.md) at that time precisely for allocations at $t_j$ or later, so its fractional [risk set](../../../../../../risk-set.md) contribution is $\sum_{j'\ge j}q_{j'}$. This justifies both parts of the hint.

For $(q_4,q_5,q_6)=(1/2,1/4,1/4)$, the fractional counts at the last three times are

$$
(r_4,d_4)=(4,3/2),\qquad(r_5,d_5)=(5/2,5/4),\qquad(r_6,d_6)=(5/4,5/4).
$$

Earlier [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) factors still give survival $4/7$ immediately before $t_4$. Consequently

$$
\boxed{\widehat F_5^1=\frac47\left(1-\frac{3/2}{4}\right)\left(1-\frac{5/4}{5/2}\right)=\frac5{28}.}
$$

**The three values are** $\widehat F_5^0=1/7\simeq0.1429$, $\widehat F_5^1=5/28\simeq0.1786$, and $\widehat F_5^*=4/21\simeq0.1905$, in strictly increasing order. Spreading the censored individual's mass beyond $t_4$ raises the survivor estimate from the immediate-event imputation and moves it toward the original [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
