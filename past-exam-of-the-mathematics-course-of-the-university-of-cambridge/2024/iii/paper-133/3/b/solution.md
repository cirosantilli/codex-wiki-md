<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S$ be a finite generating set of $H$, choose one lift $\widetilde s\in G$ for every $s\in S$, and put $K=\ker f$. The finite set

$$
\widetilde S\cup K
$$

generates $G$: lift a word representing $f(g)$ and observe that the discrepancy from $g$ lies in $K$.

Use this generating set for $G$. The quotient map does not increase word length, while lifting a shortest word in $H$ leaves only a final element of $K$, whose word length is at most one. Hence

$$
d_H(f(g),f(g'))
\le d_G(g,g')
\le d_H(f(g),f(g'))+1.
$$

The map is surjective, so it is a [finite-kernel quotient quasi-isometry](../../../../../../finite-kernel-quotient-quasi-isometry.md). Therefore $G$ is finitely generated and quasi-isometric to $H$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
