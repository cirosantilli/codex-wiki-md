<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\mu_U$ and $\mu_V$ be the [population means](../../../population-mean.md) of the newspaper trust score for the unvaccinated and vaccinated groups. A [two-sided hypothesis test](../../../two-sided-hypothesis-test.md) compares

$$
H_0:\mu_U-\mu_V=0,\qquad H_1:\mu_U-\mu_V\ne0.
$$

The observed [difference of sample means](../../../difference-of-sample-means.md) is $5.5-6.5=-1$: the vaccinated group has a one-unit higher average trust score. The negative [test statistic](../../../test-statistic.md) agrees with subtraction in this order. A [Student's t-test](../../../student-s-t-test.md) scales the estimated difference by its estimated [standard error](../../../standard-error.md); $t=-3.6$ means that the observed difference is 3.6 estimated [standard errors](../../../standard-error.md) below the equal-mean [null hypothesis](../../../null-hypothesis.md).

Using the reported reference [Student t-distribution](../../../student-s-t-distribution.md) with 747 [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md),

$$
\boxed{p=2\mathbb P(T_{747}\ge3.6)\approx0.000339.}
$$

Thus the equal-mean [null hypothesis](../../../null-hypothesis.md) is rejected at a prespecified 5%, 1% or 0.1% [significance level](../../../significance-level.md), subject to the test's assumptions. A [p-value](../../../p-value.md) is a probability of a result at least this extreme under the specified [null hypothesis](../../../null-hypothesis.md) and sampling model. It is neither the probability that the [null hypothesis](../../../null-hypothesis.md) is true nor the probability that this particular conclusion is mistaken. A chosen [significance level](../../../significance-level.md) controls the procedure's [type I error](../../../type-i-and-type-ii-errors.md) probability under that model.

The estimated difference is more informative than [statistical significance](../../../statistical-significance.md) alone. If the reported statistic uses this one-unit contrast, its estimated [standard error](../../../standard-error.md) is $1/3.6\approx0.2778$. The corresponding approximate 95% [confidence interval](../../../confidence-interval.md) is

$$
-1\pm t_{747,0.975}(0.2778)\approx[-1.545,-0.455].
$$

This interval concerns a [population mean](../../../population-mean.md) difference under repeated sampling; it is not a range containing 95% of individual trust scores. Its practical interpretation also depends on the trust scale and the importance of a one-unit difference.

The groups are disjoint, so an independent-samples comparison is appropriate if the sampled observations are independent. The exact pooled [Student's t-test](../../../student-s-t-test.md) additionally assumes common population [variance](../../../variance-split.md) and [normal distributions](../../../normal-distribution.md); [Welch's t-test](../../../welch-s-t-test.md) permits unequal [variances](../../../variance-split.md) and uses an approximate reference distribution. A bounded or ordinal rating need not be exactly normal, so treating it numerically and using a large-sample approximation also requires judgment about group sizes and the score's meaning.

There is a bookkeeping qualification. The later outputs use 748 observations. If these are also the complete observations for this two-group comparison, the pooled test has $748-2=746$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), and the [Welch degrees of freedom upper bound](../../../welch-degrees-of-freedom-upper-bound.md) is also 746. The printed 747 therefore needs the original test call or a different sample count to reconcile it. The reported-calibration calculation above answers the stated test; it does not invent group sizes or silently change the reference distribution.

**The evidence supports an association between higher newspaper trust and recorded vaccination, rather than a causal effect of trust.** An [observational study](../../../observational-study.md) does not rule out [confounding](../../../confounding.md), [selection bias](../../../selection-bias.md) or [reverse causation](../../../reverse-causality.md). A [statistical hypothesis test](../../../statistical-hypothesis-test-split.md) cannot supply those missing causal assumptions.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [2022](../../2022-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
