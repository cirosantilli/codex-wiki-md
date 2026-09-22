<h1 id="b/8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If default liquidates the firm as soon as its value crosses below $F$, equity is extinguished at that event. If default never occurs before maturity, equity receives $(V_T-F)_+$. It is therefore a no-rebate [down-and-out option](../../../../../down-and-out-claim.md) on firm value, with [strike price](../../../../../strike-price.md) and barrier both equal to $F$.

For a firm that has survived to $t$ and has $V_t>F$, part (b) gives

$$
\boxed{E_t=C^E(t,V_t;F)
-\left(\frac{V_t}{F}\right)^{1-2r/\sigma^2}
C^E(t,F^2/V_t;F).}
$$

If default has already occurred, $E_t=0$. At maturity a surviving firm has equity $(V_T-F)_+$.

The source uses a strict crossing $V<F$. With nonzero [volatility](../../../../../financial-volatility.md), continuity and immediate two-sided Brownian fluctuations at a first barrier hit make the pre-maturity absorbing value at $V=F$ zero as well: starting at the barrier, the process crosses below it immediately almost surely. At maturity the [contingent claim payoff](../../../../../contingent-claim-payoff.md) at equality is also zero. Thus this convention has the same pricing boundary as the usual barrier-hit convention in this nondegenerate model.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
