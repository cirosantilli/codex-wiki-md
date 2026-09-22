<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

An [American option](../../../../../../american-option.md) allows exercise at a [stopping time](../../../../../../stopping-time.md) $\tau\in[t,T]$. For its exercise [financial payoff](../../../../../../contingent-claim-payoff.md) $H$, the pricing problem is

$$
\boxed{V(t,S)=\sup_{\tau\in[t,T]}\mathbb E_Q[e^{-r(\tau-t)}H(S_\tau)\mid S_t=S].}
$$

The discounted value is the [Snell envelope](../../../../../../snell-envelope.md) of discounted exercise payoffs. Define the pricing operator

$$
\mathcal LV=V_t+\frac12\sigma^2S^2V_{SS}+rSV_S-rV.
$$

In the continuation region the [Black-Scholes equation](../../../../../../black-scholes-equation.md) holds, $\mathcal LV=0$. In the exercise region $V=H$, while the ability to wait and the [supermartingale](../../../../../../supermartingale.md) property give $\mathcal LV\le0$. Together these conditions are the [obstacle problem](../../../../../../obstacle-problem.md)

$$
\boxed{\max\{H-V,\mathcal LV\}=0,\qquad V(T,S)=H(S).}
$$

Thus an unknown exercise boundary must be found alongside the value. At a regular boundary in the nondegenerate [Itô diffusion](../../../../../../ito-diffusion.md), value matching is $V=H$, and [smooth pasting](../../../../../../smooth-pasting.md) is $V_S=H'$ where the [financial payoff](../../../../../../contingent-claim-payoff.md) is differentiable. A [finite difference method](../../../../../../finite-difference-method.md) or a [binomial options pricing model](../../../../../../binomial-options-pricing-model.md) steps backward taking the larger of continuation and immediate exercise values at each node.

For a non-dividend-paying [American call option](../../../../../../american-call-option.md) with $r\ge0$, [no early exercise of a call without dividends](../../../../../../no-early-exercise-of-a-call-without-dividends.md) follows directly from the European lower bound

$$
C_E(t,S)\ge\max\{S-Ke^{-r(T-t)},0\}\ge(S-K)^+.
$$

At every candidate exercise time, keeping the European call has value at least the immediate exercise [financial payoff](../../../../../../contingent-claim-payoff.md), so early exercise cannot improve the value; the American and European prices coincide. The first inequality follows from [Jensen inequality](../../../../../../jensen-s-inequality.md) or [put-call parity](../../../../../../put-call-parity.md) and nonnegative put value. With $r>0$ an [American put option](../../../../../../american-put-option.md) can benefit from early receipt of its strike at sufficiently low [stock](../../../../../../stock.md) prices, so its exercise boundary is generally nontrivial and its value is at least the European put value. Dividends can make call exercise worthwhile, and negative interest invalidates the stated no-early-exercise call argument.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
