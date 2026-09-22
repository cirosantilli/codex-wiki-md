<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First take $x\ne y$. Sample a [uniform spanning tree](../../../../../../uniform-spanning-tree.md) using [Wilson's algorithm](../../../../../../wilson-s-algorithm.md) rooted at $y$, with $x$ processed first. The first walk runs from $x$ until its first hit of $y$, so its [loop erasure](../../../../../../loop-erasure.md) is exactly the unique $x$-to-$y$ [graph path](../../../../../../path-in-a-graph.md) of the resulting [tree](../../../../../../tree-graph-theory.md). Later attachments cannot alter that [graph path](../../../../../../path-in-a-graph.md). This is the [uniform-spanning-tree path representation of loop-erased random walk](../../../../../../uniform-spanning-tree-path-representation-of-loop-erased-random-walk.md).

Instead root [Wilson's algorithm](../../../../../../wilson-s-algorithm.md) at $x$ and process $y$ first. The resulting [tree](../../../../../../tree-graph-theory.md) still has the same uniform law, while its first attachment has the law of [loop-erased random walk](../../../../../../loop-erased-random-walk.md) from $y$ to $x$. A [tree](../../../../../../tree-graph-theory.md)'s [graph path](../../../../../../path-in-a-graph.md) between two fixed [graph vertices](../../../../../../vertex-graph-theory.md) has the same unoriented [edge](../../../../../../edge-of-a-graph.md) set in both directions. Pushing the common [tree](../../../../../../tree-graph-theory.md) law through this [graph path](../../../../../../path-in-a-graph.md) map therefore gives

$$
\boxed{\mathcal E(\operatorname{LERW}_{x\to y})\overset d=\mathcal E(\operatorname{LERW}_{y\to x}).}
$$

Here $\mathcal E$ means the set of unoriented [edges](../../../../../../edge-of-a-graph.md). In fact, reversing the complete [graph vertex](../../../../../../vertex-graph-theory.md) [sequence](../../../../../../sequence.md) from the first loop-erased walk has the law of the second, giving [reversibility of loop-erased random walk](../../../../../../reversibility-of-loop-erased-random-walk.md). If $x=y$ and first hitting allows time zero, both [graph paths](../../../../../../path-in-a-graph.md) are empty and the equality is immediate.

This is a distributional assertion, not a pathwise identity between chronological [loop erasure](../../../../../../loop-erasure.md) and reversal. For example, the valid walk trajectory $x,a,b,a,c,b,y$ in a [graph](../../../../../../graph-split.md) containing the triangle on $a,b,c$ and the [edges](../../../../../../edge-of-a-graph.md) $x a,b y$ erases forward to $x,a,c,b,y$. Erasing the reversed trajectory and then reversing the result gives $x,a,b,y$, a different [graph path](../../../../../../path-in-a-graph.md). Wilson's root-independent [tree](../../../../../../tree-graph-theory.md) law is what proves the stated equality of [probability distributions](../../../../../../probability-distribution.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
