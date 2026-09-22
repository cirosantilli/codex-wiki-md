<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Four distinct objections, each with a corresponding improvement, are as follows.

- **Different patients imply different baseline risks.** Raw death rates confound performance with [case mix](../../../../../../case-mix.md), including urgency, disease severity and comorbidity. Use a prespecified, validated [risk-adjusted provider comparison](../../../../../../risk-adjusted-provider-comparison.md), standardizing to comparable patients or comparing observed deaths with $\sum_i\widehat p_i$. Check overlap and model calibration rather than assuming adjustment removes all [confounding](../../../../../../confounding.md).
- **Small annual volumes produce unstable rankings.** A few deaths can move a surgeon far up or down a league table; zero deaths need not indicate zero risk. Display counts and suitably calibrated [confidence intervals](../../../../../../confidence-interval.md) for [binomial proportions](../../../../../../binomial-proportion.md), preferably in [funnel plots](../../../../../../funnel-plot.md) against volume. Pool suitable periods or use a [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md) to stabilize estimates, while allowing genuine time changes.
- **Many simultaneous comparisons generate chance outliers.** With $m$ independent null comparisons, the [probability](../../../../../../probability.md) of at least one false positive is $1-0.95^m$, and ranks amplify selection of extremes. Use [multiple testing](../../../../../../multiple-hypothesis-testing.md) adjustments or simultaneous control limits and seek confirmation before interpreting an apparent outlier. Dependence through the national comparator must also be accounted for.
- **The endpoint and unit of attribution can mislead.** In-hospital death depends on discharge and transfer policy, and care is delivered by a team; follow-up after discharge is omitted. Use an independently audited fixed-horizon endpoint, such as a prespecified 30-day mortality outcome, linked across hospitals and to death registrations, and report an appropriate team or institutional comparison alongside any surgeon-level estimate. Reliable attribution and consistent inclusion criteria reduce incentives to manipulate coding or case selection.

**A confidence interval containing the national rate does not demonstrate equivalence**, and a raw ranking does not establish a causal performance difference. The improved presentation should convey precision and uncertainty as well as the estimated outcome.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
