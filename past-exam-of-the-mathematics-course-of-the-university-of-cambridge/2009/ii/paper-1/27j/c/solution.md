<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $M$. Each time the chain is in $\{1,\ldots,M\}$ immediately before a jump, its conditional chance to jump to zero is at least the $\delta$ from part (b). Count all these opportunities, including returns to the same state after an excursion; the $T_m$ in part (b) need not count those returns. By the [Strong Markov property](../../../../../../strong-markov-property.md) at successive such visits, the probability of surviving $r$ opportunities without absorption is at most $(1-\delta)^r$. Hence infinitely many such opportunities without hitting zero have probability zero.

A positive state cannot be occupied forever: its finite positive holding rate gives an almost surely finite holding time. For a [nonexplosive continuous-time Markov chain](../../../../../../nonexplosive-continuous-time-markov-chain.md), visits at arbitrarily late times to the finite set therefore require infinitely many of the counted opportunities. On the event of no absorption, the chain consequently eventually stays above $M$, almost surely. Intersect this probability-one assertion over integers $M$. The result is $X_t\to\infty$. If zero is ever reached it remains occupied forever, and for initial state zero this is immediate. **Thus $\boxed{\mathbb P_i(E\cup F)=1}$ for every initial state.**

This uses the usual assumption implicit in an $I$-valued chain defined for all $t\geq0$: no explosion with loss to a cemetery state. The rate conditions alone do not ensure it. For example rates $q_{i,i+1}=i^3$, $q_{i0}=1$ allow an infinite upward path with probability $\prod_i i^3/(i^3+1)>0$ and a finite total holding time, since $\sum_i1/(i^3+1)<\infty$. The minimal chain then explodes; with a cemetery state the printed dichotomy would require an additional explosion alternative.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
