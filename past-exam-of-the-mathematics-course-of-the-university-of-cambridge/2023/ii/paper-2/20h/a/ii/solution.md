<h1 id="20h/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\omega_1,\ldots,\omega_n$ be an [integral basis](../../../../../../../integral-basis.md) of $\mathcal O_K$. Since each $\alpha_j$ is an [algebraic integer](../../../../../../../algebraic-integer.md), there is an integer matrix $A=(a_{ij})$ such that

$$
\alpha_j=\sum_i a_{ij}\omega_i.
$$

The $\alpha_j$ form a $\mathbb Q$-basis, so $\det A\ne0$.

Products of algebraic integers are algebraic integers, and their traces are rational algebraic integers, hence ordinary integers. Therefore every entry

$$
\operatorname{Tr}_{K/\mathbb Q}(\alpha_i\alpha_j)
$$

is integral. Part (i) makes the trace Gram matrix nonsingular, so $\Delta(\alpha_1,\ldots,\alpha_n)$ is a nonzero integer.

Let $G_\omega$ and $G_\alpha$ be the two trace Gram matrices. A change of basis gives

$$
G_\alpha=A^TG_\omega A.
$$

Taking determinants yields the [discriminant-index formula for an integral lattice](../../../../../../../discriminant-index-formula-for-an-integral-lattice.md)

$$
\Delta(\alpha_1,\ldots,\alpha_n)
=(\det A)^2d_K,
$$

where $d_K=\det G_\omega$ is the [field discriminant](../../../../../../../field-discriminant.md). Since $\det A$ is a nonzero integer,

$$
|\Delta(\alpha_1,\ldots,\alpha_n)|\geq|d_K|>0.
$$

Equality holds exactly when $|\det A|=1$, which is equivalent to $A$ being unimodular and to $\alpha_1,\ldots,\alpha_n$ being a $\mathbb Z$-basis of $\mathcal O_K$. Thus the minimum is the positive integer

$$
\boxed{|d_K|}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [20H](../../../20h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
