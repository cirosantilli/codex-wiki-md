<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $(a,b,c)$ for holdings of cash, the [stock](../../../../../../stock.md) and the [European put option](../../../../../../european-put-option.md), and let $\gamma=-V_0$ be initial [consumption](../../../../../../consumption.md). At the given price, $a=-10b-c-\gamma$, and the three terminal payoffs, in descending order of the [stock](../../../../../../stock.md) price, are

$$
5b-c-\gamma,\qquad2b-c-\gamma,\qquad c-b-\gamma.
$$

Nonnegative terminal payoffs require $c+\gamma\leq2b$ and $c-\gamma\geq b$. Together with $\gamma\geq0$, these imply $b\geq2\gamma\geq0$. If $b=0$ they force $\gamma=c=a=0$, which is not an [arbitrage](../../../../../../arbitrage.md). If $b>0$, the highest-state payoff is at least $3b>0$, so every such choice is an [arbitrage](../../../../../../arbitrage.md). Consequently the complete set is

$$
\boxed{(a,b,c)=(-10b-c-\gamma,b,c),\quad b>0,\quad0\leq\gamma\leq b/2,\quad b+\gamma\leq c\leq2b-\gamma.}
$$

The [pure-investment arbitrages](../../../../../../pure-investment-arbitrage.md) are exactly the choices $\gamma=0$:

$$
\boxed{(a,b,c)=(-10b-c,b,c),\quad b>0,\quad b\leq c\leq2b.}
$$

For example, $(a,b,c)=(-11,1,1)$ costs zero and pays $(4,1,0)$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
