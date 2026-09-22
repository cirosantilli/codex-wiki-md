<h1 id="3/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**Always true.** Replace every [all-different constraint](../../../../../../all-different-constraint.md) by the pairwise inequalities on its scope. Then solutions are precisely the [proper graph colourings](../../../../../../graph-coloring-split.md) of the [primal graph](../../../../../../primal-graph.md) using values from $D$ as colours. Put $t=\operatorname{tw}(P)$.

A [graph](../../../../../../graph-split.md) of [treewidth](../../../../../../treewidth.md) $t$ has a [proper graph colouring](../../../../../../graph-coloring-split.md) with at most $t+1$ colours. Here is a constructive proof. In a width-$t$ [tree decomposition](../../../../../../tree-decomposition.md), remove any leaf bag contained in its neighbor. If more than one bag remains, a leaf bag has a [vertex](../../../../../../vertex-graph-theory.md) absent from its neighbor. The running-intersection property means that [vertex](../../../../../../vertex-graph-theory.md) occurs only in the leaf bag, so every neighbor of the [vertex](../../../../../../vertex-graph-theory.md) belongs to that bag. It has at most $t$ neighbors. If only one bag remains, it has at most $t+1$ [vertices](../../../../../../vertex-graph-theory.md) and the same degree bound holds.

Remove the chosen [vertex](../../../../../../vertex-graph-theory.md) and repeat; deleting [vertices](../../../../../../vertex-graph-theory.md) cannot increase the width of the restricted [tree decomposition](../../../../../../tree-decomposition.md). Now colour in reverse removal order. At most $t$ already coloured neighbors forbid colours, so one of $t+1$ colours is always available. Since the [integer](../../../../../../integer-split.md) inequality $|D|>t$ gives $|D|\ge t+1$, this produces a satisfying assignment:

$$
\boxed{|D|>\operatorname{tw}(P)\ \Longrightarrow\ \operatorname{Sol}(P)\ne\varnothing.}
$$

The common unrestricted [constraint domain](../../../../../../constraint-domain.md) and the exclusively [all-different constraints](../../../../../../all-different-constraint.md) are essential: arbitrary constraint relations do not reduce to [graph colouring](../../../../../../graph-coloring-split.md) in this way.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Intelligent systems](../../../../intelligent-systems-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
