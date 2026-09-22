<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\phi_T(y)=(2\pi T)^{-1/2}e^{-y^2/(2T)}$ be the [normal distribution](../../../../../normal-distribution.md) density. The [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) gives the killed endpoint density

$$
\mathbb P(W_T\in dy,\ \sup_{s\leq T}W_s<a)
=[\phi_T(y)-\phi_T(y-2a)]\,dy,\qquad y<a.
$$

Indeed, reflection after the first hit of $a$ maps paths ending below $a$ that have hit the barrier to paths ending at $2a-y$; symmetry gives $\phi_T(2a-y)=\phi_T(y-2a)$.

By the [Girsanov theorem](../../../../../girsanov-theorem.md), weighting the path law by $\exp(\nu W_T-\nu^2T/2)$ makes the coordinate process a [Brownian motion with drift](../../../../../brownian-motion-with-drift.md) $\nu$. Completing the two squares yields

$$
e^{\nu y-\nu^2T/2}[\phi_T(y)-\phi_T(y-2a)]
=\phi_T(y-\nu T)-e^{2a\nu}\phi_T(y-2a-\nu T).
$$

Integration up to $x\leq a$ proves the [joint endpoint and maximum law for drifted Brownian motion](../../../../../joint-endpoint-and-maximum-law-for-drifted-brownian-motion.md):

$$
\boxed{\mathbb P(W_T^\nu\leq x,M_T^\nu<a)
=\Phi\left(\frac{x-\nu T}{\sqrt T}\right)
-e^{2a\nu}\Phi\left(\frac{x-2a-\nu T}{\sqrt T}\right).}
$$

Here $\Phi$ is the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). Setting $x=a$ also gives a continuous barrier distribution, so equality at the barrier has zero [probability](../../../../../probability.md).

For the [up-and-in option](../../../../../up-and-in-claim.md), use the [risk-neutral measure](../../../../../risk-neutral-measure.md) of the [Black-Scholes model](../../../../../black-scholes-model.md) with [interest rate](../../../../../interest-rate.md) $\rho$ and [spot volatility](../../../../../spot-volatility.md) $\sigma>0$. Then

$$
S_t=S_0e^{\sigma(W_t+\nu t)},\qquad
\nu=\frac{\rho-\sigma^2/2}{\sigma},\qquad
a=\frac{\log(b/S_0)}{\sigma}>0.
$$

Above $a$, the barrier has certainly been reached. Below $a$, subtracting the killed density from the unrestricted endpoint density leaves $e^{2a\nu}\phi_T(y-2a-\nu T)$. Thus the discounted [expected value](../../../../../expected-value.md) of its payoff is

$$
e^{-\rho T}\left[\int_a^\infty f(S_0e^{\sigma y})\phi_T(y-\nu T)\,dy
+e^{2a\nu}\int_{-\infty}^a f(S_0e^{\sigma y})\phi_T(y-2a-\nu T)\,dy\right].
$$

In the second integral put $z=y-2a$, and define

$$
\boxed{\kappa=e^{-2\sigma a}=\left(\frac{S_0}{b}\right)^2.}
$$

Then $S_0e^{\sigma y}=S_0e^{\sigma z}/\kappa$, $z\leq-a$ means $S_0e^{\sigma z}\leq\kappa b$, and $e^{2a\nu}=\kappa^{-\nu/\sigma}$. Both integrals now use the unrestricted terminal [stock](../../../../../stock.md) distribution. This proves that the [reflected European payoff for an up-and-in option](../../../../../reflected-european-payoff-for-an-up-and-in-option.md) is

$$
\boxed{g(x)=f(x)\mathbf1_{\{x>b\}}+\kappa^{-\nu/\sigma}f(x/\kappa)\mathbf1_{\{x\leq\kappa b\}}.}
$$

Their initial [risk-neutral pricing](../../../../../risk-neutral-pricing.md) values agree for payoffs with finite absolute expectations in these integrals. The identity concerns prices; the two terminal payoffs need not agree along individual paths.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
