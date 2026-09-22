<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $q_{rs}$ be the [transition intensity](../../../../../../transition-intensity.md) from state $r$ to $s$, and let $Q$ be the [transition intensity matrix](../../../../../../transition-intensity-matrix.md), with $q_{rr}=-\sum_{s\ne r}q_{rs}$. For a [continuous-time multi-state model](../../../../../../continuous-time-multi-state-model.md) with the [time-homogeneous Markov property](../../../../../../time-homogeneous-markov-property.md), the [transition probability matrix](../../../../../../transition-semigroup-of-a-continuous-time-markov-chain.md) is $P(u)=e^{uQ}$, with entry $p_{rs}(u)$. Condition on each recorded initial state. Panel visits contribute [transition probabilities](../../../../../../transition-probability.md); an exact entry into the absorbing death state contributes a [statistical probability density](../../../../../../probability-density-function.md)

$$
g_{r3}(u)=\sum_{s=1}^2p_{rs}(u)q_{s3}.
$$

This [mixed panel and exact-death likelihood](../../../../../../mixed-panel-and-exact-death-likelihood.md) sums over the living state just before death. It accounts for survival until the event; replacing its final factor by $p_{r3}(u)$ would count deaths throughout the interval.

Using the actual visit times recovered from the PDF, the three individual [likelihood](../../../../../../likelihood-function.md) contributions are

$$
\begin{aligned}
L_7={}&p_{12}(2.473380)p_{22}(3.708143)p_{22}(0.114158)
 p_{22}(0.811791)p_{22}(0.359291)p_{22}(0.457878)g_{23}(0.065913),\\
L_8={}&p_{11}(3.261286)p_{11}(1.231073),\\
L_9={}&p_{11}(1.289561)p_{11}(2.694442)p_{11}(0.450082)
 p_{12}(4.338740)p_{22}(0.273262).
\end{aligned}
$$

Here $g_{23}$ means $g_{r3}$ with $r=2$, not a [transition probability](../../../../../../transition-probability.md). Subjects 8 and 9 supply no event-density factor after their last panel observation. Assume independent subjects and noninformative examination and [censoring](../../../../../../censoring-statistics.md) times; conditional on their observation schedule, its distribution supplies no additional [statistical parameter](../../../../../../statistical-parameter.md)-dependent factor. The patients' [covariates](../../../../../../covariate.md) can be incorporated by using their own $Q_i$ in these same expressions.

For the progressive structure used in the subsequent output, put $a=q_{12}$, $b=q_{13}$, $c=q_{23}$ and $\lambda=a+b$. The [progressive illness-death model](../../../../../../progressive-illness-death-model.md) permits no recovery, so

$$
p_{11}(u)=e^{-\lambda u},\qquad p_{22}(u)=e^{-cu},\qquad
p_{12}(u)=\frac{a}{\lambda-c}(e^{-cu}-e^{-\lambda u}),\qquad
 g_{23}(u)=ce^{-cu}.
$$

When $\lambda=c$, the continuous limit is $p_{12}(u)=au e^{-cu}$. Thus the [likelihood](../../../../../../likelihood-function.md) contributions simplify to

$$
\boxed{\begin{aligned}
L_7&=p_{12}(2.473380)c\,e^{-c(7.990554-2.473380)},\\
L_8&=e^{-\lambda(4.492359)},\\
L_9&=e^{-\lambda(4.434085)}p_{12}(4.338740)e^{-c(0.273262)}.
\end{aligned}}
$$

Intermediate unobserved disease transitions remain integrated into each panel [transition probability](../../../../../../transition-probability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
