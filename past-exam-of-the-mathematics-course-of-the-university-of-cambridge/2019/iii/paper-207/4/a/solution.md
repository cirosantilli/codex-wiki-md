<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Place discrete hazards $q_j$ at the ordered distinct event times $t_j$. If $d_j$ events occur among $r_j$ individuals at risk immediately before $t_j$, the nonparametric empirical likelihood is

$$
L(q)=\prod_jq_j^{d_j}(1-q_j)^{r_j-d_j},
\qquad0\leq q_j\leq1.
$$

Equivalently, an observed event at $x$ contributes the probability mass at $x$, while a right-censored observation contributes the survivor probability beyond its censoring time. Maximization gives $\widehat q_j=d_j/r_j$ and the [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md)

$$
\widehat S(t)=\prod_{t_j\leq t}(1-\widehat q_j).
$$

[Left truncation](../../../../../../left-truncation.md) means an individual is observed only conditional on surviving beyond an entry time $L$. Ignoring it overrepresents long survivors and creates [survivorship bias](../../../../../../survivorship-bias.md). A subject with event or censoring time $X>L$ contributes its usual likelihood divided by $S(L)$; in risk-set form, that individual enters each $r_j$ only for event times satisfying $L<t_j\leq X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
