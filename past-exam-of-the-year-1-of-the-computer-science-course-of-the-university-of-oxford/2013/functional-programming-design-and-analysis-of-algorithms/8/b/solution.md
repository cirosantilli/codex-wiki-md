<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Allow a zero-length [graph path](../../../../../path-in-a-graph.md), as in Question 5. Then every [vertex](../../../../../vertex-graph-theory.md) $a$ reaches itself, proving [reflexivity](../../../../../reflexive-relation.md). If $a\equiv b$, its definition already includes both directions of [reachability](../../../../../reachability-in-a-graph.md), so interchanging $a,b$ proves [symmetry](../../../../../symmetry-physics.md).

If $a\equiv b$ and $b\equiv c$, concatenate the [graph paths](../../../../../path-in-a-graph.md) $a\to b$ and $b\to c$ to obtain [reachability](../../../../../reachability-in-a-graph.md) from $a$ to $c$. Similarly concatenate $c\to b$ and $b\to a$ for the reverse direction. Repeated [vertices](../../../../../vertex-graph-theory.md) can be removed if [graph paths](../../../../../path-in-a-graph.md) are required to be simple. Thus $a\equiv c$, proving [transitivity](../../../../../transitive-relation.md). Consequently

$$
\boxed{\equiv\text{ is an equivalence relation, whose classes are the strongly connected components.}}
$$

The zero-length convention matters for an isolated [vertex](../../../../../vertex-graph-theory.md): it is still a singleton [strongly connected component](../../../../../strongly-connected-component.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
