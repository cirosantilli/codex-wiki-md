<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [two-pass strongly connected component algorithm](../../../../../two-pass-strongly-connected-component-algorithm.md). First run a complete [depth-first search](../../../../../depth-first-search.md) of $G$, starting a new search at each unvisited [vertex](../../../../../vertex-graph-theory.md) as necessary. Append each [vertex](../../../../../vertex-graph-theory.md) to a [list](../../../../../list-abstract-data-type.md) when its recursive call finishes. Next construct the [graph transpose](../../../../../graph-transpose.md) $G^T$ by reversing every [edge](../../../../../edge-of-a-graph.md). Reset all visited flags. Process the [vertices](../../../../../vertex-graph-theory.md) in decreasing first-pass finishing order, running [depth-first search](../../../../../depth-first-search.md) in $G^T$ from each still-unvisited [vertex](../../../../../vertex-graph-theory.md). The newly reached [vertices](../../../../../vertex-graph-theory.md) in each such search form one [strongly connected component](../../../../../strongly-connected-component.md).

To prove this, contract each [strongly connected component](../../../../../strongly-connected-component.md) to one [vertex](../../../../../vertex-graph-theory.md). The resulting [condensation graph](../../../../../condensation-graph.md) is a [Directed acyclic graph](../../../../../directed-acyclic-graph.md), because a directed [graph cycle](../../../../../cycle-in-a-graph.md) of distinct components would make them mutually reachable and hence a single component. For a component $C$, write $F(C)$ for its largest first-pass finishing time. If there is an [edge](../../../../../edge-of-a-graph.md) $C\to D$ between distinct components, then $F(C)>F(D)$. Indeed, if the first search reaches $C$ before $D$, it can reach $D$, which must finish before the search in $C$ finishes. If it reaches $D$ first, $D$ cannot reach $C$ or they would be the same component, so $D$ finishes before $C$ is discovered.

Among unreported components, the one with greatest $F$ therefore has no incoming [edge](../../../../../edge-of-a-graph.md) from another unreported component in $G$. In the [graph transpose](../../../../../graph-transpose.md) it has no outgoing [edge](../../../../../edge-of-a-graph.md) to any other unreported component. A second-pass search cannot escape it, while strong connectivity lets that search reach all its [vertices](../../../../../vertex-graph-theory.md). Earlier reported components are ignored by the visited flags. Repeating this argument proves

$$
\boxed{\text{each second-pass search returns exactly one SCC, and all SCCs are returned}.}
$$

Both [depth-first searches](../../../../../depth-first-search.md) visit every [vertex](../../../../../vertex-graph-theory.md) and scan every [edge](../../../../../edge-of-a-graph.md) once, and transposition costs $\Theta(|V|+|E|)$. Therefore the total [time complexity](../../../../../time-complexity.md) is $\boxed{\Theta(|V|+|E|)}$ with [adjacency lists](../../../../../adjacency-list.md). Storage for the transpose is $O(|V|+|E|)$, while visited flags, finishing order and the search stack use $O(|V|)$ additional space. No sorting is needed: reverse the [list](../../../../../list-abstract-data-type.md) recorded at finishing time.

## ↑ Ancestors (12)

1. [E](../e.md)
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
