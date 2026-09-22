<h1 id="6/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Only arrange switches towards `A`. For every [vertex](../../../../../../vertex-graph-theory.md) $u$, compute its degree $\deg(u)$ and the current number $c(u)$ of neighbours preferring `A`. Put the `B` [vertices](../../../../../../vertex-graph-theory.md) in a [max-heap](../../../../../../max-heap.md) with key $q(u)=2c(u)-\deg(u)$. Maintain each [vertex](../../../../../../vertex-graph-theory.md)'s current heap [array](../../../../../../array-data-structure.md) index during exchanges.

While the queue is nonempty and its [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) key is positive, extract that [vertex](../../../../../../vertex-graph-theory.md) $u$, show it its neighbours' preferences, append $u$ to the answer sequence, and set its preference to `A`. For every neighbour $v$ still preferring `B`, increase $c(v)$ by one and use `increaseKey` to increase its heap key by two. Stop when every remaining key is nonpositive.

A positive key means precisely a strict majority of `A` neighbours, so every listed move is legal. Degrees never change; `A` neighbours never revert in this chosen sequence. An isolated `B` [vertex](../../../../../../vertex-graph-theory.md) has key zero and cannot be converted. Initialization costs $O(|V|+|E|)$, there are at most $|V|$ extractions, and each [edge](../../../../../../edge-of-a-graph.md) causes at most two neighbour inspections and at most a constant number of key updates. The required bound is therefore **$O((|V|+|E|)\log(|V|+1))$**. A simple work queue of newly eligible [vertices](../../../../../../vertex-graph-theory.md) can even implement the same [monotone threshold activation](../../../../../../monotone-threshold-activation.md) in $O(|V|+|E|)$ time, since a [vertex](../../../../../../vertex-graph-theory.md) needs to be enqueued only once.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [6](../../../6.md)
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
