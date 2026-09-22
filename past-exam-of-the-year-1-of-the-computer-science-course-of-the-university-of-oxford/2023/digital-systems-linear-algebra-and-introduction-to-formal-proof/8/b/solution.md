<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The source's explicit parenthetical condition is domination: every unselected [vertex](../../../../../vertex-graph-theory.md) has a neighbour in the selected [set](../../../../../set-split.md). Together with independence this defines an [independent dominating set](../../../../../independent-dominating-set.md). A [first-order sentence](../../../../../first-order-sentence.md) expressing that definition with size at most three is

$$
\boxed{\exists x_1\exists x_2\exists x_3\left(
\bigwedge_{1\leq i<j\leq3}(x_i=x_j\lor\neg E(x_i,x_j))
\ \land\ 
\forall v\left(\bigvee_{i=1}^3v=x_i\ \lor\ \bigvee_{i=1}^3E(v,x_i)\right)
\right).}
$$

The finite conjunctions and disjunctions abbreviate three explicitly fixed terms, so this is a [first-order formula](../../../../../first-order-formula.md). Repeated witnesses allow one- or two-element choices; the first conjunction enforces independence only between distinct selected [vertices](../../../../../vertex-graph-theory.md). The last clause says that every [vertex](../../../../../vertex-graph-theory.md) is selected or adjacent to a selected [vertex](../../../../../vertex-graph-theory.md). With the usual nonempty-domain convention, any such choice has size at least one, so repeated witnesses cover all possibilities of size at most three.

For the standard meaning of [independent vertex cover](../../../../../independent-vertex-cover.md), replace the domination clause by

$$
\forall u\forall v\left(E(u,v)\to
\left(\bigvee_{i=1}^3u=x_i\ \lor\ \bigvee_{i=1}^3v=x_i\right)\right).
$$

This instead demands that every [edge](../../../../../edge-of-a-graph.md) has a selected endpoint. These interpretations differ: in a [triangle in a graph](../../../../../triangle-in-a-graph.md), any singleton is an [independent dominating set](../../../../../independent-dominating-set.md), but no [independent vertex cover](../../../../../independent-vertex-cover.md) exists. Giving both clauses avoids silently treating the source's two definitions as equivalent.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Introduction to formal proof](../../introduction-to-formal-proof.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
