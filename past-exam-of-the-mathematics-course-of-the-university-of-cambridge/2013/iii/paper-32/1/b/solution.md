<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $y_i$ be each trial's estimated [log risk ratio](../../../../../../log-risk-ratio.md), with estimated sampling [variance](../../../../../../variance-split.md) $s_i^2$. A [fixed-effect meta-analysis](../../../../../../fixed-effect-meta-analysis.md) models the independent estimates as $y_i\simeq N(\mu,s_i^2)$, with one common true [log risk ratio](../../../../../../log-risk-ratio.md) $\mu$. Differentiating the Gaussian [log-likelihood](../../../../../../log-likelihood.md), or minimizing $\sum_i(y_i-\mu)^2/s_i^2$, gives inverse-[variance](../../../../../../variance-split.md) weights $w_i=1/s_i^2$ and

$$
\boxed{\widehat\mu=\frac{\sum_iw_iy_i}{\sum_iw_i},\qquad
\operatorname{Var}(\widehat\mu)\simeq\frac1{\sum_iw_i}.}
$$

The [variance](../../../../../../variance-split.md) follows directly by adding independent [variances](../../../../../../variance-split.md) of the weighted estimates: $\sum_iw_i^2s_i^2/(\sum_iw_i)^2=1/\sum_iw_i$.

Using the printed rounded estimates and [standard errors](../../../../../../standard-error.md), $\sum_iw_i=50.2923$, so

$$
\boxed{\widehat\mu=-0.1028,\qquad
\widehat{\operatorname{Var}}(\widehat\mu)=0.019884,
\qquad\operatorname{SE}(\widehat\mu)=0.14101.}
$$

The pooled [risk ratio](../../../../../../risk-ratio.md) is about $0.902$. An interval using the same quantile two is $(-0.3848,0.1792)$ on the log scale, so it includes no effect. Recomputing all trial estimates from the event counts would change the last digits because the printed log estimates and errors are rounded.

The key assumptions are independent trials, a common true treatment effect on this chosen log scale, approximately unbiased and approximately normal trial estimates, and suitable sampling-[variance](../../../../../../variance-split.md) estimates. The common-effect assumption is stronger than merely studying the same named treatment: systematic population, treatment or design differences may produce genuine heterogeneity. For an unbiased interpretation of the pooled evidence, inclusion of studies must also not depend selectively on their results. Treating the plug-in [variances](../../../../../../variance-split.md) as fixed is the usual approximation in the displayed [variance](../../../../../../variance-split.md) formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
