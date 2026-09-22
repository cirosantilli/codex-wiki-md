<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For subject $i$, write $\delta_i=\mathbf1_{\{T_i\le C_i\}}$, and define the [counting process](../../../../../counting-process.md) and pre-event [at-risk process](../../../../../at-risk-process.md) by

$$
N(t)=\sum_i\mathbf1_{\{X_i\le t,\ \delta_i=1\}},\qquad R(t)=\sum_i\mathbf1_{\{X_i\ge t\}}.
$$

Under independent [censoring](../../../../../censoring-statistics.md) and a common [hazard](../../../../../hazard-function.md), each observed event-free subject has conditional event [probability](../../../../../probability.md) $h(t)dt$ in a short interval. Therefore $\mathbb E(dN(t)\mid\text{past})=R(t)dH(t)$ to first order. Equivalently the [compensator of a counting process](../../../../../compensator-of-a-counting-process.md) is $\int_0^tR(s)dH(s)$. Dividing the observed increments by current exposure gives the estimating equation $d\widehat H=dN/R$, hence

$$
\boxed{\widehat H(t)=\int_0^t\frac{\mathbf1_{\{R(s)>0\}}}{R(s)}dN(s)=\sum_{t_j\le t}\frac{d_j}{r_j}.}
$$

Here $t_j$ are distinct event times, $d_j$ the number of events at that time, and $r_j=R(t_j)$ the number at risk immediately before it. One can also obtain the same increment by maximizing the local multiplicative-intensity likelihood $a^{d_j}e^{-r_ja}$: differentiation gives $a=d_j/r_j$. This derives the [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md), rather than merely naming it.

A censored observation contributes to the denominator while under observation, and then leaves the [risk set](../../../../../risk-set.md); it contributes no event jump. For tied events, use the single increment $d_j/r_j$, not $d_j$ successive one-event increments with shrinking denominators. If [censoring](../../../../../censoring-statistics.md) and events share a recorded time, a convention is needed; counting the event before removing same-time censored subjects uses the pre-time [risk set](../../../../../risk-set.md) above. Rounded or interval-censored data may require a model suited to their observation mechanism.

For the distinct ordered observations in the question, let $\delta_j$ indicate whether $X_j$ is an event. The [risk set](../../../../../risk-set.md) at $X_j$ contains precisely the $n-j+1$ subjects whose recorded time is at least $X_j$. Thus

$$
\widehat H(X_i)=\sum_{j\le i}\frac{\delta_j}{n-j+1},\qquad
\sum_{i=1}^n\widehat H(X_i)=\sum_{j=1}^n\frac{\delta_j}{n-j+1}\sum_{i=j}^n1
=\sum_{j=1}^n\delta_j.
$$

Therefore **the sum of the fitted integrated [hazards](../../../../../hazard-function.md) at all observation times equals the observed number of events**, the [event-count identity for Nelson–Aalen cumulative hazards](../../../../../event-count-identity-for-nelson-aalen-cumulative-hazards.md). The [grouped Nelson–Aalen event-count identity](../../../../../grouped-nelson-aalen-event-count-identity.md) extends the same argument to tied observations with their multiplicities and the stated risk-set convention.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
