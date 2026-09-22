<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A one-period [self-financing strategy](../../../../../self-financing-portfolio.md) is a deterministic holdings vector $h=(h^0,\ldots,h^d)$, with initial cost $h\cdot S_0$ and terminal wealth $h\cdot S_1$. In the zero-initial-cost convention, an [arbitrage](../../../../../arbitrage.md) satisfies

$$
h\cdot S_0=0,\qquad h\cdot S_1\ge0\text{ a.s.},\qquad\mathbb P(h\cdot S_1>0)>0.
$$

The convention allowing a nonpositive initial cost is equivalent here: invest any initial proceeds in the strictly positive [numéraire](../../../../../numeraire.md) to obtain a zero-cost [portfolio](../../../../../investment-portfolio.md) with nonnegative terminal wealth.

Suppose a strictly positive [state-price density](../../../../../state-price-density.md) $\rho$ satisfies the asset-pricing equations, with the indicated products integrable. By linearity,

$$
\mathbb E[\rho(h\cdot S_1)]=h\cdot S_0.
$$

For an [arbitrage](../../../../../arbitrage.md), the right-hand side is zero while the left-hand side is strictly positive, since the integrand is nonnegative and is positive with positive probability. This contradiction proves **absence of [arbitrage](../../../../../arbitrage.md)**.

An [attainable European contingent claim](../../../../../attainable-european-contingent-claim.md) $X$ is a terminal random payoff for which some holdings vector $h$ satisfies $h\cdot S_1=X$ almost surely; its replication cost is $h\cdot S_0$. To prove uniqueness in a [complete market](../../../../../complete-market.md), suppose $\rho'$ is another positive [state-price density](../../../../../state-price-density.md). For every event $A$, attainability gives a [portfolio](../../../../../investment-portfolio.md) replicating $S_1^{(0)}\mathbf1_A$. Its initial cost has both representations, so

$$
\mathbb E[(\rho-\rho')S_1^{(0)}\mathbf1_A]=0\qquad\text{for every }A.
$$

The signed random variable here is integrable, because $\mathbb E[\rho S_1^{(0)}]=\mathbb E[\rho'S_1^{(0)}]=S_0^{(0)}<\infty$. Take $A$ to be the event where it is positive and then where it is negative. Both its positive and negative parts have expectation zero, and hence vanish almost surely. Since $S_1^{(0)}>0$,

$$
\boxed{\rho=\rho'\quad\text{a.s.}}
$$

This proves that [complete markets have unique state-price densities](../../../../../complete-markets-have-unique-state-price-densities.md) without requiring an extra lower bound on the random terminal [numéraire](../../../../../numeraire.md).

For the finite-state example, order the states from top to bottom in the diagram and write the density values as $\rho_1,\rho_2,\rho_3$. The two pricing equations are

$$
3\rho_1+5\rho_2+6\rho_3=12,\qquad6\rho_1+4\rho_2+3\rho_3=15.
$$

Adding gives $\rho_1+\rho_2+\rho_3=3$. Put $t=\rho_3$; substitution then gives

$$
\boxed{(\rho_1,\rho_2,\rho_3)=\left(\frac{3+t}{2},\frac{3(1-t)}2,t\right),\qquad0<t<1.}
$$

These are all the strictly positive solutions, and each satisfies both equations. The parameter is a state-price-density value, not a probability.

For a concrete unattainable [contingent claim](../../../../../contingent-claim.md), take the payoff vector $(0,1,0)$. A replicating [portfolio](../../../../../investment-portfolio.md) $(a,b)$ would have to satisfy $3a+6b=0$ and $6a+3b=0$ in the first and third states. These imply $a=b=0$, contradicting the required payoff one in the middle state. Thus **the market is an [incomplete market](../../../../../incomplete-market.md)**, despite having strictly positive [state-price densities](../../../../../state-price-density.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
