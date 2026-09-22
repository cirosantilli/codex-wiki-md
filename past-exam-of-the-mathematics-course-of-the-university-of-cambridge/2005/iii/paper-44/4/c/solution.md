<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume equal allocation of $n$ independent offenders to each arm and a two-sided [statistical test](../../../../../../statistical-test.md) of [significance level](../../../../../../significance-level.md) $\alpha$. Write $p_0=0.60$ for P30 and $p_1=0.56$ for initial community-service assignment, with $\Delta=p_0-p_1=0.04$ and $\bar p=(p_0+p_1)/2=0.58$. The two event counts have independent [binomial distributions](../../../../../../binomial-distribution.md). Under the stated alternative, the difference of sample proportions is approximately a [normal distribution](../../../../../../normal-distribution.md) with mean $\Delta$ and [variance](../../../../../../variance-split.md)

$$
\frac{p_0(1-p_0)+p_1(1-p_1)}{n}.
$$

The pooled two-proportion test has approximate upper rejection threshold $z_{1-\alpha/2}\sqrt{2\bar p(1-\bar p)/n}$ at the planning rates, where $z_q$ is the [standard normal quantile](../../../../../../standard-normal-quantile.md). To obtain [statistical power](../../../../../../statistical-power.md) $0.80$ against a positive difference, place the alternative mean $z_{0.80}$ alternative-standard-errors above that threshold:

$$
\Delta\sqrt n
\simeq z_{1-\alpha/2}\sqrt{2\bar p(1-\bar p)}
+z_{0.80}\sqrt{p_0(1-p_0)+p_1(1-p_1)}.
$$

Solving yields the usual [sample size for comparing two proportions](../../../../../../sample-size-for-comparing-two-proportions.md):

$$
\boxed{n\simeq\frac{\left[z_{1-\alpha/2}\sqrt{2(0.58)(0.42)}
+z_{0.80}\sqrt{(0.60)(0.40)+(0.56)(0.44)}\right]^2}{(0.04)^2}}
$$

per arm, rounded upwards, with total [sample size](../../../../../../sample-size.md) $2n$. This targets the dominant rejection tail under the planning alternative; an exact power calculation can include the very small opposite-tail probability or use the [binomial distributions](../../../../../../binomial-distribution.md) directly.

For illustration, at $\alpha=0.05$, $z_{0.975}\simeq1.960$ and $z_{0.80}\simeq0.842$, giving $n\simeq2388.8$. Thus

$$
\boxed{2389\text{ per arm, or }4778\text{ altogether}.}
$$

For a prespecified one-sided test, replace $z_{1-\alpha/2}$ by $z_{1-\alpha}$. The calculation assumes complete endpoint ascertainment, independent individual allocation and that the two initial-policy rates are appropriate; losses or clustered allocation would require corresponding design adjustments.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
