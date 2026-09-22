<h1 id="9/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**TODO: Attachment C is absent. Check its contents before treating this as a source-complete answer; the computation below uses the printed table, independent observations, a common within-season [variance](../../../../../variance-split.md) model and an explicitly chosen $5\%$ significance level.**

For a one-factor [analysis of variance](../../../../../analysis-of-variance.md), let $n_j,\bar x_j,s_j$ be the four seasonal sizes, means and [standard deviations](../../../../../standard-deviation.md). The weighted grand [arithmetic mean](../../../../../arithmetic-mean.md) is

$$
N=1430+1569+1639+2248=6886,\qquad \bar x=\frac{\sum_jn_j\bar x_j}{N}=5.06861458.
$$

This agrees with the rounded annual mean $5.07$. The between-season and within-season sums of squares are

$$
SS_B=\sum_jn_j(\bar x_j-\bar x)^2=2670.154583,\qquad SS_W=\sum_j(n_j-1)s_j^2=61829.619600.
$$

There are $4-1=3$ between-season [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md), because the four fitted seasonal means are compared subject to their weighted grand-mean constraint. There are $N-4=6882$ within-season [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md), because one mean was estimated in each group. The total has $N-1=6885$, equal to their sum. Hence

$$
MS_B=890.051528,\quad MS_W=8.98425161,\qquad \boxed{F=99.06797}.
$$

Under $H_0:\mu_W=\mu_{Sp}=\mu_{Su}=\mu_F$, compare with the [F-distribution](../../../../../f-distribution.md) on $(3,6882)$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). The $5\%$ critical value is about $2.60620$, with [p-value](../../../../../p-value.md) approximately $8.9\times10^{-63}$ from the rounded summaries. **Reject equality of all four means very strongly under the stated model.** The omnibus [hypothesis test](../../../../../statistical-hypothesis-test-split.md) establishes that at least one mean differs; it does not identify every pairwise difference.

The summer [variance](../../../../../variance-split.md) is substantially lower than the other three, so the exact common-variance [ANOVA](../../../../../analysis-of-variance.md) assumptions deserve checking, as does temporal independence. Raw observations would permit diagnostics and a heteroscedastic or time-dependent analysis. As a cross-check on arithmetic, $SS_B+SS_W=64499.774183$ implies annual sample [standard deviation](../../../../../standard-deviation.md) $3.06074$, matching the table's $3.06$. The numerical significance must not be mistaken for verification of the unobserved Attachment C or of the sampling model.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
