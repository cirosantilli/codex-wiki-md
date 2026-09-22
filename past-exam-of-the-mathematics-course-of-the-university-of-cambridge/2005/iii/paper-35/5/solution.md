<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $\phi_t(y)=(2\pi t)^{-1/2}e^{-y^2/(2t)}$ be the centered [normal probability density](../../../../../normal-density.md) with [variance](../../../../../variance-split.md) $t$, and take $t>0$. For a zero-drift [Brownian motion](../../../../../brownian-motion-split.md) $B$, reflect the path after its first hit of $a>0$. The [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) identifies endpoints $y<a$ on paths that have hit $a$ with endpoints $2a-y>a$. Thus the endpoint density on paths staying below $a$ is $\phi_t(y)-\phi_t(2a-y)$ for $y<a$.

To introduce drift $\nu$, use the [Girsanov theorem](../../../../../girsanov-theorem.md) with likelihood $e^{\nu B_t-\nu^2t/2}$. The coordinate path then has the law of $W_s^\nu=B_s+\nu s$. Since the likelihood depends only on the endpoint, the joint event in question has probability

$$
\int_{-\infty}^x e^{\nu y-\nu^2t/2}\bigl[\phi_t(y)-\phi_t(2a-y)\bigr]dy.
$$

Completing the two squares gives

$$
e^{\nu y-\nu^2t/2}\phi_t(y)=\phi_t(y-\nu t),\qquad e^{\nu y-\nu^2t/2}\phi_t(2a-y)=e^{2a\nu}\phi_t(y-2a-\nu t).
$$

Consequently the [joint endpoint and maximum law for drifted Brownian motion](../../../../../joint-endpoint-and-maximum-law-for-drifted-brownian-motion.md) is

$$
\boxed{\mathbb P(W_t^\nu\le x,M_t^\nu<a)=\Phi\left(\frac{x-\nu t}{\sqrt t}\right)-e^{2a\nu}\Phi\left(\frac{x-2a-\nu t}{\sqrt t}\right),\quad x\le a.}
$$

The endpoint and the maximum have no relevant atom at the boundary, so the same integral includes $x=a$.

For the [down-and-in claim](../../../../../down-and-in-claim.md), use non-dividend-paying [Black-Scholes model](../../../../../black-scholes-model.md) dynamics under the [risk-neutral measure](../../../../../risk-neutral-measure.md). Put $T=t_0$ and

$$
Y_t=\frac1\sigma\log(S_t/S_0)=W_t^Q+\nu t,\qquad\nu=\frac{\rho-\sigma^2/2}{\sigma},\qquad\ell=\frac1\sigma\log(b/S_0)<0.
$$

Let $\tau_b$ be the first time the [stock](../../../../../stock.md) reaches $b$. If $Y_T\le\ell$, continuity ensures $\tau_b\le T$, so these terminal values contribute the payoff $f(S_T)\mathbf1_{S_T\le b}$. For $y>\ell$, lower-barrier reflection followed by the same exponential tilt gives the endpoint density on paths that have hit the barrier:

$$
\mathbb P_Q(Y_T\in dy,\tau_b\le T)/dy=e^{2\nu\ell}\phi_T(y-2\ell-\nu T).
$$

Indeed at zero drift the reflected density is $\phi_T(y-2\ell)$, and multiplying by $e^{\nu y-\nu^2T/2}$ gives the displayed expression.

Thus the remaining, undiscounted payoff [expectation](../../../../../expected-value.md) is

$$
e^{2\nu\ell}\int_\ell^\infty f(S_0e^{\sigma y})\phi_T(y-2\ell-\nu T)dy.
$$

Set $z=y-2\ell$ and

$$
\boxed{\kappa=(S_0/b)^2>1,\qquad\nu=(\rho-\sigma^2/2)/\sigma.}
$$

Then $e^{2\nu\ell}=\kappa^{-\nu/\sigma}$, $S_0e^{\sigma y}=S_0e^{\sigma z}/\kappa$, and $z>-\ell$ is equivalent to $S_0e^{\sigma z}>\kappa b$. The integration variable $z$ has the ordinary terminal log-price density. Adding the first contribution therefore proves the [static terminal-payoff representation of a down-and-in claim](../../../../../static-terminal-payoff-representation-of-a-down-and-in-claim.md):

$$
\boxed{V_0=e^{-\rho T}\mathbb E_Q[g(S_T)],\qquad g(x)=f(x)\mathbf1_{x\le b}+\kappa^{-\nu/\sigma}f(x/\kappa)\mathbf1_{x>\kappa b}.}
$$

This holds for nonnegative measurable payoffs, and for signed payoffs whenever the [expectations](../../../../../expected-value.md) are absolutely integrable. It is an equality of prices, not equality of pathwise terminal payments.

For the call, write $C(s,c,\tau)$ for the ordinary [European call option](../../../../../european-call-option.md) value, with remaining lifetime $\tau>0$ and strike $c>b$. Before activation take current spot $s>b$. The first term in $g$ is zero because the call pays nothing below $b$. The second term reduces to $\kappa^{-\nu/\sigma-1}(x-\kappa c)^+$, since $\kappa c>\kappa b$. The homogeneity $C(s,\kappa c,\tau)=\kappa C(s/\kappa,c,\tau)$ therefore gives the inactive [down-and-in claim](../../../../../down-and-in-claim.md) value

$$
I(s,\tau)=\left(\frac bs\right)^\alpha C(b^2/s,c,\tau),\qquad\alpha=\frac{2\nu}{\sigma}=\frac{2\rho}{\sigma^2}-1.
$$

At $s=b$ its value is $C(b,c,\tau)$, as required by activation. Its pre-activation [option delta](../../../../../option-delta.md), however, has boundary limit

$$
I_s(b+,\tau)=-\frac\alpha bC(b,c,\tau)-C_s(b,c,\tau),
$$

whereas the active contract's [delta hedge](../../../../../delta-hedge.md) holds $C_s(b,c,\tau)$ shares. The [stock](../../../../../stock.md) holding consequently jumps by

$$
\boxed{\Delta_{\rm after}-\Delta_{\rm before}=2C_s(b,c,\tau)+\frac\alpha bC(b,c,\tau).}
$$

This jump is strictly positive, even for negative interest rates. To verify that there is no exceptional cancellation, put $z=\log(s/b)/\sigma$ and $y=\log(S_T/b)/\sigma$. The density for log-price paths killed at the lower barrier is

$$
e^{\nu(y-z)-\nu^2\tau/2}\bigl[\phi_\tau(y-z)-\phi_\tau(y+z)\bigr],\qquad z,y>0.
$$

The [down-and-out claim](../../../../../down-and-out-claim.md) is the ordinary call minus $I$. Differentiate its value at $z=0+$: the bracket vanishes there and its derivative is $2y\phi_\tau(y)/\tau$. Consequently its derivative with respect to the spot at $b$ is

$$
\frac{e^{-\rho\tau-\nu^2\tau/2}}{\sigma b}\int_{\log(c/b)/\sigma}^{\infty}(be^{\sigma y}-c)e^{\nu y}\frac{2y}{\tau}\phi_\tau(y)dy>0.
$$

This derivative is exactly the displayed delta jump. Thus on reaching the barrier before maturity the number of shares changes discontinuously. The [portfolio](../../../../../investment-portfolio.md) value remains continuous; the bank position changes to finance the share adjustment. Hitting precisely at maturity has probability zero and does not alter this conclusion. This is the [delta jump at activation of a down-and-in call](../../../../../delta-jump-at-activation-of-a-down-and-in-call.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
