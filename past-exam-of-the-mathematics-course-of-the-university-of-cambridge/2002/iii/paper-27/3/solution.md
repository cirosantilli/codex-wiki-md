<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For real $\lambda$, the [normal](../../../../../normal-distribution.md) moment-generating formula gives $\mathbb E e^{\lambda(B_t-B_s)}=e^{\lambda^2(t-s)/2}$. Using [independent increments](../../../../../independent-increments.md) and conditioning on the Brownian [filtration](../../../../../filtration-probability-theory.md),

$$
\mathbb E\left[e^{\lambda B_t-\lambda^2t/2}\mid\mathcal F_s\right]
=e^{\lambda B_s-\lambda^2t/2}e^{\lambda^2(t-s)/2}
=e^{\lambda B_s-\lambda^2s/2}.
$$

All terms are integrable by the same [normal](../../../../../normal-distribution.md) formula. Thus the displayed process is an [Exponential martingale for Brownian motion](../../../../../exponential-martingale-for-brownian-motion.md).

For the interval exit time, we first show both almost-sure finiteness and finite expectation. On $\{T>n\}$, the position at time $n$ lies in $(-b,a)$. If $X_{n+1}-X_n\ge a+b$, the continuous path must exit by time $n+1$. This increment is [independent](../../../../../independent-random-variables.md) of $\mathcal F_n$ and has law $N(\mu,1)$, so the conditional probability of this event is a fixed $c>0$. Therefore

$$
\mathbb P(T>n+1)\le(1-c)\mathbb P(T>n),
\qquad \mathbb P(T>n)\le(1-c)^n.
$$

This [geometric tail bound from a uniform escape probability](../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) implies $T<\infty$ almost surely and $\mathbb ET<\infty$.

Take $\lambda=-2\mu$. Then $e^{-2\mu X_t}=e^{-2\mu B_t-2\mu^2t}$ is the exponential [martingale](../../../../../martingale-split.md) just proved. Its stopped values lie between $e^{-2\mu a}$ and $e^{2\mu b}$. The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $T\wedge t$, followed by bounded convergence, gives $\mathbb E e^{-2\mu X_T}=1$. With $v=\mathbb P(X_T=a)$ and the two possible boundary values,

$$
v e^{-2\mu a}+(1-v)e^{2\mu b}=1.
$$

Solving yields

$$
\boxed{\mathbb P(X_T=a)=\frac{1-e^{-2\mu b}}{1-e^{-2\mu(a+b)}}.}
$$

Next apply bounded-time [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $B_t$. Since $B_{T\wedge t}=X_{T\wedge t}-\mu(T\wedge t)$, we obtain $\mathbb EX_{T\wedge t}=\mu\mathbb E(T\wedge t)$. The stopped position is bounded, and the stopped time increases to an integrable $T$. Passing to the limit gives $\mu\mathbb ET=av-b(1-v)$. Therefore

$$
\boxed{\mathbb ET=\frac1\mu\left[(a+b)\frac{1-e^{-2\mu b}}{1-e^{-2\mu(a+b)}}-b\right].}
$$

As a check, letting $\mu\downarrow0$ gives the driftless formulas $v\to b/(a+b)$ and $\mathbb ET\to ab$. The expectation calculation uses a justified stopping limit, rather than assuming that [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) holds at every unbounded time.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
