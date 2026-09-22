<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V$ be a finite-dimensional real or complex [inner product space](../../../../../../inner-product-space.md), and let $A\subseteq\operatorname{End}(V)$ be a unital [subalgebra](../../../../../../subalgebra.md) stable under the [adjoint operator](../../../../../../adjoint-operator.md). Define its [commutant of an operator algebra](../../../../../../commutant-of-an-operator-algebra.md) by $A'=\{T:Ta=aT\text{ for all }a\in A\}$. The [double commutant theorem for star-algebras](../../../../../../double-commutant-theorem-for-star-algebras.md) asserts $\boxed{A''=A}$. The inclusion $A\subseteq A''$ follows immediately from the definition; we prove the reverse.

Write $N=\dim V$, fix a [basis](../../../../../../basis.md) $v_1,\ldots,v_N$, and act diagonally on $V^N$. The [linear subspace](../../../../../../vector-subspace.md)

$$
W=\{(av_1,\ldots,av_N):a\in A\}
$$

is invariant under every diagonal $a$. Since $A$ is closed under adjoints, its [orthogonal complement](../../../../../../orthogonal-complement.md) $W^\perp$ is invariant too: $\langle aw,z\rangle=\langle w,a^*z\rangle=0$ for $w\in W^\perp$, $z\in W$. Hence the [orthogonal projection](../../../../../../orthogonal-projection.md) $P$ onto $W$ commutes with every diagonal $a$.

Writing $P$ as an $N$ by $N$ block [matrix](../../../../../../matrix.md) $(P_{ij})$, this says $P_{ij}a=aP_{ij}$, so each $P_{ij}\in A'$. If $b\in A''$, it commutes with every $P_{ij}$, and its diagonal action therefore commutes with $P$ and preserves $W$. Because $1\in A$, $(v_1,\ldots,v_N)\in W$. Therefore there is one $a\in A$ such that

$$
(bv_1,\ldots,bv_N)=(av_1,\ldots,av_N).
$$

Equality on the [basis](../../../../../../basis.md) gives $b=a$, proving the theorem over either scalar field.

The identity hypothesis is necessary. For a possibly nonunital adjoint-stable [subalgebra](../../../../../../subalgebra.md), adjoining the ambient identity does not change its [commutant of an operator algebra](../../../../../../commutant-of-an-operator-algebra.md), so the exact statement is $A''=A+\mathbb F I$. For example $A=\{0\}$ has $A''=\mathbb F I$ on a nonzero $V$. Thus the usual exam formulation takes the algebra to contain the identity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
