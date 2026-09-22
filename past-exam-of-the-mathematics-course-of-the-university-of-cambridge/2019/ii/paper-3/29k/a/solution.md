<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
d_\pm
=\frac{\log(S_0/K)+(r\pm\sigma^2/2)T}
{\sigma\sqrt T}.
$$

The call payoff is $(S_T-K)^+$, and it is positive when

$$
y\geq
\frac{\log(K/S_0)-(r-\sigma^2/2)T}{\sigma\sqrt T}
=-d_-.
$$

Writing $\phi$ for the [standard normal density](../../../../../../standard-normal-density.md), the given [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) formula becomes

$$
\begin{aligned}
C_0
&=e^{-rT}\int_{-d_-}^{\infty}
\left[S_0e^{\sigma\sqrt T y+(r-\sigma^2/2)T}-K\right]
\phi(y)\,dy.
\end{aligned}
$$

Completing the square gives

$$
e^{\sigma\sqrt T y}\phi(y)
=e^{\sigma^2T/2}\phi(y-\sigma\sqrt T),
$$

so the two tail integrals are $\Phi(d_+)$ and $\Phi(d_-)$, where $\Phi$ is the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). Therefore the [Black-Scholes formula](../../../../../../black-scholes-formula.md) is

$$
\boxed{C_0=S_0\Phi(d_+)-Ke^{-rT}\Phi(d_-).}
$$

The payoff identity

$$
(S_T-K)^+-(K-S_T)^+=S_T-K
$$

replicates the call-minus-put position by one stock and borrowing the present value of $K$. Hence [put-call parity](../../../../../../put-call-parity.md) gives

$$
C_0-P_0=S_0-Ke^{-rT},
$$

and therefore

$$
\boxed{
P_0=Ke^{-rT}\Phi(-d_-)-S_0\Phi(-d_+).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
