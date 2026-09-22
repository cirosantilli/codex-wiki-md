<h1 id="r/r2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Encode a [labelled tree](../../../../../labelled-tree.md) by repeatedly deleting its smallest-labelled [leaf of a graph](../../../../../leaf-of-a-graph.md) and recording its neighbor, stopping when two [vertices](../../../../../vertex-graph-theory.md) remain. This produces a sequence of length $n-2$ with entries in $\{1,\ldots,n\}$.

Conversely, given such a sequence, at each step choose the smallest unused label not occurring in the remaining sequence, join it to the first sequence entry, delete that chosen label and the first entry, and continue. Finally join the two labels left over. A label outside the remaining sequence always exists because two more labels than entries remain. The process never uses a previously deleted label as a sequence entry. Each step attaches a new [leaf of a graph](../../../../../leaf-of-a-graph.md) to the eventual remaining graph, so backward [induction](../../../../../mathematical-induction.md) shows that the result is [connected](../../../../../connected-space.md) and acyclic, hence a [tree](../../../../../tree-graph-theory-split.md).

In a [tree](../../../../../tree-graph-theory-split.md) encoding, a [vertex](../../../../../vertex-graph-theory.md) occurs once for every incident [edge](../../../../../edge-of-a-graph.md) except the [edge](../../../../../edge-of-a-graph.md) by which it is eventually removed, or the final surviving [edge](../../../../../edge-of-a-graph.md). Thus its number of occurrences is its [degree](../../../../../degree-graph-theory.md) minus one. The labels absent from the current remaining sequence are exactly the current [leaves of a graph](../../../../../leaf-of-a-graph.md). Both procedures therefore choose the same smallest [leaf of a graph](../../../../../leaf-of-a-graph.md) and [edge](../../../../../edge-of-a-graph.md) at every stage. They are [inverse](../../../../../inverse-element.md) maps, proving the claimed [bijection](../../../../../bijection.md), including the empty sequence when $n=2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [R2](../../r2.md)
3. [R](../../../r.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
