<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take a riskless gross return $R>0$ per period and a [stock](../../../../../stock.md) whose independent multiplicative moves are $u$ and $d$, with physical up probability $p\in(0,1)$. Assume $0<d<R<u$. With $K_k$ up moves by date $k$,

$$
B_k=R^k,\qquad S_k=S_0u^{K_k}d^{k-K_k}.
$$

A [self-financing portfolio](../../../../../self-financing-portfolio.md) chooses each [stock](../../../../../stock.md) holding from information available before the next move, and invests the remainder in the [bank account](../../../../../bank-account.md). At any node the two possible next payoffs can be matched by two holdings because $u\ne d$. Backward induction therefore makes the [binomial market](../../../../../discrete-time-binomial-market.md) complete.

The unique [risk-neutral probability](../../../../../risk-neutral-probability.md) of an up move is determined by the discounted-stock [martingale](../../../../../martingale-split.md) equation:

$$
qu+(1-q)d=R,\qquad\boxed{q=\frac{R-d}{u-d}\in(0,1).}
$$

The [risk-neutral measure](../../../../../risk-neutral-measure.md) assigns product probabilities to the successive moves. A path with $K=K_n$ up moves has physical probability $p^K(1-p)^{n-K}$ and pricing probability $q^K(1-q)^{n-K}$. Its [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md) is therefore

$$
Z=\frac{dQ}{dP}=\left(\frac qp\right)^K\left(\frac{1-q}{1-p}\right)^{n-K}.
$$

Since $S_n=S_0d^n(u/d)^K$, eliminate $K$ to obtain the requested terminal-price expression:

$$
\boxed{Z=\left(\frac{1-q}{1-p}\right)^n\left(\frac{S_n}{S_0d^n}\right)^\beta,\qquad\beta=\frac{\log\!\left(q(1-p)/(p(1-q))\right)}{\log(u/d)}.}
$$

The pricing density depends only on the terminal [stock](../../../../../stock.md) price even though different paths to that price have different intermediate histories.

For $w_0>0$, a nonnegative terminal wealth $X$ with initial cost $w_0$ satisfies

$$
\mathbb E_P[ZX]=\mathbb E_QX=R^nw_0.
$$

The [utility function](../../../../../utility-function-split.md) has derivative $v'(x)=x^{-(\gamma-1)/\gamma}$. Put $\eta=\gamma/(\gamma-1)>1$. Its first-order condition makes $v'(X)$ proportional to $Z$, so $X=CZ^{-\eta}$. Choosing $C$ to satisfy the pricing [budget constraint](../../../../../budget-constraint.md) gives the [binomial power-utility terminal wealth](../../../../../binomial-power-utility-terminal-wealth.md)

$$
\boxed{X_*=\frac{R^nw_0}{\mathbb E_P[Z^{1-\eta}]}Z^{-\eta}.}
$$

All states have positive probability and the state space is finite, so this payoff is positive, integrable and attainable. The normalizing constant is explicit: independence gives

$$
\mathbb E_P[Z^{1-\eta}]=\left[p\left(\frac qp\right)^{1-\eta}+(1-p)\left(\frac{1-q}{1-p}\right)^{1-\eta}\right]^n.
$$

Combining these two formulas with the terminal-price expression for $Z$ gives $X_*$ entirely as a function of $S_n$.

To prove global optimality, [strict concavity](../../../../../strict-concavity.md) gives $v(X)-v(X_*)\le v'(X_*)(X-X_*)$. Because $v'(X_*)=C^{-1/\eta}Z$, the [expectation](../../../../../expected-value.md) of the right side is zero for any other payoff satisfying the same pricing [budget constraint](../../../../../budget-constraint.md). Equality requires $X=X_*$ almost surely. Backward replication supplies its [self-financing strategy](../../../../../self-financing-portfolio.md), so this static optimum is attainable by trading. If $w_0=0$ and terminal wealth must be nonnegative, the only feasible terminal wealth is zero. For $p=q$, the density is one and the optimizer is the riskless wealth $R^nw_0$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
