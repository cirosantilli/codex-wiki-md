<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**The printed group means suggest about 13.49 more tweets in the liberal group, but the reported significance cannot be accepted as one coherent test result. The printed $p=0.04288$ would reject equal means at 5%; the printed $t=-1.9436$ with 23.92 [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md) instead gives a two-sided [p-value](../../../p-value.md) about 0.06380 and would not reject at 5%. The confidence-interval fields are also inconsistent.**

There are 14 conservative-coded and 12 liberal-coded observations. The tweet summary has [sample median](../../../sample-median.md) 258.5, [quartiles](../../../quartile.md) 204.5 and 323.2, and range 108 to 441, so the [interquartile range](../../../interquartile-range.md) is about 118.7 tweets. No measurement period is specified, so these should not be reinterpreted as tweets per day. The displayed overall [sample mean](../../../sample-mean.md) is 261.5, subject to a further consistency issue below. These are small groups; the summary alone cannot establish normality, lack of outliers or an appropriate sampling design.

Let $\mu_C$ and $\mu_L$ be the two population means for the defined tweet measure. The [null hypothesis](../../../null-hypothesis.md) is $H_0:\mu_C-\mu_L=0$, against the [two-sided test](../../../two-sided-hypothesis-test.md) alternative $H_1:\mu_C-\mu_L\ne0$. [Welch's t-test](../../../welch-s-t-test.md) uses

$$
t=\frac{\overline y_C-\overline y_L}{\sqrt{s_C^2/n_C+s_L^2/n_L}},
$$

allowing unequal group [variances](../../../variance-split.md). It requires independent observations and a suitable approximation to the sampling distribution of the mean difference; a large-sample justification cannot simply be assumed with group sizes 14 and 12. Its noninteger [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md) comes from the Welch approximation, not a fractional number of respondents.[Arguments and Details: two-sided alternative and unequal-variance Welch calculation](../../../student-s-t-test-in-the-r-documentation.md)

The two displayed [sample means](../../../sample-mean.md) imply

$$
\widehat\Delta=255.4286-268.9167=\boxed{-13.4881\text{ tweets}.}
$$

The negative sign means the liberal-coded group has the larger observed mean. This is a difference in group averages, not a statement about every individual and not evidence that political orientation causes tweeting behaviour. Practical importance concerns this difference and its context; [statistical significance](../../../statistical-significance.md) does not itself measure its importance.

A [p-value](../../../p-value.md) is calculated under the [null hypothesis](../../../null-hypothesis.md) and the assumed sampling model. It is the probability of a result at least as incompatible with that hypothesis as the observed one, not the probability that the hypothesis is true or that this conclusion is mistaken. A prespecified [significance level](../../../significance-level.md) controls the long-run [Type I error](../../../type-i-and-type-ii-errors.md) rate of rejecting a true null; a [Type II error](../../../type-i-and-type-ii-errors.md) is nonrejection of a false null, and [statistical power](../../../statistical-power.md) concerns rejection under a specified alternative. Neither a small [p-value](../../../p-value.md) nor a nonrejection settles the [effect size](../../../effect-size.md) or a causal explanation.

Taken on its own, the printed [p-value](../../../p-value.md) supports a nominal 5% rejection, but not a 1% rejection. Taken instead from the printed t statistic and [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), the two-sided tail is about 0.06380. These different 5% decisions cannot be reconciled by ordinary rounding. Conditional on trusting the group means, t and degrees of freedom, the implied [standard error](../../../standard-error.md) is $(-13.4881)/(-1.9436)\approx6.93975$ and the corresponding 95% [confidence interval](../../../confidence-interval.md) is

$$
\boxed{[-27.814,\ 0.837]\text{ tweets, conditional on those fields}.}
$$

It includes zero, consistently with that larger [p-value](../../../p-value.md). This calculation is a conditional consistency check, not recovery of the true raw-data interval.

The source lists its interval endpoints as 0.04582 and $-126.7904$, in that order. They are not ordered, and merely sorting them would still give midpoint about $-63.3723$, rather than the estimated difference $-13.4881$. The [symmetric confidence-interval consistency identities](../../../symmetric-confidence-interval-consistency-identities.md) therefore fail for the usual t interval. A frequentist 95% interval describes repeated-sample coverage of its procedure, not a 95% posterior probability for a fixed parameter; neither interpretation justifies silently repairing these endpoints.

The group summaries also imply pooled mean $(14\times255.4286+12\times268.9167)/26\approx261.6539$, which cannot round to the printed 261.5. The [pooled-mean compatibility under rounding](../../../pooled-mean-compatibility-under-rounding.md) identifies this additional mismatch for summaries of the same complete sample. Thus **the observed direction is conditionally liberal-greater-than-conservative, but the inferential decision and interval require corrected coherent output. Nonrejection under the t/df reading would not establish equal population means.** Random assignment, representativeness and possible [confounding](../../../confounding.md) are not supplied by this test.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [2018](../../2018-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
