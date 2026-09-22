<h1 id="o/o1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the same sample size $n$, the [geometric distribution](../../../../../geometric-distribution.md) provides more [Fisher information](../../../../../fisher-information-matrix.md):

$$
\frac{I_n^{\rm geom}(\theta)}{I_n^{\rm Bern}(\theta)}=\frac1\theta>1
\qquad(0<\theta<1).
$$

The corresponding asymptotic variances of the [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md) are

$$
\operatorname{Var}(\widehat\theta_{\rm geom})\approx\frac{\theta^2(1-\theta)}n,
\qquad
\operatorname{Var}(\widehat\theta_{\rm Bern})\approx\frac{\theta(1-\theta)}n.
$$

Hence **choose the geometric sample for more precise inference at equal numbers of observations**. Its asymptotic [variance](../../../../../variance-split.md) is $\theta$ times as large, and its [standard error](../../../../../standard-error.md) is $\sqrt\theta$ times as large. This illustrates [Fisher information per observation and per trial](../../../../../fisher-information-per-observation-and-per-trial.md). It is a per-observation comparison: one geometric observation records a waiting time containing, on average, $1/\theta$ Bernoulli trials. A constraint on the total number of underlying trials would be a different sampling-budget comparison.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [O1](../../o1.md)
3. [O](../../../o.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
