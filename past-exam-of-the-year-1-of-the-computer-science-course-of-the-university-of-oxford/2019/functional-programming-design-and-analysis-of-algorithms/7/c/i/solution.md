<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The printed formula for the [edge](../../../../../../edge-of-a-graph.md) label has mismatched variable names. The type-correct reading is $x_i=\sigma(v_{i-1},v_i)$. Interpret the requested route as a [directed walk](../../../../../../directed-walk.md) of consecutive labelled [edges](../../../../../../edge-of-a-graph.md), allowing repeated [vertices](../../../../../../vertex-graph-theory.md); the distinction from a vertex-simple [directed path](../../../../../../directed-path.md) is discussed below.

Let $R_t$ be the [set](../../../../../../set-split.md) of [vertices](../../../../../../vertex-graph-theory.md) reachable from the specified start after reading exactly the first $t$ labels. Initialize $R_0=\{v_0\}$ and update

$$
R_t=\{v:\text{there is }(u,v)\in E\text{ with }u\in R_{t-1}\text{ and }\sigma(u,v)=x_t\}.
$$

After $k$ stages, answer **yes exactly when $R_k\ne\varnothing$**. A [directed walk](../../../../../../directed-walk.md) realizing a prefix decomposes into a walk realizing the shorter prefix and one correctly labelled final [edge](../../../../../../edge-of-a-graph.md); conversely every such extension is valid. This proves the [dynamic programming](../../../../../../dynamic-programming.md) invariant by [induction](../../../../../../mathematical-induction.md) on $t$. Store reachable [vertices](../../../../../../vertex-graph-theory.md) in Boolean [arrays](../../../../../../array-data-structure.md) and scan the [edges](../../../../../../edge-of-a-graph.md) per stage. The [running time](../../../../../../running-time.md) is $O(k(|V|+|E|))$ with $O(|V|)$ rolling-table [space complexity](../../../../../../space-complexity.md), in addition to [graph](../../../../../../graph-split.md) storage. The empty label sequence is realized by staying at $v_0$.

If “path” is instead required to mean vertex-simple, augment the state to $(S,v)$, where $S$ is the [set](../../../../../../set-split.md) of visited [vertices](../../../../../../vertex-graph-theory.md). Start with $R_0(\{v_0\},v_0)$ and extend a matching [edge](../../../../../../edge-of-a-graph.md) to $w$ only when $w\notin S$, replacing $S$ by $S\cup\{w\}$. This gives an exact [dynamic programming](../../../../../../dynamic-programming.md) [algorithm](../../../../../../algorithm-split.md) for that interpretation too; reject immediately when $k\ge|V|$. A straightforward bound is $O(k2^{|V|}(|V|+|E|))$ [running time](../../../../../../running-time.md) with $O(2^{|V|}|V|)$ rolling-table storage. The exponential distinction is substantive: all labels equal and $k=|V|-1$ include the [Hamiltonian path](../../../../../../hamiltonian-path.md) problem from a fixed start. The efficient layered recurrence answers the consecutive-edge interpretation without pretending to enforce distinct [vertices](../../../../../../vertex-graph-theory.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
