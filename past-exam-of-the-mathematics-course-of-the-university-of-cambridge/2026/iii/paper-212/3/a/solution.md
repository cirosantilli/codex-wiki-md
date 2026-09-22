<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take an increasing exhaustion $G_n$ of $G$ by finite connected vertex sets, identify every vertex outside $G_n$ to one boundary vertex, and choose a [uniform spanning tree](../../../../../../uniform-spanning-tree.md) of the resulting finite wired graph. The weak limit as $n\to\infty$ is the [wired uniform spanning forest](../../../../../../wired-uniform-spanning-forest.md) of $G$.

For [Wilson algorithm rooted at infinity](../../../../../../wilson-algorithm-rooted-at-infinity.md), enumerate $V$ as $v_1,v_2,\ldots$. Run a [simple random walk](../../../../../../simple-random-walk.md) from $v_1$ forever and add its chronological [loop erasure](../../../../../../loop-erasure.md). Transience makes the infinite loop erasure well-defined. Next, from the first vertex not already in the forest, run an independent random walk until it hits the existing forest; if it never hits, run it forever. Add its loop erasure and continue through the enumeration. Wilson's theorem rooted at infinity says that the resulting forest has the wired uniform spanning forest law.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 212](../../../paper-212-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
