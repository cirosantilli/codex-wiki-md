<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the source's unrestricted “cycle” means a [closed walk](../../../../../closed-walk.md), permitting repeated [vertices](../../../../../vertex-graph-theory.md); part (d) explicitly separates this from a [simple cycle](../../../../../cycle-in-a-graph.md).[p. 7, Questions 8(c)–(d)](../../../../../functional-programming-design-and-analysis-of-algorithms-examination-paper-by-the-university-of-oxford-2013.md)

Suppose a [closed walk](../../../../../closed-walk.md) contains both colours. Any two [vertices](../../../../../vertex-graph-theory.md) on it reach one another by following suitable portions of the [closed walk](../../../../../closed-walk.md). All its [vertices](../../../../../vertex-graph-theory.md), and therefore all its [edges](../../../../../edge-of-a-graph.md), lie inside one [strongly connected component](../../../../../strongly-connected-component.md). That [strongly connected component](../../../../../strongly-connected-component.md) contains internal [edges](../../../../../edge-of-a-graph.md) of both colours.

Conversely, suppose one [strongly connected component](../../../../../strongly-connected-component.md) contains a black [edge](../../../../../edge-of-a-graph.md) $u\to v$ and a white [edge](../../../../../edge-of-a-graph.md) $x\to y$. Its strong connectivity supplies a [graph path](../../../../../path-in-a-graph.md) from $v$ to $x$ and another from $y$ to $u$, both inside the component. Concatenate

$$
u\xrightarrow{\mathrm{black}}v\leadsto x\xrightarrow{\mathrm{white}}y\leadsto u.
$$

This is a [closed walk](../../../../../closed-walk.md) containing both chosen [edges](../../../../../edge-of-a-graph.md). Either connecting [graph path](../../../../../path-in-a-graph.md) may have length zero. Thus the [mixed-colour closed walk criterion](../../../../../mixed-colour-closed-walk-criterion.md) is

$$
\boxed{\text{a mixed-colour closed walk exists}\iff\text{some SCC has internal edges of both colours}.}
$$

The [edges](../../../../../edge-of-a-graph.md) must be internal: differently coloured [edges](../../../../../edge-of-a-graph.md) merely leaving a [strongly connected component](../../../../../strongly-connected-component.md) do not establish the claim.

## ↑ Ancestors (12)

1. [C](../c.md)
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
