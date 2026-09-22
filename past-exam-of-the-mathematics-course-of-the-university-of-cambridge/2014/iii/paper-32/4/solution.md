<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [counting process](../../../../../counting-process.md) $N(t)$ adapted to its observed history $\mathcal F_t$, a predictable [counting-process intensity](../../../../../counting-process-intensity.md) $\lambda(t)$ specifies

$$
E\{dN(t)\mid\mathcal F_{t-}\}=\lambda(t)\,dt,
$$

or more generally $N(t)-\int_0^t\lambda(u)\,du$ is a [local martingale](../../../../../local-martingale.md). In [survival analysis](../../../../../survival-analysis-split.md), let $N_i(t)=\mathbf1\{x_i\le t,v_i=1\}$ record failures and $Y_i(t)=\mathbf1\{x_i\ge t\}$ record the [risk set](../../../../../risk-set.md), including subjects at their own observation time. Under independent [right censoring](../../../../../right-censoring.md) and a common [hazard function](../../../../../hazard-function.md) $h$, the aggregate intensity is $Y(t)h(t)$, where $N=\sum_iN_i$ and $Y=\sum_iY_i$.

Writing $H(t)=\int_0^th(u)\,du$, the conditional increment equation is $E(dN\mid\mathcal F_{t-})=Y\,dH$. Replacing $dH$ by the observed increment $dN/Y$ gives the [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md)

$$
\boxed{\widehat H(t)=\int_0^t\frac{\mathbf1\{Y(u)>0\}}{Y(u)}\,dN(u)=\sum_{t_j\le t}\frac1{Y(t_j)},}
$$

where $t_j$ ranges over the distinct observed event times. Censored observations remove subjects from subsequent [risk sets](../../../../../risk-set.md) but do not produce hazard jumps.

For these data the [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md) gives

$$
\begin{array}{c|rrrrrr}
\text{observation time}&3&4&5&6&9&13\\\hline
\text{risk count just before}&6&5&4&3&2&1\\
\text{hazard increment}&1/6&0&0&1/3&1/2&1\\
\widehat H(\text{observation time})&1/6&1/6&1/6&1/2&1&2
\end{array}
$$

Thus the six fitted [cumulative hazards](../../../../../cumulative-hazard-function.md) sum to $3(1/6)+1/2+1+2=4$, the number of observed failures.

The [event-count identity for Nelson–Aalen cumulative hazards](../../../../../event-count-identity-for-nelson-aalen-cumulative-hazards.md) follows by exchanging the finite sums. With everyone entering at time zero,

$$
\boxed{\sum_{i=1}^n\widehat H(x_i)=\sum_{j:\text{event}}\frac{\sum_i\mathbf1\{x_i\ge t_j\}}{Y(t_j)}=\sum_{j:\text{event}}1=d.}
$$

This includes each failure subject in its own [risk set](../../../../../risk-set.md). A delayed-entry dataset requires a different risk indicator and is not covered by this particular identity.

Under a [constant hazard survival model](../../../../../constant-hazard-survival-model.md), $\widehat H(x_i)=\widehat\theta x_i$. Imposing the same identity gives the [events divided by exposure estimator](../../../../../events-divided-by-exposure-estimator.md)

$$
\boxed{\widehat\theta=\frac d{\sum_i x_i}=\frac4{40}=0.1\ \text{per time unit}.}
$$

Its fitted [cumulative hazards](../../../../../cumulative-hazard-function.md) at the six times are $0.3,0.4,0.5,0.6,0.9,1.3$, again summing to four. It is also the [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) under independent [right censoring](../../../../../right-censoring.md), since the parameter-dependent [likelihood](../../../../../likelihood-function.md) is $\theta^d e^{-\theta\sum_i x_i}$. This is a sensible estimate if the exponential survival model is appropriate, but four failures give little precision. The event-count identity by itself does not validate constant hazard; the large final jump in the [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md) also reflects a [risk set](../../../../../risk-set.md) of one, rather than by itself proving an increasing hazard.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
