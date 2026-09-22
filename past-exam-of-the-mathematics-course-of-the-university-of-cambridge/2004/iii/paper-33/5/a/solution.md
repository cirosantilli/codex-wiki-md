<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Drop the [subtour elimination constraints](../../../../../../subtour-elimination-constraints.md), retaining the one-incoming/one-outgoing equations and any branch decisions. This is an [assignment problem](../../../../../../assignment-problem.md), solvable in [polynomial time](../../../../../../polynomial-time.md). Its optimum is a [lower bound](../../../../../../lower-bound-in-a-partially-ordered-set.md) on the best schedule in that branch because every admissible schedule satisfies the relaxed constraints. Add the constant processing-time sum to compare completion-time bounds.

Keep a feasible schedule as an incumbent [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md). At each [branch and bound](../../../../../../branch-and-bound.md) node, solve the restricted [assignment problem](../../../../../../assignment-problem.md). If it is infeasible or its bound is at least the incumbent, discard the node. If its optimum is a single tour, it is a feasible schedule attaining the bound, so update the incumbent and close the node. If it has a proper subtour $C$ with arcs $e_1,\ldots,e_r$, every valid Hamiltonian tour must omit at least one of those arcs.

For a disjoint exhaustive branching rule, child $h$ forces $e_1,\ldots,e_{h-1}$ and forbids $e_h$, for $h=1,\ldots,r$. Every valid tour falls into the child indexed by the first omitted arc. Re-solve the corresponding assignment relaxations, prioritize small bounds, and repeat. Finitely many binary choices give an exact terminating search; its worst-case [tree](../../../../../../tree-graph-theory.md) can be exponential. **Assignment optima provide lower bounds, while complete tours provide upper bounds.** Patching subtours or local improvement can improve the incumbent without changing the exact pruning argument.

## ↑ Ancestors (11)

1. [A](../a.md)
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
