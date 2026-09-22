<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The survival estimates favor the new treatment at the two reported times, with absolute survival differences **$0.199$ at two years and $0.157$ at five years**. These point differences alone do not establish efficacy. [Randomization](../../../../../../randomization.md) supports a causal comparison of the treatment assignments, but [sampling variance](../../../../../../variance-of-an-estimator.md), [censoring](../../../../../../censoring-statistics.md), follow-up, protocol adherence and the prespecified endpoint still matter. One should not infer a statistically established benefit merely from two larger estimates.

A [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) is

$$
\widehat S(t)=\prod_{t_j\le t}\left(1-\frac{d_j}{r_j}\right),
$$

where $r_j$ is the [risk set](../../../../../../risk-set.md) and $d_j$ the event count. Its uncertainty depends on the actual risk sets, not just the initial group size. The [Greenwood formula](../../../../../../greenwood-formula.md) estimates

$$
\operatorname{Var}(\widehat S(t))\approx\widehat S(t)^2\sum_{t_j\le t}\frac{d_j}{r_j(r_j-d_j)}.
$$

Without the missing survival tables one cannot calculate these [standard errors](../../../../../../standard-error.md) or the uncertainty of the group difference. In particular, replacing the estimator variance by the variance of an uncensored binomial proportion would generally be wrong.

I would advise presenting both curves with numbers at risk and [confidence intervals](../../../../../../confidence-interval.md), checking [independent censoring](../../../../../../independent-censoring.md), and reporting a prespecified overall comparison plus an effect estimate and interval. For an unadjusted [log-rank test](../../../../../../log-rank-test.md), write $O_1=\sum_jd_{1j}$ and $E_1=\sum_jd_jr_{1j}/r_j$. Its hypergeometric null variance is

$$
V=\sum_j\frac{r_{1j}r_{0j}d_j(r_j-d_j)}{r_j^2(r_j-1)},\qquad\frac{(O_1-E_1)^2}{V}\ \dot\sim\ \chi^2_1.
$$

Terms with no possible variation contribute zero. This compares the entire event history rather than selecting two arbitrary times, uses the available risk sets, and avoids choosing favorable time points after examining the curves. It is especially effective under proportional hazards. Crossing curves can make a log-rank comparison insensitive; a prespecified [restricted mean survival time](../../../../../../restricted-mean-survival-time.md) difference or another suitable time-varying analysis may then be more informative. An overall comparison does not make a clinically important prespecified time-point contrast invalid.

The [Kaplan–Meier median survival time](../../../../../../kaplan-meier-median-survival-time.md) is the first event time at which $\widehat S(t)\le1/2$. Monotonicity of the reported estimates implies

$$
\boxed{\widehat m_{\mathrm{new}}>5\text{ years if estimable},\qquad2<\widehat m_{\mathrm{standard}}\le5\text{ years}.}
$$

If the new-treatment curve never reaches one half during observed follow-up, its median is not estimable from that curve. The exact crossing times cannot be reconstructed from two survival probabilities: the standard curve could first cross at three or at four years and still have the same values at two and five years. **The point estimates suggest benefit, but the evidence and exact medians require the missing event/censoring tables.** Neither a conclusive agreement nor a conclusive rejection of benefit is justified from these numbers alone.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
