<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Couple the [Wald test](../../../../../../wald-test.md) statistics as $W_i=Z_i+\delta_i/s_i$, where the joint centered [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md) of $(Z_1,Z_2)$ is fixed. Increasing either $\delta_i$ enlarges, pointwise in this coupling, the event $\{W_1>c\text{ or }W_2>c\}$. Its probability is consequently nondecreasing in each treatment effect.

If both [null hypotheses](../../../../../../null-hypothesis.md) hold, then $\delta_1,\delta_2\le0$, so this probability is maximal at the joint boundary $(0,0)$. To check the [familywise error rate](../../../../../../familywise-error-rate.md) across all configurations, suppose only hypothesis $i$ is true. A [Type I error](../../../../../../type-i-and-type-ii-errors.md) then occurs only if $W_i>c$, with probability at most $1-\Phi(c)$, where $\Phi$ is the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). This is no larger than the any-rejection probability at $(0,0)$, since that joint event contains $\{Z_i>c\}$. If neither [null hypothesis](../../../../../../null-hypothesis.md) is true, the [familywise error rate](../../../../../../familywise-error-rate.md) is zero. Hence **the [least-favourable null configuration](../../../../../../least-favourable-null-configuration.md) for [Type I error](../../../../../../type-i-and-type-ii-errors.md)** is

$$
\boxed{\delta_1=\delta_2=0,\qquad\operatorname{FWER}_{\max}=1-\Phi_2(c,c;\rho),}
$$

where $\Phi_2$ is the centered [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md) function with [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) $\rho$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
