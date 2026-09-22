<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under [independent censoring](../../../../../../independent-censoring.md), order the distinct observed failure times as $t_1<\cdots<t_m$. Let $r_j=\#\{i:x_i\geq t_j\}$ be the size of the [risk set](../../../../../../risk-set.md) just before $t_j$, and let $d_j=\#\{i:x_i=t_j,v_i=1\}$ be the number of failures there. The estimated [conditional probability](../../../../../../conditional-probability.md) of surviving that event time is $1-d_j/r_j$. Multiplying these conditional survival [probabilities](../../../../../../probability.md) gives the [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md)

$$
\boxed{\widehat S(t)=\prod_{t_j\leq t}\left(1-\frac{d_j}{r_j}\right).}
$$

A censored observation leaves the [risk set](../../../../../../risk-set.md) after its [censoring](../../../../../../censoring-statistics.md) time but does not create a downward survival jump. With tied failure and [censoring](../../../../../../censoring-statistics.md) times, the displayed risk-set convention includes those censored at the time while processing failures, then removes them.

Since $H=-\log S$, the [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) of the [cumulative hazard function](../../../../../../cumulative-hazard-function.md) is

$$
\boxed{\widehat H_{\mathrm{KM}}(t)=-\log\widehat S(t)=\sum_{t_j\leq t}-\log\left(1-\frac{d_j}{r_j}\right).}
$$

This is not exactly the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) $\sum_{t_j\leq t}d_j/r_j$, although the two are close when the individual fractions are small. If a jump exhausts the [risk set](../../../../../../risk-set.md), $\widehat S$ becomes zero and $\widehat H_{\mathrm{KM}}$ becomes infinite; transformed residuals beyond that point require a finite-tail modelling convention or restriction of follow-up.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
