<h1 id="17f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Euler formula for a connected planar graph](../../../../../../euler-formula-for-a-connected-planar-graph.md) follows by induction on the number of cycle edges. If $G$ is a tree, then $e=n-1$ and $f=1$, so $n-e+f=2$. Otherwise remove an edge belonging to a cycle. The graph remains connected, while the two faces adjoining that edge merge: both $e$ and $f$ decrease by one. Thus $n-e+f$ is unchanged, and induction reaches a tree.

Every edge borders two face sides, so the sum of the face sizes is $2e$. If every face has size at least $g$, then

$$
gf\leq2e.
$$

Substitute $f=2-n+e$ from Euler's formula:

$$
g(2-n+e)\leq2e,
$$

and hence the [planar girth edge bound](../../../../../../planar-girth-edge-bound.md)

$$
\boxed{e\leq\frac{g(n-2)}{g-2}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17F](../../17f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
