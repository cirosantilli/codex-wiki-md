<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A precise safe-extension form of the [cut lemma for minimum spanning trees](../../../../../cut-lemma-for-minimum-spanning-trees.md) is as follows. Let $F\subseteq E$ be contained in some [minimum spanning tree](../../../../../minimum-spanning-tree.md). Let $S$ be a nonempty proper subset of $V$, and suppose no [edge](../../../../../edge-of-a-graph.md) of $F$ crosses the [cut of a graph](../../../../../cut-graph-theory.md) $(S,V\setminus S)$. If $e$ is any least-weight crossing [edge](../../../../../edge-of-a-graph.md), then

$$
\boxed{F\cup\{e\}\text{ is contained in some minimum spanning tree}.}
$$

To prove it, choose a [minimum spanning tree](../../../../../minimum-spanning-tree.md) $T$ containing $F$. If $e\in T$, it already certifies the claim. Otherwise inserting $e$ creates a [graph cycle](../../../../../cycle-in-a-graph.md). The other part of that [graph cycle](../../../../../cycle-in-a-graph.md) must cross the [cut of a graph](../../../../../cut-graph-theory.md), so choose a crossing [edge](../../../../../edge-of-a-graph.md) $f\in T$. It does not belong to $F$, and $w(e)\le w(f)$. Then $T-f+e$ is a [spanning tree](../../../../../spanning-tree.md) containing $F\cup\{e\}$, of weight no greater than the optimum. It is therefore also optimal.

With $F=\varnothing$, a lightest crossing [edge](../../../../../edge-of-a-graph.md) belongs to at least one [minimum spanning tree](../../../../../minimum-spanning-tree.md). If that [edge](../../../../../edge-of-a-graph.md) is uniquely lightest, it belongs to every [minimum spanning tree](../../../../../minimum-spanning-tree.md), the strict version of the [minimum spanning tree cut property](../../../../../minimum-spanning-tree-cut-property.md). With ties, “every” would be false: in an equal-weight triangle either crossing edge can be omitted from some optimum.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
