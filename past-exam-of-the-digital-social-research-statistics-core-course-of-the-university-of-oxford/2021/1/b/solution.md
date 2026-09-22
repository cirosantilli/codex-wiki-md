<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Under the question's stipulated nonzero population difference, failing to reject is a [type II error](../../../../type-i-and-type-ii-errors.md).** A [type I error](../../../../type-i-and-type-ii-errors.md) would instead reject a true equal-mean [null hypothesis](../../../../null-hypothesis.md). The premise concerns the underlying difference: another study's [statistical significance](../../../../statistical-significance.md), by itself, would not prove that its conclusion is correct.

For a specified alternative and sampling design, write

$$
\beta=\mathbb P_{\rm alternative}(\text{do not reject }H_0),\qquad
1-\beta=\mathbb P_{\rm alternative}(\text{reject }H_0).
$$

The second probability is [statistical power](../../../../statistical-power.md). Across repeated [random samples](../../../../independent-and-identically-distributed-random-variables.md) under that same alternative and design, the long-run frequency of this kind of error is $\beta$.

**No numerical value of $\beta$ follows from this output.** It depends on the true [effect size](../../../../effect-size.md), group [variances](../../../../variance-split.md), [sample sizes](../../../../sample-size.md), decision rule and chosen [significance level](../../../../significance-level.md). In particular, it is neither $0.9561$, nor $1-0.9561$, nor automatically 5%. The reusable result that [a p-value does not determine the type II error probability](../../../../a-p-value-does-not-determine-the-type-ii-error-probability.md) demonstrates this directly in a simple normal testing model.

A small [effect size](../../../../effect-size.md) or an imprecise estimator can produce low [statistical power](../../../../statistical-power.md). The present [confidence interval](../../../../confidence-interval.md) describes the precision of the estimated difference; it does not supply the missing true alternative needed to calculate the [power function](../../../../power-function-of-a-statistical-test.md). A specified 5% [significance level](../../../../significance-level.md) concerns the [type I error](../../../../type-i-and-type-ii-errors.md) rate under the null, rather than a universal error rate whenever a result is nonsignificant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the digital social research: statistics core course of the University of Oxford](../../../split.md)
5. [Digital social research: statistics core course of the University of Oxford](../../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
6. [MSc in social science of the internet course of the University of Oxford](../../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
