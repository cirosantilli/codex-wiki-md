<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By (i), two simple [graph paths](../../../../../path-in-a-graph.md) with different [edge](../../../../../edge-of-a-graph.md) sets have different lengths. In particular two distinct simple [graph paths](../../../../../path-in-a-graph.md) from the fixed root $v$ to the same [graph vertex](../../../../../vertex-graph-theory.md) $u$ have different [edge](../../../../../edge-of-a-graph.md) sets, so there is a **unique shortest [graph path](../../../../../path-in-a-graph.md) from $v$ to each $u$**. Positive weights ensure that a shortest walk has no repeated [graph vertex](../../../../../vertex-graph-theory.md): removing a [graph cycle](../../../../../cycle-in-a-graph.md) strictly reduces its length.

For each $u\ne v$, take the final [edge](../../../../../edge-of-a-graph.md) of its unique shortest [graph path](../../../../../path-in-a-graph.md). Every initial segment of a shortest [graph path](../../../../../path-in-a-graph.md) is itself shortest, since replacing it by a shorter one would shorten the whole route. Thus these [edges](../../../../../edge-of-a-graph.md) agree with the [graph paths](../../../../../path-in-a-graph.md)' unique predecessors. Following a predecessor strictly decreases $d_G(v,u)$, so no predecessor [graph cycle](../../../../../cycle-in-a-graph.md) is possible, and all [graph vertices](../../../../../vertex-graph-theory.md) eventually connect to $v$. They form a [shortest-path tree](../../../../../shortest-path-tree.md). Every other such [tree](../../../../../tree-graph-theory-split.md) would have to use the same unique root-to-vertex [graph paths](../../../../../path-in-a-graph.md), proving

$$
\boxed{\text{the shortest-path tree rooted at }v\text{ is unique}.}
$$

**Literal wording qualification.** “Any two paths” needs a convention. Reversing an undirected [graph path](../../../../../path-in-a-graph.md) preserves its [edge](../../../../../edge-of-a-graph.md) set and length; distinct zero-edge [graph paths](../../../../../path-in-a-graph.md) at different [graph vertices](../../../../../vertex-graph-theory.md) also have length zero. Thus the unrestricted statement is false if these count as different [graph paths](../../../../../path-in-a-graph.md). The proved edge-set assertion, and in particular uniqueness for [graph paths](../../../../../path-in-a-graph.md) with the same ordered endpoints, is exactly what is needed for the deduction. Arbitrary walks are not included.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
