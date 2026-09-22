<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Y_{it}$ be the accident count at location $i$ in period $t\in\{0,1\}$, and $e_{it}$ its exposure in years, where $t=1$ denotes after installation. The [Poisson exposure model](../../../../../../poisson-exposure-model.md) is

$$
Y_{it}\overset{\mathrm{ind}}\sim\operatorname{Poisson}(e_{it}e^{\alpha+\beta t}),\qquad\log\mathbb E[Y_{it}]=\log e_{it}+\alpha+\beta t.
$$

The [offset](../../../../../../generalized-linear-model-offset.md) $\log e_{it}$ has its coefficient fixed at one. The model assumes constant rates within each period, a common before rate across locations, a common treatment rate ratio, independent counts, and Poisson variance equal to the mean. The [incidence rate ratio](../../../../../../rate-ratio.md) is $r=e^\beta$, so

$$
\boxed{\hat r=e^{-0.69901}=0.497077.}
$$

An approximate 95% [Wald confidence interval](../../../../../../wald-confidence-interval.md) transforms the interval for $\beta$:

$$
\boxed{\left[e^{-0.69901-1.96(0.27466)},e^{-0.69901+1.96(0.27466)}\right]=[0.290,0.852].}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
