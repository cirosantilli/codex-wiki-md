# Orthogonal null-space completion of a square matrix

↑ **Parent:** [Matrix rank](matrix-rank.md)

Let $A$ be a real $n\times n$ [matrix](matrix.md) of [matrix rank](matrix-rank.md) $n-m$, and let the columns of $L,R$ be [bases](basis.md) of $\ker A^\top$ and $\ker A$, respectively. Then $B=LR^\top$ has [matrix rank](matrix-rank.md) $m$, $A^\top B=AB^\top=0$, and $M=A+B$ is an [invertible matrix](invertible-matrix.md).

**Proof.** Since $R$ has independent columns, its [Gram matrix](gram-matrix.md) $R^\top R$ is invertible, and $R^\top$ maps onto $\mathbb R^m$. Thus $\operatorname{im}B=\operatorname{im}L=\ker A^\top$ and $\operatorname{rank}B=m$. The basis conditions give the two zero products. In particular,

$$
MM^\top=AA^\top+BB^\top,
\qquad AA^\top BB^\top=0.
$$

If $MM^\top x=0$, taking its [dot product](dot-product.md) with $x$ gives $\|A^\top x\|^2+\|B^\top x\|^2=0$. Hence $x\in\ker A^\top=\operatorname{im}B$ and simultaneously $x\in\ker B^\top=(\operatorname{im}B)^\perp$. Therefore $x=0$, and $M$ is invertible. The case $m=0$ is immediate.

For a common [eigenvector](eigenvector.md) of $AA^\top$ and $BB^\top$, the two [eigenvalues](eigenvalue.md) have zero product and positive sum: exactly one is zero. Thus the added term fills the missing orthogonal output directions without interfering with the original ones.

## ↑ Ancestors (9)

1. [Matrix rank](matrix-rank.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/4/g/solution.md)
