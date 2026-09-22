<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mu_0,\mu_1$ be the [population means](../../../../population-mean.md) of the numerical [vaccination intention](../../../../vaccination-intention.md) score in the two recorded groups. The [two-sided hypothesis test](../../../../two-sided-hypothesis-test.md) compares

$$
H_0:\mu_0-\mu_1=0,\qquad H_1:\mu_0-\mu_1\ne0.
$$

The [sample means](../../../../sample-mean.md) are $13.48553$ and $13.46565$, giving a [difference of sample means](../../../../difference-of-sample-means.md) of approximately **0.01988 score points**, in the order group zero minus group one. The reported group counts are 1,866 and 262; seven observations have a missing group indicator.

[Welch's t-test](../../../../welch-s-t-test.md) divides that estimated difference by its estimated [standard error](../../../../standard-error.md). Its reported [test statistic](../../../../test-statistic.md) is $t=0.055032$, with approximately $344.43$ [statistical degrees of freedom](../../../../statistical-degrees-of-freedom.md). This is an unequal-variance comparison; fractional [statistical degrees of freedom](../../../../statistical-degrees-of-freedom.md) are appropriate for the Welch approximation. The two groups need not have equal [sample sizes](../../../../sample-size.md) or equal population [variances](../../../../variance-split.md).[Section 1.3.5.3, unpaired test statistic, unequal-variance standard error, and Welch–Satterthwaite degrees of freedom](../../../../two-sample-t-test-for-equal-means-by-national-institute-of-standards-and-technology.md)

The reported [p-value](../../../../p-value.md) is $0.9561$. Under the specified equal-mean [null hypothesis](../../../../null-hypothesis.md) and sampling model, a [p-value](../../../../p-value.md) measures the probability of a result at least as extreme as the observed one. It is not a posterior probability that the [null hypothesis](../../../../null-hypothesis.md) is true. **There is no rejection at a prespecified 5% significance level.** The observed [difference of sample means](../../../../difference-of-sample-means.md) is tiny relative to its estimated [standard error](../../../../standard-error.md).

The 95% [confidence interval](../../../../confidence-interval.md) is approximately

$$
\boxed{\mu_0-\mu_1:\quad[-0.69071,\ 0.73047].}
$$

It includes zero and differences in either direction. The interval's coverage refers to repeated use of the procedure under its assumptions, rather than to a probability assigned to this fixed unknown parameter or to the spread of individual scores. Nonrejection does not establish that the two [population means](../../../../population-mean.md) are identical.

[Simple random sampling](../../../../simple-random-sampling.md) supports the sampling interpretation, but the score is bounded and its raw distribution need not be a [normal distribution](../../../../normal-distribution.md). The large group sizes can support an approximate normal sampling distribution of the [sample means](../../../../sample-mean.md) under regularity conditions. The supplied [observational study](../../../../observational-study.md) does not identify a causal explanation of any difference, and the numeric coding of the group labels creates no biological or ordinal interpretation.

## ↑ Ancestors (11)

1. [A](../a.md)
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
