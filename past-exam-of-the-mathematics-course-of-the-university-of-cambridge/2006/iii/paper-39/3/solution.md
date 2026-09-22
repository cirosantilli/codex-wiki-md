<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Subtract the boundary slope from the [Brownian motion](../../../../../brownian-motion-split.md): $X_t=B_t-bt$. Then $T_{a,b}$ is the [first-passage time](../../../../../first-passage-time.md) of $X$ to the fixed level $a$. The zero-drift [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) gives

$$
\mathbb P(T_a\leq t)=2\{1-\Phi(a/\sqrt t)\},\qquad
h_0(t)=\frac{a}{\sqrt{2\pi t^3}}e^{-a^2/(2t)}.
$$

Here $\Phi$ is the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). To change the [drift](../../../../../drift-coefficient.md) to $-b$, use the [Girsanov theorem](../../../../../girsanov-theorem.md) on each finite horizon, with density $L_t=\exp(-bB_t-b^2t/2)$. On $\{T_a\leq t\}$, [conditional expectation](../../../../../conditional-expectation.md) at the stopped time gives $\mathbb E[L_t\mid\mathcal F_{T_a}]=L_{T_a}$, because the density is a true [martingale](../../../../../martingale-split.md). Since $B_{T_a}=a$, the [drifted Brownian first-passage density](../../../../../drifted-brownian-first-passage-density.md) is consequently

$$
h_b(s)=e^{-ab-b^2s/2}h_0(s)
=\frac{a}{\sqrt{2\pi s^3}}\exp\left(-\frac{(a+bs)^2}{2s}\right),\qquad s>0.
$$

There may be additional mass at infinite hitting time; the displayed density only describes finite passage. With $e^{-\theta\infty}=0$, apply the given zero-drift [Brownian first-passage Laplace transform](../../../../../brownian-first-passage-laplace-transform.md):

$$
\begin{aligned}
\mathbb E[e^{-\theta T_{a,b}}]
&=e^{-ab}\int_0^\infty e^{-(\theta+b^2/2)s}h_0(s)\,ds\\
&=\boxed{\exp[-a(b+\sqrt{b^2+2\theta})]},\qquad\theta>0.
\end{aligned}
$$

The zero-discount limit is $1$ for $b\leq0$ and $e^{-2ab}$ for $b>0$, so the [hitting probability](../../../../../hitting-probability.md) is less than one precisely when the line moves away with positive slope.

For a direct verification of the [linear-boundary Brownian first-passage distribution](../../../../../linear-boundary-brownian-first-passage-distribution.md), define

$$
F_b(t)=e^{-2ab}\Phi\left(\frac{bt-a}{\sqrt t}\right)+\Phi\left(-\frac{a+bt}{\sqrt t}\right).
$$

Both terms tend to zero as $t\downarrow0$. Let $\phi$ be the [standard normal density](../../../../../standard-normal-density.md). The identity

$$
e^{-2ab}\phi\left(b\sqrt t-\frac a{\sqrt t}\right)
=\phi\left(b\sqrt t+\frac a{\sqrt t}\right)
$$

follows by expanding the two squares. Differentiating the two normal probabilities then gives

$$
F_b'(t)=\phi\left(b\sqrt t+\frac a{\sqrt t}\right)
\left[\frac b{2\sqrt t}+\frac a{2t^{3/2}}-\frac b{2\sqrt t}+\frac a{2t^{3/2}}\right]
=h_b(t).
$$

Since this is the previously derived hitting density and both distribution functions start at zero,

$$
\boxed{\mathbb P(T_{a,b}\leq t)=e^{-2ab}\Phi\left(\frac{bt-a}{\sqrt t}\right)+1-\Phi\left(\frac{a+bt}{\sqrt t}\right).}
$$

This proof applies to every real $b$, including the defective distribution when $b>0$.

For the [barrier digital put](../../../../../barrier-digital-put.md), use the dividend-free [Black-Scholes model](../../../../../black-scholes-model.md) with constant [interest rate](../../../../../interest-rate.md) $\rho$ and [spot volatility](../../../../../spot-volatility.md) $\sigma>0$. Under the [risk-neutral measure](../../../../../risk-neutral-measure.md),

$$
S_t=S_0\exp\left((\rho-\sigma^2/2)t+\sigma W_t^Q\right).
$$

Set $T=t_0$ and

$$
a=\frac{\log(c/S_0)}\sigma>0,\qquad
b=\frac{\sigma^2/2-\rho}\sigma.
$$

Reaching the barrier $c$ is equivalent to $W_t^Q$ reaching $a+bt$. The [contingent claim](../../../../../contingent-claim.md) pays one only on the survival event $\{T_{a,b}>T\}$. [Risk-neutral pricing](../../../../../risk-neutral-pricing.md) therefore gives

$$
\boxed{V_0=e^{-\rho T}\left[\Phi\left(\frac{a+bT}{\sqrt T}\right)-e^{-2ab}\Phi\left(\frac{bT-a}{\sqrt T}\right)\right].}
$$

This is a path-survival price, not the price of a terminal [digital put option](../../../../../digital-put-option.md). Continuity of the [stock](../../../../../stock.md) paths and the absence of an atom in the finite-horizon maximum imply that alternative touching conventions change no price. As $c\to\infty$, the value tends to $e^{-\rho T}$; as $c\downarrow S_0$, it tends to zero. Both checks agree with the survival interpretation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
