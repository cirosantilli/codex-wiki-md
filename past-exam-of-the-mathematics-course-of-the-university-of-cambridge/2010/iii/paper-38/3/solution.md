<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $C_t$ be the cumulative claim amount and $U_t=u+ct-C_t$ the surplus in the [classical risk model](../../../../../classical-risk-model.md). The supplied [adjustment coefficient](../../../../../adjustment-coefficient.md) satisfies $\lambda(M_X(R)-1)=cR$. The [Compound Poisson process](../../../../../compound-poisson-process.md) has independent increments, and the [random-sum transform identity](../../../../../random-sum-transform-identity.md) gives

$$
\mathbb E[e^{R(C_t-C_s)}]=\exp((t-s)\lambda(M_X(R)-1)).
$$

It follows that $Z_t=\exp(R(C_t-ct))$ is a nonnegative [martingale](../../../../../martingale-split.md) with $Z_0=1$: conditional on the past, the multiplicative increment has [expected value](../../../../../expected-value.md) one. This is the [exponential surplus martingale](../../../../../exponential-surplus-martingale.md).

Let $\tau=\inf\{t\ge0:U_t<0\}$ be the ruin [stopping time](../../../../../stopping-time.md). Surplus decreases only at claim arrivals, so on $\{\tau\le t\}$ the deficit at ruin gives $C_\tau-c\tau>u$ and $Z_\tau>e^{Ru}$. The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at the bounded [stopping time](../../../../../stopping-time.md) $\tau\wedge t$ yields

$$
1=\mathbb E Z_{\tau\wedge t}\ge\mathbb E[Z_\tau\mathbf1_{\{\tau\le t\}}]
\ge e^{Ru}\mathbb P(\tau\le t).
$$

As $t$ increases without bound, the events $\{\tau\le t\}$ increase to eventual ruin. Hence the [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) satisfies the [Lundberg inequality](../../../../../lundberg-inequality.md)

$$
\boxed{\psi(u)=\mathbb P(\tau<\infty)\le e^{-Ru},\qquad u\ge0.}
$$

The proof uses only bounded-time stopping; it does not presume that the [martingale](../../../../../martingale-split.md) can be stopped with equality of [expected values](../../../../../expected-value.md) at an unbounded ruin time.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
