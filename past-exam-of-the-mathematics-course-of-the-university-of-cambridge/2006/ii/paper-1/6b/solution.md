<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The [probability generating function](../../../../../probability-generating-function.md) encodes the population distribution in one analytic function. Its coefficients and [derivative](../../../../../derivative.md) recover

$$
P(n,t)=\frac1{n!}\partial_s^n\phi(0,t),\qquad\langle n\rangle=\partial_s\phi(1,t),
$$

provided the mean is finite. Higher [derivatives](../../../../../derivative.md) at one give [factorial moments](../../../../../factorial-moment.md), and normalization says $\phi(1,t)=1$.

Interpret the supplied birth and death expressions as [transition rates](../../../../../transition-intensity.md): over a small time $dt$ their [probabilities](../../../../../probability.md) are $(\alpha+\beta n)dt+o(dt)$ and $\gamma n\,dt+o(dt)$. Incoming [probability](../../../../../probability.md) from $n-1$ and $n+1$, minus both outgoing rates, gives

$$
\partial_tP(n,t)=(\alpha+\beta(n-1))P(n-1,t)+\gamma(n+1)P(n+1,t)-[\alpha+(\beta+\gamma)n]P(n,t),
$$

with $P(-1,t)=0$. Multiplying by $s^n$ and summing yields

$$
\boxed{\phi_t=\alpha(s-1)\phi+(s-1)(\beta s-\gamma)\phi_s.}
$$

At stationarity, $\phi_s/\phi=\alpha/(\gamma-\beta s)$, so [integration](../../../../../integral.md) and normalization give

$$
\boxed{\phi(s)=\left(\frac{\gamma-\beta}{\gamma-\beta s}\right)^{\alpha/\beta},\qquad\langle n\rangle=\frac{\alpha}{\gamma-\beta}.}
$$

Alternatively differentiating the evolution equation at one gives $m'=\alpha-(\gamma-\beta)m$, so $m(t)=\alpha/(\gamma-\beta)+[m(0)-\alpha/(\gamma-\beta)]e^{-(\gamma-\beta)t}$. If $\beta=0$, the displayed power expression is understood in its limit: $\phi(s)=e^{(\alpha/\gamma)(s-1)}$, a [Poisson distribution](../../../../../poisson-distribution.md) with mean $\alpha/\gamma$.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
