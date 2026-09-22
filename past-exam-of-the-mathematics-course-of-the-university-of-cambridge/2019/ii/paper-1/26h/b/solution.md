<h1 id="26h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\operatorname{Sym}_n$ be the vector space of real symmetric matrices and consider

$$
\Phi:M_n(\mathbb R)\longrightarrow\operatorname{Sym}_n,
\qquad
\Phi(A)=A^TA.
$$

At $R\in O(n)$,

$$
D_R\Phi(H)=R^TH+H^TR.
$$

This derivative is surjective: for $S\in\operatorname{Sym}_n$, choosing $H=RS/2$ gives $D_R\Phi(H)=S$. Thus $I$ is a regular value and the [orthogonal group](../../../../../../orthogonal-group.md) $O(n)=\Phi^{-1}(I)$ is a submanifold of codimension

$$
\dim\operatorname{Sym}_n=\frac{n(n+1)}2.
$$

The determinant takes only the values $\pm1$ on $O(n)$, so the [special orthogonal group](../../../../../../special-orthogonal-group.md) $SO(n)=\{R\in O(n):\det R=1\}$ is an open-and-closed submanifold of $O(n)$. Therefore

$$
\dim SO(n)=n^2-\frac{n(n+1)}2=\frac{n(n-1)}2.
$$

The tangent space is the kernel of $D_R\Phi$:

$$
\boxed{T_RSO(n)
=\{H:R^TH+H^TR=0\}
=\{RA:A\in\mathfrak{so}(n)\}},
$$

where the [Special orthogonal Lie algebra](../../../../../../special-orthogonal-lie-algebra.md) $\mathfrak{so}(n)$ is the vector space of [skew-symmetric matrices](../../../../../../skew-symmetric-matrix.md). This proves the [special orthogonal group as a submanifold](../../../../../../special-orthogonal-group-as-a-submanifold.md) description.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26H](../../26h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
