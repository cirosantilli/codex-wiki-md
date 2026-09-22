<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Cutset conditioning](../../../../../cutset-conditioning.md) selects a [cycle cutset](../../../../../cycle-cutset.md) $C$: deleting its [vertices](../../../../../vertex-graph-theory.md) makes the binary [constraint graph](../../../../../constraint-graph.md) a [forest](../../../../../forest.md). Enumerate assignments to $C$, reject those violating internal constraints, and filter each remaining [constraint domain](../../../../../constraint-domain.md) against the chosen cutset values. Solve the residual components by [tree-structured constraint satisfaction](../../../../../tree-structured-constraint-satisfaction.md). Stop at a successful assignment, or report failure after all cutset assignments fail. Completeness follows by considering the restriction of any full solution to $C$; soundness follows by checking internal, crossing and residual constraints. With maximum [constraint domain](../../../../../constraint-domain.md) size $q$ and $k$ cutset [variables](../../../../../variable-mathematics.md), a typical bound is $O(q^k(n-k)q^2)$ for the residual [forest](../../../../../forest.md) work, with cutset and crossing checks added explicitly.[§2.4.1, tree passes and cutset conditioning](../../../../../cs-188-constraint-ordering-and-structure-notes.md)

Here take **$C=\{c,e\}$**. The residual [constraint graph](../../../../../constraint-graph.md) has [vertices](../../../../../vertex-graph-theory.md) $a,b,d$ and only [edges](../../../../../edge-of-a-graph.md) $ab,ad$, a [tree](../../../../../tree-graph-theory-split.md) rooted at $a$. Choose the consistent cutset values $c=3,e=1$. Filtering against these assignments gives

$$
D_a=\{1,2\},\quad D_b=\{2\},\quad D_d=\{2,4\}.
$$

The upward support pass from $b$ deletes $a=2$, because $b$ can only equal $2$. The pass from $d$ retains $a=1$, which has support $2$ or $4$. Assign $a=1$ at the root and then supported child values $b=2,d=2$. Together with $c=3,e=1$, this gives the solution in (c).

No singleton [cycle cutset](../../../../../cycle-cutset.md) exists: deleting $a,b,d$ or $e$ leaves, respectively, a triangle on $bce,acd,abc$ or $abc$; deleting $c$ leaves the [cycle in a graph](../../../../../cycle-in-a-graph.md) $a-b-e-d-a$. Thus the two-element choice is also minimum, although the [algorithm](../../../../../algorithm-split.md) only requires a valid cutset.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
