<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Root the graph at $x_0$ and let $P^{(0)}$ be the transition matrix of simple random walk killed on hitting $x_0$, indexed by the remaining vertices. Its Green matrix is $G=(I-P^{(0)})^{-1}$. Successively eliminating vertices in an order $x_1,\ldots,x_n$ takes [Schur complements](../../../../../../schur-complement.md); the corresponding diagonal pivot at step $j$ is exactly $g_{D\setminus\{x_0,\ldots,x_{j-1}\}}(x_j)$. The product of the pivots is therefore

$$
\det G=\frac1{\det(I-P^{(0)})},
$$

which is invariant under the elimination order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
