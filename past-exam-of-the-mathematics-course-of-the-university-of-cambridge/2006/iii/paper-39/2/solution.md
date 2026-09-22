<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let the one-period riskless gross return be $R>0$, with $0<d<R<u$, and let the physical up probability be $\pi\in(0,1)$. The [binomial market](../../../../../discrete-time-binomial-market.md) has [risk-neutral probability](../../../../../risk-neutral-probability.md)

$$
q=\frac{R-d}{u-d}\in(0,1),\qquad qu+(1-q)d=R.
$$

Under its [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q$, successive multipliers $J_k$ are independent, taking $u,d$ with probabilities $q,1-q$. The [risk-neutral pricing](../../../../../risk-neutral-pricing.md) function has the extension

$$
g_r(s)=R^{-(n-r)}\mathbb E_Q\left[f\left(s\prod_{k=r+1}^nJ_k\right)\right],\qquad s>0.
$$

For every fixed positive multiplier $A$, the function $s\mapsto f(As)$ is [convex](../../../../../convex-function.md) when $f$ is [convex](../../../../../convex-function.md). Taking a positive weighted sum preserves [convexity](../../../../../convex-function.md). More explicitly, for $0\leq\lambda\leq1$,

$$
g_r(\lambda s+(1-\lambda)t)\leq\lambda g_r(s)+(1-\lambda)g_r(t).
$$

Thus the pricing extension is [convex](../../../../../convex-function.md), and so are its values on the attainable stock-price grid.

The [replicating portfolio in a binomial market](../../../../../replicating-portfolio-in-a-binomial-market.md) holds

$$
\Delta_r(s)=\frac{g_{r+1}(us)-g_{r+1}(ds)}{(u-d)s}
$$

shares over the next interval. If $r+1<n$, put $A=\Delta_{r+1}(us)$ and $D=\Delta_{r+1}(ds)$. These are the secant slopes of $g_{r+2}$ on $[uds,u^2s]$ and $[d^2s,uds]$, respectively. For a [convex function](../../../../../convex-function.md), the slope of a secant on a later adjacent interval is no smaller than that on the earlier interval: apply the defining [convexity](../../../../../convex-function.md) inequality to the middle point $uds$, then rearrange. Hence $A\geq D$. Using [backward option pricing](../../../../../backward-option-pricing.md) twice gives

$$
\begin{aligned}
g_{r+1}(us)-g_{r+1}(ds)
&=R^{-1}\left[q\{g_{r+2}(u^2s)-g_{r+2}(uds)\}+(1-q)\{g_{r+2}(uds)-g_{r+2}(d^2s)\}\right],\\
\Delta_r(s)&=\frac{qu}{R}A+\frac{(1-q)d}{R}D.
\end{aligned}
$$

The two coefficients are positive and sum to one. Therefore [convex-payoff delta monotonicity in a binomial market](../../../../../convex-payoff-delta-monotonicity-in-a-binomial-market.md) yields

$$
\boxed{\Delta_{r+1}(us)\geq\Delta_r(s)\geq\Delta_{r+1}(ds).}
$$

In particular an up move cannot reduce the [stock](../../../../../stock.md) holding. “Increases” here means nondecreases: an affine payoff gives equality, so strict increase cannot be claimed for every [convex](../../../../../convex-function.md) payoff.

For the [expected utility maximization](../../../../../expected-utility-maximization.md) problem, let $P$ be the physical measure and $Z=dQ/dP$ on terminal paths. If a path has $j$ up moves, its [binomial-market probability density](../../../../../binomial-market-probability-density.md) is

$$
Z_j=\left(\frac q\pi\right)^j\left(\frac{1-q}{1-\pi}\right)^{n-j}.
$$

Every terminal payoff is replicable in this [complete market](../../../../../complete-market.md). Buying a positive payoff $H$ with initial wealth $w_0$ therefore imposes the [state-price budget constraint](../../../../../state-price-budget-constraint.md) $\mathbb E_QH=R^nw_0$. Since the [utility function](../../../../../utility-function-split.md) is increasing, the full budget is used. Its derivative and second derivative are

$$
v'(x)=x^{-(\gamma-1)/\gamma},\qquad
v''(x)=-\frac{\gamma-1}{\gamma}x^{-(2\gamma-1)/\gamma}<0.
$$

Put $a=\gamma/(\gamma-1)$. The first-order condition $v'(H_*)=\lambda Z$ for a positive multiplier $\lambda$ gives $H_*=C Z^{-a}$. The budget determines $C$ uniquely. Independence of the successive moves gives

$$
D:=\mathbb E_QZ^{-a}
=\left[q\left(\frac q\pi\right)^{-a}+(1-q)\left(\frac{1-q}{1-\pi}\right)^{-a}\right]^n.
$$

Thus the optimal claim, as a function of the number of up moves, is

$$
\boxed{H_*(j)=\frac{R^nw_0}{D}
\left(\frac\pi q\right)^{aj}
\left(\frac{1-\pi}{1-q}\right)^{a(n-j)}.}
$$

Because $S_n=S_0u^jd^{n-j}$ uniquely determines $j$, this is also a terminal-stock-price payoff, attainable by [backward option pricing](../../../../../backward-option-pricing.md) and [claim replication](../../../../../claim-replication.md). It rewards states relatively more probable under the investor's physical measure than under the pricing measure. If $\pi=q$, the optimum is the riskless payoff $R^nw_0$.

To prove global optimality rather than merely assert a stationary point, use the tangent inequality for the strictly [concave function](../../../../../concave-function.md) $v$:

$$
v(H)\leq v(H_*)+v'(H_*)(H-H_*)=v(H_*)+\lambda Z(H-H_*).
$$

Taking physical [expectations](../../../../../expected-value.md) makes the last term zero for any fully financed competing claim, and nonpositive for any claim costing less. Therefore $\mathbb E_Pv(H)\leq\mathbb E_Pv(H_*)$, with equality only when $H=H_*$ almost surely. Finiteness causes no difficulty on the finite binomial tree, and $H_*>0$ in every terminal state.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
