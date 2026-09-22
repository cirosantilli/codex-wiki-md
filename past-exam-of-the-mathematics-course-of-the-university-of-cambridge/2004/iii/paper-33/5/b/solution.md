<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent a schedule by a [permutation](../../../../../../permutation.md) $v_1,\ldots,v_{40}$, with $v_0=v_{41}=0$. Choose $1\leq p<q\leq40$ and reverse the block $v_p,\ldots,v_q$. This is a [2-opt](../../../../../../2-opt.md) move on the dummy tour. Its exact setup-cost change is the [asymmetric 2-opt reversal cost](../../../../../../asymmetric-2-opt-reversal-cost.md)

$$
\Delta=c_{v_{p-1},v_q}+c_{v_p,v_{q+1}}
-c_{v_{p-1},v_p}-c_{v_q,v_{q+1}}
+\sum_{r=p}^{q-1}
(c_{v_{r+1},v_r}-c_{v_r,v_{r+1}}).
$$

The internal sum matters because the specified changeovers need not be symmetric. When the block begins at the first job, the boundary terms correctly update the initial setup; the dummy return costs are zero. Processing times cancel.

At temperature $T>0$, [simulated annealing](../../../../../../simulated-annealing.md) accepts a move with [probability](../../../../../../probability.md)

$$
\boxed{\min\{1,\exp(-\Delta/T)\}.}
$$

With uniformly sampled reversal pairs the proposal is symmetric, so this is the appropriate [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md). Improvements and ties are always accepted; occasional uphill moves escape local minima. Repeatedly sample moves, gradually lower $T$, and retain the best schedule seen even if the current schedule worsens. Reversing a block of length two swaps adjacent jobs, so these moves connect the whole [permutation](../../../../../../permutation.md) space. A cooling schedule, iteration budget and restarts control practical performance. This is a heuristic at a finite budget; it does not certify global optimality unless paired with an exact bound or an appropriate limiting convergence argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
