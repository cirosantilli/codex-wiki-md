<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For edge weights $w_{ij}$, form the out-Laplacian

$$
L_{ij}=\begin{cases}
\sum_{k\ne i}w_{ik},&i=j,\\
-w_{ij},&i\ne j.
\end{cases}
$$

The directed [matrix-tree theorem](../../../../../../kirchhoff-s-theorem.md) states that the cofactor $\det L^{(r)}$, obtained by deleting row and column $r$, equals the sum of $\prod_{e\in T}w_e$ over directed spanning trees oriented towards $r$.

Expand the determinant by permutations, and in each diagonal entry expand the sum of outgoing edge weights. A term chooses one outgoing edge at every vertex other than $r$. If the resulting functional digraph contains a directed cycle, sign-reversing inclusion-exclusion over its cycles cancels the term. The surviving choices are precisely the acyclic ones; every vertex then reaches $r$, so they are rooted directed spanning trees, each with positive sign and its product weight. This proves the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 145](../../../paper-145-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
