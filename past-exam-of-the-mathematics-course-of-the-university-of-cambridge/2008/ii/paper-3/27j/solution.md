<h1 id="27j/solution">Solution</h1>

↑ **Parent:** [27J](../27j.md)

An [arbitrage](../../../../../arbitrage.md) is a self-financing strategy with zero initial value and terminal value nonnegative almost surely and strictly positive with positive probability. If an [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q$ exists, a self-financing portfolio in the stated constant-numeraire setting is a $Q$-martingale. Its terminal expectation therefore equals zero. Equivalence preserves the positive-probability event of positive profit, which would make that expectation strictly positive. This contradiction proves no arbitrage in this finite-time finite-state setting.

For the numerical tree use the bank account growing by $1+r=5/4$ and discount stock prices accordingly. The risk-neutral up probabilities solve $qS_u+(1-q)S_d=(5/4)S$, giving

$$
\boxed{q_0=\frac38,\qquad q_{30}=\frac16,\qquad q_{12}=\frac56.}
$$

Thus the four path probabilities are $1/16,5/16,25/48,5/48$, respectively.

The [American put option](../../../../../american-put-option.md) has terminal payoffs $0,0,0,5$. At the upper time-one node, both immediate exercise and continuation are zero. At the lower node, exercise gives three while discounted continuation gives $(4/5)(1/6)5=2/3$. Hence the option values at time one are $0,3$, and backward induction gives

$$
\boxed{V_0=\frac45\left(\frac38\,0+\frac58,3\right)=\frac32.}
$$

The lower node should indeed be exercised immediately, since $3>2/3$.

The seller's initial replicating hedge holds $-1/6$ share and four units in the bank account, costing $3/2$. At the bad node it is worth $-2+5=3$, enough for immediate exercise. If the buyer fails to exercise, the remaining European liability costs only $2/3$: hold $-5/6$ share and $32/3$ in the bank account, whose final payoffs are zero at stock price16 and five at stock price10. Switching to that hedge frees

$$
\boxed{3-\frac23=\frac73}
$$

as certain profit at time one, worth $35/12$ if banked until time two.

## ↑ Ancestors (10)

1. [27J](../27j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
