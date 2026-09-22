<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [Brownian first-passage time](../../../../../brownian-first-passage-time.md) to a line, set $\lambda=\theta>0$ and choose $h=b+\sqrt{b^2+2\lambda}>0$, so $h^2/2-bh=\lambda$. The [Exponential martingale for Brownian motion](../../../../../exponential-martingale-for-brownian-motion.md) $M_s=e^{hW_s-h^2s/2}$, stopped at $T_{a,b}$, obeys

$$
0\leq M_{s\wedge T_{a,b}}\leq e^{ha}e^{-\lambda(s\wedge T_{a,b})}.
$$

The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at the bounded time $s\wedge T_{a,b}$ gives expectation one. The contribution from $\{T_{a,b}>s\}$ is at most $e^{ha-\lambda s}$, and tends to zero. Taking $e^{-\lambda\infty}=0$ therefore yields

$$
\boxed{\mathbb E e^{-\theta T_{a,b}}=e^{-a(b+\sqrt{b^2+2\theta})},\qquad b\in\mathbb R.}
$$

Letting $\theta\downarrow0$ shows that the hitting probability is one for $b\leq0$ and $e^{-2ab}$ for $b>0$; in the latter case the hitting-time law has mass at infinity.

To derive the finite-time [linear-boundary Brownian first-passage distribution](../../../../../linear-boundary-brownian-first-passage-distribution.md), put $Z_s=W_s-bs$. This is [Brownian motion](../../../../../brownian-motion-split.md) with drift $\mu=-b$, and the event is $\{\sup_{s\leq t}Z_s\geq a\}$. For driftless [Brownian motion](../../../../../brownian-motion-split.md), the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) says that the joint endpoint density on this event equals the normal density $p_t(x)$ when $x\geq a$ and the reflected density $p_t(2a-x)$ when $x<a$, where $p_t(x)=(2\pi t)^{-1/2}e^{-x^2/(2t)}$. The constant-drift change of measure weights these densities by $e^{\mu x-\mu^2t/2}$. Thus the crossing probability is

$$
\int_a^\infty e^{\mu x-\mu^2t/2}p_t(x)\,dx+\int_{-\infty}^a e^{\mu x-\mu^2t/2}p_t(2a-x)\,dx.
$$

Completing the square gives respectively $\Phi((\mu t-a)/\sqrt t)$ and $e^{2\mu a}\Phi((-\mu t-a)/\sqrt t)$. Substituting $\mu=-b$ proves

$$
\boxed{\mathbb P(T_{a,b}\leq t)=e^{-2ab}\Phi\!\left(\frac{bt-a}{\sqrt t}\right)+1-\Phi\!\left(\frac{a+bt}{\sqrt t}\right).}
$$

The density weighting follows directly from the [Exponential martingale for Brownian motion](../../../../../exponential-martingale-for-brownian-motion.md), or the [Girsanov theorem](../../../../../girsanov-theorem.md), on the fixed finite horizon; it does not require eventual hitting.

For the [barrier digital call](../../../../../barrier-digital-call.md), under the [risk-neutral measure](../../../../../risk-neutral-measure.md) in the [Black-Scholes model](../../../../../black-scholes-model.md),

$$
\log(S_s/S_0)=(\rho-\sigma^2/2)s+\sigma W_s^Q.
$$

Assume $\sigma>0$, put $a=\log(c/S_0)/\sigma>0$ and $b=-(\rho-\sigma^2/2)/\sigma$. The upper stock barrier is reached exactly when $W_s^Q$ reaches $a+bs$. The payment is at the fixed maturity $t_0$, not at the random hitting time. Hence its price is

$$
\boxed{V_0=e^{-\rho t_0}\left[e^{-2ab}\Phi\!\left(\frac{bt_0-a}{\sqrt{t_0}}\right)+1-\Phi\!\left(\frac{a+bt_0}{\sqrt{t_0}}\right)\right].}
$$

If $\sigma=0$, use the deterministic path $S_s=S_0e^{\rho s}$ instead: the value is $e^{-\rho t_0}$ if that path reaches $c$ by $t_0$, and zero otherwise. The nondegenerate formula concerns the usual positive-volatility model.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
