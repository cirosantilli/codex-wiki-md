<h1 id="5/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a homogeneous [continuous-time Markov chain](../../../../../../../continuous-time-markov-chain.md), the [holding time](../../../../../../../holding-time.md) in a living state $r$ before the next transition has survival [probability](../../../../../../../probability.md) $e^{-\lambda_rt}$, where $\lambda_r=\sum_{s\ne r}q_{rs}=-q_{rr}$. Indeed, conditional on still occupying that state, the [probability](../../../../../../../probability.md) of leaving in the next $dt$ is $\lambda_rdt+o(dt)$, so its survival function satisfies $S'(t)=-\lambda_rS(t)$ and $S(0)=1$. Integrating gives the [mean holding time from a transition intensity matrix](../../../../../../../mean-holding-time-from-a-transition-intensity-matrix.md):

$$
\boxed{\tau_r=\int_0^\infty e^{-\lambda_rt}\,dt=\frac1{\lambda_r}=-\frac1{q_{rr}}.}
$$

This is the mean time until any allowed exit from that state, not necessarily the patient's remaining lifetime.

For confidence limits, use the supplied [standard error](../../../../../../../standard-error.md) $s_r$ of the corresponding diagonal generator estimate. Changing its sign does not change its [standard error](../../../../../../../standard-error.md), so it is also the [standard error](../../../../../../../standard-error.md) of $\widehat\lambda_r$. The [delta method](../../../../../../../delta-method.md), with derivative $d(1/\lambda)/d\lambda=-1/\lambda^2$, gives

$$
\operatorname{se}(\widehat\tau_r)\approx\frac{s_r}{\widehat\lambda_r^2},\qquad
\widehat\tau_r\pm1.96\frac{s_r}{\widehat\lambda_r^2}.
$$

The resulting approximate 95% [Wald confidence intervals](../../../../../../../wald-confidence-interval.md) are

$$
\boxed{\begin{array}{c|r|r|c}
\text{state}&\widehat\tau_r\ (\text{years})&\operatorname{se}(\widehat\tau_r)&95\%\text{ interval}\rule{0pt}{2.5ex}\\\hline
1&11.765&0.498&(10.788,12.741)\\
2&5.525&0.644&(4.263,6.787)\\
3&2.710&0.181&(2.356,3.064)\\
4&1.949&0.258&(1.444,2.454)
\end{array}}
$$

The diagonal [standard errors](../../../../../../../standard-error.md) already incorporate the [covariance](../../../../../../../covariance.md) among outgoing rates. They should not be replaced by the square root of a sum of squared off-diagonal [standard errors](../../../../../../../standard-error.md), which would silently assume those rate estimates independent.

Alternatively construct a positive rate [confidence interval](../../../../../../../confidence-interval.md) and apply the [confidence interval for an inverse rate](../../../../../../../confidence-interval-for-an-inverse-rate.md) transformation. Here every normal rate interval has a positive lower endpoint, giving

$$
\left[\frac1{\widehat\lambda_r+1.96s_r},\frac1{\widehat\lambda_r-1.96s_r}\right].
$$

These approximate intervals are, respectively, $(10.863,12.830)$, $(4.497,7.161)$, $(2.397,3.117)$ and $(1.548,2.631)$ years. They are asymmetric because inversion is nonlinear; positive log-rate or likelihood-based intervals could also be inverted. The symmetric delta intervals and the inverted-rate intervals are two legitimate first-order approaches and need not have numerically identical endpoints.

The death state has zero exit rate, so its [holding time](../../../../../../../holding-time.md) is infinite. There is no finite mean-sojourn estimate or ordinary finite [confidence interval](../../../../../../../confidence-interval.md) for this structurally [absorbing state](../../../../../../../absorbing-state.md). All intervals above concern the mean parameter, not a [prediction interval](../../../../../../../prediction-interval.md) for one patient's realized [holding time](../../../../../../../holding-time.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [5](../../../5.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
