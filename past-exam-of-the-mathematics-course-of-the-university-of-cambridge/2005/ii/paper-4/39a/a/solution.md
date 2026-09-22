<h1 id="39a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At step $k=1,\ldots,n-2$, isolate the active column tail $a=A_{k+1:n,k}$. If its subtail is already zero, no reflection is needed. Otherwise choose a [Householder reflection](../../../../../../householder-transformation.md) $H=I-2vv^T/(v^Tv)$ on the active coordinates such that $Ha$ has only its first component nonzero. A cancellation-resistant choice is $v=a+\operatorname{sgn}(a_1)\|a\|e_1$, with an arbitrary positive sign if $a_1=0$. Embed $H$ as $P=\operatorname{diag}(I_k,H)$ and replace $A$ by $P^TAP$. Previous reduced columns are untouched, and column $k$ now has no entries below the first subdiagonal.

Similarity by an [orthogonal matrix](../../../../../../orthogonal-matrix.md) preserves skew symmetry. Consequently an upper-Hessenberg result also has zeros above the first superdiagonal, so it is tridiagonal with zero diagonal and opposite-sign corresponding off-diagonal entries.

For the active skew-symmetric block $D$, compute $w=2Dv/(v^Tv)$. Because $v^TDv=0$, expanding the two-sided reflection simplifies to

$$
\boxed{HDH=D+vw^T-wv^T}.
$$

Store and update just one triangle, obtain the other by negation, and keep the diagonal exactly zero. Matrix-vector multiplication can likewise use each stored entry once to contribute to two output coordinates. This is [skew-symmetric Householder tridiagonalization](../../../../../../skew-symmetric-householder-tridiagonalization.md); there is no need for two dense matrix-matrix multiplications.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39A](../../39a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
