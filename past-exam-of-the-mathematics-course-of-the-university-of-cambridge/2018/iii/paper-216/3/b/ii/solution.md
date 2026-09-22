<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Given the parameters and $Z$, the coordinates are conditionally independent. Write $m_i=x_i^T\beta+\sigma^2Z_i$, $v=\sigma_0^2$, and let $y_i$ denote the observed count. Their full [conditional distributions](../../../../../../../conditional-distribution.md) have scalar densities

$$
\boxed{q_i(t)\propto\exp\left[y_it-n_i\log(1+e^t)-\frac{(t-m_i)^2}{2v}\right],\qquad t\in\mathbb R.}
$$

Each is proper: the [binomial distribution](../../../../../../../binomial-distribution.md) likelihood factor is bounded, and the remaining factor is a proper [normal distribution](../../../../../../../normal-distribution.md) density.

One completely specified exact algorithm is [rejection sampling](../../../../../../../rejection-sampling.md) from $N(m_i,v)$. Define

$$
H_i(t)=\frac{e^{y_it}}{(1+e^t)^{n_i}},\qquad
M_i=\sup_tH_i(t).
$$

For $0<y_i<n_i$,

$$
M_i=\left(\frac{y_i}{n_i}\right)^{y_i}
\left(1-\frac{y_i}{n_i}\right)^{n_i-y_i};
$$

for $y_i=0$ or $y_i=n_i$, take $M_i=1$, and for $n_i=0$ take $H_i=M_i=1$. Propose $t\sim N(m_i,v)$ and accept with probability $H_i(t)/M_i$, repeating until acceptance. The accepted density is proportional to the proposal times $H_i$, exactly $q_i$. Its acceptance probability is positive, so it terminates almost surely, although it can be inefficient.

An efficient exact alternative is [adaptive rejection sampling](../../../../../../../adaptive-rejection-sampling.md). The log density has

$$
\ell_i'(t)=y_i-n_i\frac{e^t}{1+e^t}-\frac{t-m_i}{v},\qquad
\ell_i''(t)=-n_i\frac{e^t}{(1+e^t)^2}-\frac1v<0.
$$

Thus it is a [log-concave probability density](../../../../../../../log-concave-probability-density.md). Choose one tangent point with positive derivative in the left tail and one with negative derivative in the right tail; these exist because the Gaussian term dominates there. Their tangent upper hull gives an integrable piecewise exponential rejection envelope. Sample that envelope, accept using the target-to-envelope ratio, and add evaluated points to improve it. Concavity guarantees the upper bound, so accepted samples remain exact. Sample each coordinate independently by either method; a finite number of Metropolis steps would not provide the requested exact draws.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 216](../../../../paper-216-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
