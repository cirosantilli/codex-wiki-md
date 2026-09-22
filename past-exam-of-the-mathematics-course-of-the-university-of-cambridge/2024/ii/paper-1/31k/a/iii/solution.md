<h1 id="31k/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take any $p+1$ points $z_1,ldots,z_{p+1}\in\mathbb R^p$. For each coordinate $j$, choose a point attaining the largest $j$th coordinate. At most $p$ points are chosen, so some point $z_k$ is not among them.

Consider the labeling that assigns $1$ to every chosen coordinate maximizer and $0$ to $z_k$. Any lower orthant

$$
\prod_{j=1}^p(-\infty,a_j]
$$

containing all the chosen points must have $a_j\geq\max_i(z_i)_j$ for every $j$, and hence contains $z_k$ as well. This labeling is impossible. No $p+1$ points are shattered, so

$$
\boxed{VC(H)\leq p.}
$$

This is the [VC dimension bound for lower orthants](../../../../../../../vc-dimension-bound-for-lower-orthants.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [31K](../../../31k.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
