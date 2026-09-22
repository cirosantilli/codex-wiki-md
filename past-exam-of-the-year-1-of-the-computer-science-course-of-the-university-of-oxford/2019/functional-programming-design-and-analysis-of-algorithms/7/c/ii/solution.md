<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the multiplicative score exactly as defined in the paper. Let $P_t(v)$ be the largest score of a matching length-$t$ route ending at $v$. Initialize $P_0(v_0)=1$ and mark all other entries unreachable. For each stage, clear the new layer and inspect matching [edges](../../../../../../edge-of-a-graph.md) from reachable entries:

$$
P_t(v)=\max_{\substack{(u,v)\in E,\ \sigma(u,v)=x_t\\u\text{ reachable at stage }t-1}} P_{t-1}(u)\,p(u,v).
$$

An empty candidate [set](../../../../../../set-split.md) is marked unreachable, rather than given score zero: a genuine route may have score zero. A Boolean reachability table or a sentinel $-1$ with a guard before multiplication distinguishes the cases. Store the maximizing predecessor [edge](../../../../../../edge-of-a-graph.md) at each reachable layer entry, retaining one on a tie.

Multiplication by a nonnegative [edge](../../../../../../edge-of-a-graph.md) factor preserves order, so replacing a prefix by a larger-scoring matching prefix cannot worsen its extension. [Induction](../../../../../../mathematical-induction.md) proves this [maximum-product edge-labelled walk](../../../../../../maximum-product-edge-labelled-walk.md) recurrence correct. Choose a reachable final entry of greatest score and follow its layer-indexed predecessors backwards to reconstruct the answer. If no final entry is reachable, report that no matching route exists, even though all numeric scores might otherwise look like zero.

The [running time](../../../../../../running-time.md) is $O(k(|V|+|E|))$, and rolling scores have [space complexity](../../../../../../space-complexity.md) $O(|V|)$, while retaining all reconstruction pointers gives [space complexity](../../../../../../space-complexity.md) $O(k|V|)$. For the vertex-simple interpretation, retain the visited [set](../../../../../../set-split.md) in each state as in part i, prohibit revisits and maximize the same products over those states. This exact exponential-state variant preserves both the zero-score distinction and predecessor reconstruction. If the starting [vertex](../../../../../../vertex-graph-theory.md) is unrestricted rather than inherited from part i, initialize $P_0(v)=1$ for every [vertex](../../../../../../vertex-graph-theory.md). The calculation needs no independence assumption beyond the paper's definition of a product score; repeated physical edge-activation events would require a separate probabilistic model.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
