<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take bank-account values $B_k=R^k$ with $R>0$, and let the [stock](../../../../../stock.md) multiply independently by $u$ or $d$ at each step, where $0<d<R<u$. Under the physical [probability measure](../../../../../probability-measure.md) $P$, the up probability is $p\in(0,1)$; the [filtration](../../../../../filtration-probability-theory.md) records the successive moves. These assumptions specify the standard [binomial market](../../../../../discrete-time-binomial-market.md). If $R$ lies outside the strict interval $(d,u)$, a long or short stock position financed through the [bank account](../../../../../bank-account.md) gives an [arbitrage](../../../../../arbitrage.md).

The [risk-neutral probability in a binomial market](../../../../../risk-neutral-probability-in-a-binomial-market.md) is fixed by $qu+(1-q)d=R$, giving

$$
\boxed{q=\frac{R-d}{u-d}\in(0,1).}
$$

For successor claim values $V_u,V_d$ at a node with current stock price $S$, solve the two replication equations. The current stock holding and current cash value are

$$
\Delta=\frac{V_u-V_d}{S(u-d)},\qquad
C=\frac{uV_d-dV_u}{R(u-d)}.
$$

The cost of this [replicating portfolio in a binomial market](../../../../../replicating-portfolio-in-a-binomial-market.md) is

$$
\Delta S+C=\frac{qV_u+(1-q)V_d}{R}.
$$

Apply this [backward option pricing](../../../../../backward-option-pricing.md) recursion from any terminal [contingent claim](../../../../../contingent-claim.md) $H$, including claims depending on the whole sequence of moves. It constructs a [self-financing portfolio](../../../../../self-financing-portfolio.md) and proves [market completeness](../../../../../complete-market.md) by induction on the remaining number of periods. Taking successive [conditional expectations](../../../../../conditional-expectation.md) under the measure $Q$ with independent up probability $q$ gives the unique [risk-neutral pricing](../../../../../risk-neutral-pricing.md) value

$$
V_k=R^{-(n-k)}\mathbb E_Q[H\mid\mathcal F_k].
$$

Any other price would give an [arbitrage](../../../../../arbitrage.md) by buying the cheaper of the claim and its replica and selling the dearer.

If $K$ is the number of up moves, a particular path has probabilities $p^K(1-p)^{n-K}$ under $P$ and $q^K(1-q)^{n-K}$ under $Q$. Therefore the [binomial-market probability density](../../../../../binomial-market-probability-density.md), namely the [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md), is

$$
\boxed{Z=\frac{dQ}{dP}=\left(\frac qp\right)^K\left(\frac{1-q}{1-p}\right)^{n-K},\qquad
K=\frac{\log(S_n/(S_0d^n))}{\log(u/d)}.}
$$

This last expression makes $Z$ a function of the terminal [stock](../../../../../stock.md) price. Summing over paths gives $\mathbb E_PZ=1$, and strict positivity proves equivalence of the two [probability measures](../../../../../probability-measure.md).

For unrestricted terminal [portfolio wealth](../../../../../portfolio-wealth.md) $H$, its initial replication cost is $R^{-n}\mathbb E_QH$. Hence feasible wealth satisfies the [state-price budget constraint](../../../../../state-price-budget-constraint.md) $\mathbb E_QH=R^nw_0$. For the stated [exponential utility](../../../../../constant-absolute-risk-aversion-utility.md), $v'(x)=e^{-ax}$ and $v''(x)=-ae^{-ax}<0$. The [binomial exponential-utility terminal wealth](../../../../../binomial-exponential-utility-terminal-wealth.md) is

$$
\boxed{H^*=R^nw_0+\frac{\mathbb E_Q\log Z-\log Z}{a},}
$$

where

$$
\mathbb E_Q\log Z
=n\left[q\log\frac qp+(1-q)\log\frac{1-q}{1-p}\right].
$$

It satisfies the budget, and its [marginal utility](../../../../../marginal-utility.md) is $v'(H^*)=\lambda Z$ with $\lambda=\exp(-aR^nw_0-\mathbb E_Q\log Z)>0$. The [concave supporting-tangent inequality](../../../../../concave-supporting-tangent-inequality.md) gives

$$
v(H)\leq v(H^*)+\lambda Z(H-H^*).
$$

Taking [expectations](../../../../../expected-value.md) under $P$ makes the last term zero by the budget. Strict [concavity](../../../../../concave-function.md) makes equality possible only when $H=H^*$ in every positive-probability state. The already constructed [complete market](../../../../../complete-market.md) supplies its [replicating strategy](../../../../../replicating-strategy.md), so this proves global optimality and uniqueness. The formula allows negative final wealth, as permitted by the unrestricted trading problem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
