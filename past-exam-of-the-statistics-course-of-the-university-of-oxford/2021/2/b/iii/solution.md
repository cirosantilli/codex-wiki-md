<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Condition on the total of 400 complaints. Assume each complaint independently has the same [probability](../../../../../probability.md) $p$ of being received on Monday; in particular, repeated complaints from one incident must not create material dependence. The Monday count $S$ then has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $(400,p)$. Test $H_0:p=0.2$ against $H_1:p>0.2$, rejecting for large $S$ as suggested by the [monotone likelihood ratio](../../../../../monotone-likelihood-ratio.md).

Under the [null hypothesis](../../../../../null-hypothesis.md), $\mathbb E_0S=80$ and $\operatorname{Var}_0(S)=400(0.2)(0.8)=64$. Both expected successes and expected failures are large, so the [central limit theorem](../../../../../central-limit-theorem.md) gives a suitable [normal approximation](../../../../../normal-approximation.md):

$$
Z=\frac{S-80}{8}\ \mathrel{\dot\sim}\ N(0,1),\qquad
\boxed{z_{\rm obs}=\frac{100-80}{8}=2.5}.
$$

Using the paper's supplied rounded table, the upper-tail [p-value](../../../../../p-value.md) is approximately

$$
\boxed{p_{\rm approx}=1-\Phi(2.5)\approx0.005}.
$$

A more accurate evaluation of the [standard normal distribution](../../../../../standard-normal-distribution.md) [cumulative distribution function](../../../../../cumulative-distribution-function.md) gives about 0.0062. For example, choose [significance level](../../../../../significance-level.md) 0.05 before examining the data; the supplied upper 5% [standard normal quantile](../../../../../standard-normal-quantile.md) is approximately 1.6, and $2.5>1.6$. **Reject $H_0$ at 5%, and also at 1%, using this approximation.** The observed [binomial proportion](../../../../../binomial-proportion.md) is $100/400=0.25$, providing evidence that the Monday [probability](../../../../../probability.md) exceeds 0.2 under the sampling assumptions.

If applying a [continuity correction](../../../../../continuity-correction.md), approximate $\mathbb P_0(S\geq100)$ by $1-\Phi((99.5-80)/8)=1-\Phi(2.4375)\approx0.0074$; this gives the same 5% and 1% conclusions. The uncorrected value 0.005 is approximate, so a decision exactly at the 0.5% boundary is not warranted by the supplied rounded table.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
