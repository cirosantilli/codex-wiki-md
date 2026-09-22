<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The northwest-corner rule constructs an initial basic feasible solution: fill the current cell with the smaller remaining supply and demand, delete the exhausted row or column, and continue.

For a current spanning-tree [basis](../../../../../../basis.md), solve $u_i+v_j=c_{ij}$ on its occupied cells, fixing one potential to zero. The [reduced cost](../../../../../../reduced-cost.md) of an unoccupied cell is

$$
\bar c_{ij}=c_{ij}-u_i-v_j.
$$

If all reduced costs are nonnegative, part (a) proves optimality. Otherwise choose a cell with negative reduced cost. Adding its edge to the tree creates a unique even cycle. Mark its cells alternately $+$ and $-$, starting with $+$ at the entering cell, and set

$$
\theta=\min\{x_{ij}: (i,j)\text{ is a }-\text{ cell}\}.
$$

Add $\theta$ on the plus cells and subtract it on the minus cells. Row and column totals are unchanged, the entering cell becomes positive, and a minimizing minus cell leaves the [basis](../../../../../../basis.md). In the nondegenerate case the objective decreases strictly. There are finitely many [bases](../../../../../../basis.md), so no [basis](../../../../../../basis.md) repeats and the algorithm terminates at a [basis](../../../../../../basis.md) with no negative reduced cost, which is optimal.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
