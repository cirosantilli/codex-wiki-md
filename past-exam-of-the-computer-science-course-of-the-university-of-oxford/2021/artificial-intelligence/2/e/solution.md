<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**This is a [graph colouring](../../../../../graph-coloring-split.md) [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md), with four available colours and one fixed colour.** Interpret slot labels as colours. Every conflict [edge](../../../../../edge-of-a-graph.md) requires distinct endpoint colours, exactly as in [proper graph colouring](../../../../../graph-coloring-split.md); [independent sets](../../../../../independent-set-graph-theory.md) of [vertices](../../../../../vertex-graph-theory.md) can share a slot. The unary restriction on $A$ fixes its colour to $1$.

The lecture's 3-colouring problem is the same construction with domains $\{1,2,3\}$. For the present [graph](../../../../../graph-split.md) under the assumptions in (a), the [clique](../../../../../clique-graph-theory.md) $\{A,B,E,G\}$ prevents a 3-colouring, while (c) supplies a 4-colouring. The fixed colour on $A$ does not otherwise change existence, since an unconstrained colouring can have its colour names permuted to put $A$ in colour $1$.

This four-colour necessity is conditional on the explicit $EA$ overlap. Removing that one [edge](../../../../../edge-of-a-graph.md) permits, for example, the 3-colouring $(A,B,C,D,E,F,G)=(1,2,2,3,1,2,3)$; the four-slot schedule remains valid in either model. Thus attendee modelling, rather than the mere availability of four slots, determines the required number of colours.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
