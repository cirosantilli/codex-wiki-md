<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A useful finite-horizon form of the [Girsanov theorem](../../../../../girsanov-theorem.md) is as follows. Let $W$ be a [Brownian motion](../../../../../brownian-motion-split.md) and $\eta$ an adapted, [progressively measurable process](../../../../../progressive-measurability.md) with $\int_0^T\eta_s^2ds<\infty$ almost surely. Suppose its [stochastic exponential](../../../../../doleans-dade-exponential.md)

$$
Z_t=\exp\left(-\int_0^t\eta_s\,dW_s-\frac12\int_0^t\eta_s^2ds\right)
$$

is a true [martingale](../../../../../martingale-split.md) with mean one. The [Novikov condition](../../../../../novikov-s-condition.md) $\mathbb E\exp(\frac12\int_0^T\eta_s^2ds)<\infty$ is a sufficient condition. Under the [equivalent probability measure](../../../../../equivalent-probability-measure.md) $dQ=Z_TdP$, the process $W_t^Q=W_t+\int_0^t\eta_sds$ is a [Brownian motion](../../../../../brownian-motion-split.md).

For the proof sketch, the [Itô formula](../../../../../ito-s-lemma.md) gives $dZ=-Z\eta\,dW$. Integration by parts cancels the drift in $d(ZW^Q)$, since $Z\eta\,dt$ from $dW^Q$ cancels $d[Z,W^Q]=-Z\eta\,dt$. After localization, the [Bayes formula for conditional expectation](../../../../../bayes-formula-for-conditional-expectation.md) makes $W^Q$ a [continuous local martingale](../../../../../continuous-local-martingale.md) under $Q$. Its [quadratic variation](../../../../../quadratic-variation.md) is still $t$, because adding a [finite-variation process](../../../../../finite-variation-process.md) does not change quadratic variation. One can see the Brownian conclusion directly: for real $z$, the [Itô formula](../../../../../ito-s-lemma.md) makes $\exp(izW_t^Q+z^2t/2)$ a local martingale. Its modulus is bounded on the fixed horizon, so it is a true martingale. Thus

$$
\mathbb E_Q[e^{iz(W_t^Q-W_s^Q)}\mid\mathcal F_s]=e^{-z^2(t-s)/2}.
$$

This is the conditional [characteristic function](../../../../../characteristic-function.md) of a centered [normal distribution](../../../../../normal-distribution.md) with variance $t-s$, independent of the past. Continuity and these independent normal increments give the defining properties of [Brownian motion](../../../../../brownian-motion-split.md).

Now put $\phi_t(x)=(2\pi t)^{-1/2}e^{-x^2/(2t)}$ and $\Phi(z)=\int_{-\infty}^z\phi_1(x)dx$, the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). At zero drift the endpoint density of paths staying below $a$ is

$$
P(W_t\in dx,\ \sup_{s\leq t}W_s<a)=\{\phi_t(x)-\phi_t(2a-x)\}\,dx,\qquad x<a.
$$

Indeed, reflect the portion of a path after its first hitting time of $a$. By continuity and the independent symmetric [Brownian motion](../../../../../brownian-motion-split.md) increments after this stopping time, reflection preserves its probability law and maps a crossing path ending at $x<a$ to a path ending at $2a-x>a$. This subtracts exactly $\phi_t(2a-x)$ from the unrestricted endpoint density; it is the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md).

Taking the constant drift tilt $dQ/dP=e^{\mu W_t-\mu^2t/2}$ in the [Girsanov theorem](../../../../../girsanov-theorem.md) makes $W$ under $Q$ have the same law as $W+\mu s$ under $P$. Therefore the desired [finite-horizon maximum of Brownian motion with drift](../../../../../finite-horizon-maximum-of-brownian-motion-with-drift.md) has probability

$$
\int_{-\infty}^a e^{\mu x-\mu^2t/2}\{\phi_t(x)-\phi_t(2a-x)\}\,dx.
$$

Completing squares gives $e^{\mu x-\mu^2t/2}\phi_t(x)=\phi_t(x-\mu t)$ and $e^{\mu x-\mu^2t/2}\phi_t(2a-x)=e^{2\mu a}\phi_t(x-2a-\mu t)$. Hence

$$
\boxed{P\left(\sup_{s\leq t}(W_s+\mu s)\leq a\right)=\Phi\left(\frac{a-\mu t}{\sqrt t}\right)-e^{2\mu a}\Phi\left(\frac{-a-\mu t}{\sqrt t}\right).}
$$

The maximum has no atom at a positive level, so strict and weak barrier inequalities agree. This also follows from continuity of the displayed distribution function. At $\mu=0$ the formula reduces to $2\Phi(a/\sqrt t)-1$.

For the [up-and-out power claim](../../../../../up-and-out-power-claim.md), write $T=t_0>0$ and use the [risk-neutral measure](../../../../../risk-neutral-measure.md) for the [Black-Scholes model](../../../../../black-scholes-model.md), under which

$$
S_t=S_0\exp\left(\sigma W_t+(\rho-\tfrac12\sigma^2)t\right),\qquad
A=\frac{\log(c/S_0)}{\sigma},\qquad m_0=\frac{\rho-\sigma^2/2}{\sigma},
$$

with $\sigma>0$. The barrier survives exactly when $\sup_{t\leq T}(W_t+m_0t)<A$. Its [risk-neutral pricing](../../../../../risk-neutral-pricing.md) value is

$$
V_0=S_0^2e^{(\rho+\sigma^2)T}\mathbb E_Q\left[e^{2\sigma W_T-2\sigma^2T}\mathbf1_{\{\sup_{t\leq T}(W_t+m_0t)<A\}}\right].
$$

The factor inside the [expectation](../../../../../expected-value.md) is a mean-one [Exponential martingale for Brownian motion](../../../../../exponential-martingale-for-brownian-motion.md). Under the probability tilted by it, $W_t-2\sigma t$ is a [Brownian motion](../../../../../brownian-motion-split.md), so the barrier process has drift $m=m_0+2\sigma=(\rho+3\sigma^2/2)/\sigma$. Applying the preceding survival formula yields

$$
\boxed{V_0=S_0^2e^{(\rho+\sigma^2)T}\left[\Phi\left(\frac{A-mT}{\sqrt T}\right)-e^{2mA}\Phi\left(\frac{-A-mT}{\sqrt T}\right)\right].}
$$

As $c\to\infty$, the bracket tends to one and the price becomes the discounted second moment $S_0^2e^{(\rho+\sigma^2)T}$. As $c\downarrow S_0$, it tends to zero. If $\sigma=0$, use the deterministic path instead: the price is $S_0^2e^{\rho T}$ when $S_0\max(1,e^{\rho T})<c$, and zero otherwise. At $T=0$, with $c>S_0$, the price is simply $S_0^2$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
