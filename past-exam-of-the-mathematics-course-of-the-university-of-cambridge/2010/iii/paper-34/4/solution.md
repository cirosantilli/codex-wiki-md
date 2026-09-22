<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For individual $i$, let $N_i(t)$ count its observed event by time $t$ and let $Y_i(t)$ indicate membership of the [risk set](../../../../../risk-set.md) immediately before $t$. Set $N=\sum_iN_i$ and $Y=\sum_iY_i$. Under a common [hazard function](../../../../../hazard-function.md) $h(t)$ and [independent censoring](../../../../../independent-censoring.md), a currently at-risk subject has event probability $h(t)dt+o(dt)$ in the next short interval. Summing over the current [risk set](../../../../../risk-set.md) gives the conditional intensity

$$
\mathbb E[dN(t)\mid\mathcal F_{t-}]=Y(t)h(t)dt=Y(t)dH(t).
$$

Equivalently, the event count decomposes as

$$
N(t)=\int_0^tY(u)dH(u)+M(t),
$$

where $M$ is the mean-zero [counting-process martingale](../../../../../counting-process-martingale.md) obtained by subtracting its conditional compensator. Estimating the unknown hazard increment by the observed event increment divided by the [risk set](../../../../../risk-set.md) size gives the [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md)

$$
\boxed{\widehat H(t)=\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dN(u)
=\sum_{a_j\leq t}\frac1{r_j}.}
$$

Here $a_j$ are the distinct observed event times and $r_j=Y(a_j)$ includes the subject who is about to fail. A censored observation affects subsequent [risk sets](../../../../../risk-set.md), but causes no event jump. This is the requested no-ties estimator; tied event counts would produce $d_j/r_j$.

The derivation also identifies the estimation error:

$$
\widehat H(t)-\int_0^t\mathbf1_{\{Y(u)>0\}}\,dH(u)
=\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dM(u).
$$

Thus it estimates $H(t)$ on the time range where individuals remain at risk. It is not exactly unbiased for the entire cumulative hazard after the last risk set disappears. Its usual [Nelson–Aalen variance estimator](../../../../../nelson-aalen-variance-estimator.md) is $\sum_{a_j\leq t}r_j^{-2}$, since the compensator variance increment of the no-ties event process is $Y\,dH$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
