<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Here is the Brownian change-of-drift form of the [Girsanov theorem](../../../../../girsanov-theorem.md). Let $W$ be a standard [Brownian motion](../../../../../brownian-motion-split.md) on $[0,T]$ and $\theta$ predictable with $\int_0^T\theta_s^2ds<\infty$ almost surely. Suppose the [stochastic exponential](../../../../../doleans-dade-exponential.md)

$$
Z_t=\exp\left(-\int_0^t\theta_s\,dW_s-\frac12\int_0^t\theta_s^2ds\right)
$$

is a true [martingale](../../../../../martingale-split.md) with $\mathbb EZ_T=1$. Define $dQ=Z_TdP$. Then $Q$ is equivalent to $P$ and

$$
\boxed{W_t^Q=W_t+\int_0^t\theta_sds\text{ is a standard Brownian motion under }Q.}
$$

The same statement holds in $d$ dimensions with scalar products, squared norms and a vector drift. [Novikov's condition](../../../../../novikov-s-condition.md) $\mathbb E\exp(\frac12\int_0^T\theta_s^2ds)<\infty$ is a standard sufficient condition for the true-martingale hypothesis. Bounded $\theta$ is enough for all applications below.

For the proof, [Itô formula](../../../../../ito-s-lemma.md) gives $dZ_t=-Z_t\theta_t\,dW_t$. The [Itô product rule](../../../../../ito-product-rule.md) gives the cancellation

$$
d(Z_tW_t^Q)=W_t^QdZ_t+Z_t(dW_t+\theta_tdt)+d[Z,W]_t
=Z_t(1-\theta_tW_t^Q)dW_t.
$$

The two drift terms cancel because $d[Z,W]_t=-Z_t\theta_tdt$. Stop $W^Q$ when its absolute value reaches $n$, at a time $\tau_n$ capped by $T$. The same product calculation makes $Z_tW_{t\wedge\tau_n}^Q$ a [local martingale](../../../../../local-martingale.md) under $P$. Its absolute value is at most $nZ_t$; the density [martingale](../../../../../martingale-split.md) is uniformly integrable over this finite horizon, so the stopped product is a true [martingale](../../../../../martingale-split.md). Bayes' conditional identity then gives

$$
\mathbb E_Q[W_{t\wedge\tau_n}^Q\mid\mathcal F_s]
=Z_s^{-1}\mathbb E_P[Z_tW_{t\wedge\tau_n}^Q\mid\mathcal F_s]
=W_{s\wedge\tau_n}^Q.
$$

As $n$ increases, these stopping times exhaust the horizon by continuity. Thus $W^Q$ is a continuous [local martingale](../../../../../local-martingale.md) under $Q$. Adding a finite-variation drift does not change [quadratic variation](../../../../../quadratic-variation.md), so $[W^Q]_t=t$.

To prove the Brownian conclusion rather than just assert it, for every real $u$ apply [Itô formula](../../../../../ito-s-lemma.md) to $F_t=\exp(iuW_t^Q+u^2t/2)$. Its differential is $iuF_t\,dW_t^Q$, and its modulus is bounded on the fixed horizon, so it is a true [martingale](../../../../../martingale-split.md). Consequently

$$
\mathbb E_Q[e^{iu(W_t^Q-W_s^Q)}\mid\mathcal F_s]=e^{-u^2(t-s)/2}.
$$

The conditional [characteristic function](../../../../../characteristic-function.md) identifies a centered normal increment with [variance](../../../../../variance-split.md) $t-s$, independent of the past. Together with continuity and $W_0^Q=0$, this proves the Brownian assertion. For vector $u$, the same argument uses $\|u\|^2$ and gives the multivariate version. If $|\theta|\le K$, stopping $Z$ and applying [Itô formula](../../../../../ito-s-lemma.md) to $Z^2$ gives a uniform second-moment bound $\mathbb EZ_{t\wedge\tau}^2\le e^{K^2t}$ by [Gronwall inequality](../../../../../gronwall-inequality.md); this proves uniform integrability of the stopped densities and the needed true-martingale property in the bounded case.

In the [Black-Scholes model](../../../../../black-scholes-model.md) with its usual augmented Brownian [filtration](../../../../../filtration-probability-theory.md), write $dS_t=S_t(\alpha dt+\sigma dW_t)$, $B_t=e^{\rho t}$, with $\sigma>0$. Take $\theta=(\alpha-\rho)/\sigma$, the [market price of risk](../../../../../market-price-of-risk.md). Under $Q$, the preceding change of drift gives

$$
dS_t=\rho S_tdt+\sigma S_t dW_t^Q,
$$

so $S_t/B_t$ is a [martingale](../../../../../martingale-split.md). The [Martingale representation theorem](../../../../../martingale-representation-theorem.md) then makes integrable Brownian-market claims attainable and gives their [risk-neutral pricing](../../../../../risk-neutral-pricing.md) as discounted [conditional expectations](../../../../../conditional-expectation.md). The physical drift $\alpha$ has disappeared from the price dynamics.

For the joint terminal-value and maximum law, first use the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) at level $a>0$. Reflecting a path after its first hit of $a$ preserves its law as a [Brownian motion](../../../../../brownian-motion-split.md) and sends a terminal value $y<a$ to $2a-y>a$; the symmetry and strong Markov property of the post-hit increments justify this map. Thus, with $\varphi_t(y)=(2\pi t)^{-1/2}e^{-y^2/(2t)}$,

