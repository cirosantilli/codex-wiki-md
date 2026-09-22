<h1 id="17f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The eigenvalues of a graph are the eigenvalues of its adjacency matrix. Order the vertices with those of $X$ first and those of $Y$ second. The adjacency matrix then has block form

$$
A=\begin{pmatrix}0&B\\B^T&0\end{pmatrix},
$$

where $B$ is the $|X|\times|Y|$ [bipartite adjacency matrix](../../../../../../bipartite-adjacency-matrix.md).

Since zero is not an eigenvalue, $A$ is invertible. If $|X|\ne|Y|$, then

$$
\operatorname{rank}A\leq2\min(|X|,|Y|)<|X|+|Y|,
$$

a contradiction. Thus $|X|=|Y|=r$. Moreover, if $B$ were singular, a nonzero $v$ with $Bv=0$ would give $A(0,v)^T=0$. Hence $B$ is invertible.

In the determinant expansion

$$
\det B=\sum_{\pi\in S_r}\operatorname{sgn}(\pi)
\prod_{i=1}^r B_{i,\pi(i)},
$$

at least one product is nonzero. For its permutation $\pi$, all entries $B_{i,\pi(i)}$ equal one, so the corresponding $r$ edges pair every vertex of $X$ with a distinct vertex of $Y$. They form the required matching.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17F](../../17f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
