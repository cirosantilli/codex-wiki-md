<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a conventional [two-sided test](../../../../../../two-sided-hypothesis-test.md) at [significance level](../../../../../../significance-level.md) $0.05$. Let $n=4000$ per arm, $p_C=0.005$, $p_T=0.0025$ and $\Delta=p_C-p_T=0.0025$. Under the specified alternative, the [normal approximation](../../../../../../normal-approximation.md) to the difference of independent [binomial proportions](../../../../../../binomial-proportion.md) has [standard deviation](../../../../../../standard-deviation.md)

$$
\sigma_1=\sqrt{\frac{p_C(1-p_C)+p_T(1-p_T)}n}=0.00136646.
$$

For planning the pooled null [standard error](../../../../../../standard-error.md), use $\bar p=(p_C+p_T)/2=0.00375$, giving $\sigma_0=\sqrt{2\bar p(1-\bar p)/n}=0.00136674$. The rejection threshold is approximately $1.96\sigma_0=0.00267880$, exceeding the mean alternative difference. With $\Phi$ the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md), the approximate [statistical power](../../../../../../statistical-power.md) is

$$
1-\Phi\left(\frac{1.96\sigma_0-\Delta}{\sigma_1}\right)+\Phi\left(\frac{-1.96\sigma_0-\Delta}{\sigma_1}\right)\simeq0.448.
$$

**No: the usual two-sided 5% calculation gives about 45% power, below 50%.** The expected death counts are only 20 and 10, so an exact discrete design calculation could refine this approximation.

The question does not specify the tail convention. If a beneficial direction is prespecified and a [one-sided test](../../../../../../one-sided-hypothesis-test.md) at 5% is justified, replace $1.96$ by approximately $1.645$; the resulting [statistical power](../../../../../../statistical-power.md) is about $0.573$, and the answer is then yes. This change of testing convention must be declared.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
