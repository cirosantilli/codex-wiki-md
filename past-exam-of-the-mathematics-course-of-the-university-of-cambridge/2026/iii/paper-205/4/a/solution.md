<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The graph has edges $1\to2\leftarrow3$, $1\to4$, $2\to4$, $3\to5$, $4\to5$, $4\to6$, and $6\to5$. Any [D-separating set](../../../../../../d-separating-set.md) for 1 and 6 must contain 4 because of the directed path $1\to4\to6$. Conditioning on 4 activates the collider $1\to4\leftarrow2$ and, through its descendant, the collider $1\to2\leftarrow3$. The remaining route through $3\to5\leftarrow6$ is open exactly when 5 is conditioned on and 3 is not. Hence all separating sets, among the nonendpoint vertices, are

$$
\{4\},\quad\{2,4\},\quad\{3,4\},\quad\{2,3,4\},
\quad\{3,4,5\},\quad\{2,3,4,5\}.
$$

For the second graph, $2\perp\!\!\!\perp5\mid1,6$ forces colliders on the unblocked two-edge paths: $2\to3\leftarrow5$ and $2\to4\leftarrow5$. Acyclicity then forces $1\to4$ and $6\to4$. Thus its edges are

$$
\boxed{1\to2,quad2\to3,quad5\to3,quad1\to4,quad2\to4,
\quad5\to4,quad6\to4,quad6\to5.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