$$
P(W_t\in dy,\ \sup_{s\le t}W_s<a)
=[\varphi_t(y)-\varphi_t(2a-y)]\,dy\quad(y<a).
$$

Take the constant-drift exponential density $e^{\mu W_t-\mu^2t/2}$. By [Girsanov theorem](../../../../../girsanov-theorem.md), the coordinate process under this tilted measure has the law of $W_s+\mu s$ under $P$. Consequently, for $t>0$ and $x\le a$,

$$
P(W_t^\mu\le x,M_t^\mu<a)
=\int_{-\infty}^x e^{\mu y-\mu^2t/2}[\varphi_t(y)-\varphi_t(2a-y)]\,dy.
$$

Completing the squares gives

$$
e^{\mu y-\mu^2t/2}\varphi_t(y)=\varphi_t(y-\mu t),\qquad
e^{\mu y-\mu^2t/2}\varphi_t(2a-y)=e^{2a\mu}\varphi_t(y-2a-\mu t).
$$

Integrating proves

$$
\boxed{P(W_t^\mu\le x,M_t^\mu<a)=
\Phi\!\left(\frac{x-\mu t}{\sqrt t}\right)
-e^{2a\mu}\Phi\!\left(\frac{x-2a-\mu t}{\sqrt t}\right).}
$$

Here $\Phi$ is the standard normal distribution function. The first variable is the terminal Brownian value, distinct from its running maximum.

Set $T=t_0$, $a=\log(b/S_0)/\sigma>0$ and $\mu=(\rho-\sigma^2/2)/\sigma$. Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), $\log(S_s/S_0)/\sigma=W_s^Q+\mu s$. Taking $x=a$ in the joint law gives the [probability](../../../../../probability.md) of not hitting the upper level. Complementing it and discounting the unit payment at maturity gives the [one-touch option](../../../../../one-touch-option.md) price

$$
\boxed{V_0=e^{-\rho T}\left[
\Phi\!\left(\frac{\mu T-a}{\sqrt T}\right)
+e^{2a\mu}\Phi\!\left(\frac{-a-\mu T}{\sqrt T}\right)\right].}
$$

The exponential weight is also $(b/S_0)^{2\rho/\sigma^2-1}$. The payment occurs at $T$, even if the barrier was hit earlier, so its discount factor is $e^{-\rho T}$, not a hitting-time discount factor.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
