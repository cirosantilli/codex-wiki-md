<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

An [arbitrage](../../../../../arbitrage.md) is a portfolio with nonpositive initial cost, nonnegative terminal payoff [almost surely](../../../../../almost-sure-convergence.md), and a strict benefit either from a negative initial cost or a positive payoff with positive [probability](../../../../../probability.md). An [equivalent martingale measure](../../../../../risk-neutral-measure.md) is a [probability](../../../../../probability.md) law equivalent to the physical law under which discounted traded prices are martingales. The bond has constant price one, so no discount factor is needed here.

Order the four states as $UU,UD,DU,DD$. Equivalence requires positive [probability](../../../../../probability.md) in every state, since the physical product law has full support. Each stock has risk-neutral up [probability](../../../../../probability.md) $1/2$, obtained by solving $1=(1+\epsilon)p+(1-\epsilon)(1-p)$. Thus all equivalent [martingale](../../../../../martingale-split.md) laws are

$$
\boxed{(q_{UU},q_{UD},q_{DU},q_{DD})=(a,1/2-a,1/2-a,a),\quad0<a<1/2.}
$$

The two risky returns need not be independent under a pricing measure.

A replicating portfolio pays $b+\theta S_2+\varphi S_3$, so its four payoffs satisfy

$$
\boxed{Y_{UU}+Y_{DD}=Y_{UD}+Y_{DU}.}
$$

Conversely this condition suffices: take $\theta=(Y_{UU}-Y_{DU})/(2\epsilon)$, $\varphi=(Y_{UU}-Y_{UD})/(2\epsilon)$, and choose the bond holding to match $Y_{DD}$. The relation then matches the fourth state as well. Its unique price is $(Y_{UU}+Y_{DD})/2=(Y_{UD}+Y_{DU})/2$.

For the same-direction claim, the payoff vector is $(1,0,0,1)$ and its price under $q$ is $2a$. Thus the possible strictly [arbitrage](../../../../../arbitrage.md)-free prices fill $(0,1)$ and **the lower [arbitrage](../../../../../arbitrage.md) bound is the infimum zero**. It is not achieved by an equivalent measure, and pricing the nonnegative nonzero claim at zero would itself permit [arbitrage](../../../../../arbitrage.md) by buying it. Its payoff is not replicable, since the displayed payoff relation fails. A buyer may pay a positive amount for its insurance against joint downward moves, for a view about dependence, or according to risk preferences. Under the stated physical independent law its expected payoff is $13/25$, illustrating that a zero lower bound does not make the payoff economically worthless.

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
