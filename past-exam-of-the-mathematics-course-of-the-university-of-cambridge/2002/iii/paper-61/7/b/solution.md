<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [inner product](../../../../../../inner-product.md) linear in its first argument; for a real space no conjugation convention is needed. Insert $u^*=\sum_{j=1}^n a_j u_j$ into the orthogonality condition against each [basis](../../../../../../basis.md) vector $u_i$. The [normal equations](../../../../../../normal-equation.md) are

$$
\boxed{\sum_{j=1}^n(u_j,u_i)a_j=(x,u_i),\qquad1\le i\le n.}
$$

Equivalently $Ha=b$, where $H_{ij}=(u_j,u_i)$ and $b_i=(x,u_i)$. This orientation of the [Gram matrix](../../../../../../gram-matrix.md) matches the stated inner-product convention. It is Hermitian and positive definite: for a nonzero [coefficient](../../../../../../coefficient.md) vector $a$,

$$
a^*Ha=\left\|\sum_j a_j u_j\right\|^2>0
$$

by [linear independence](../../../../../../linear-independence.md) of the [basis](../../../../../../basis.md). Hence $H$ is invertible and $a=H^{-1}b$ gives existence and uniqueness of $u^*$. For an [orthonormal basis](../../../../../../orthonormal-basis.md) this simplifies to $a_i=(x,u_i)$; for a general [basis](../../../../../../basis.md) the Gram inverse correctly accounts for interactions between [basis](../../../../../../basis.md) vectors.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../1.md)
3. [7](../../7.md)
4. [Paper 61](../../../paper-61-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
