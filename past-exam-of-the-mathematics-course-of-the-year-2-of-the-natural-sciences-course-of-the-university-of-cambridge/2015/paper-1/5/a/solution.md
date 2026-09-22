<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Av_j=a_jv_j$. Commutation gives $A(Bv_j)=B(Av_j)=a_jBv_j$, so $B$ preserves each [eigenspace](../../../../../eigenspace.md) of $A$. Since the [eigenvalues](../../../../../eigenvalue.md) of $A$ are nondegenerate, each [eigenspace](../../../../../eigenspace.md) is one-dimensional and $Bv_j=b_jv_j$. The [spectral theorem](../../../../../spectral-theorem.md) for a [Hermitian matrix](../../../../../hermitian-operator.md) lets us choose these [vectors](../../../../../vector.md) as an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md). With $U=(v_1,\ldots,v_n)$,

$$
\boxed{A=U\Lambda_AU^\dagger,\qquad B=U\Lambda_BU^\dagger,\qquad U^\dagger U=I.}
$$

This is [simple spectrum gives simultaneous diagonalization](../../../../../simple-spectrum-gives-simultaneous-diagonalization.md). The common [eigenvectors](../../../../../eigenvector.md) can be chosen up to their phases and ordering. In fact degeneracy does not prevent a common eigenbasis for commuting [Hermitian matrices](../../../../../hermitian-operator.md), but the one-dimensional argument already suffices here.

The convergent [matrix exponential](../../../../../matrix-exponential.md) series respects similarity, so $e^A=Ue^{\Lambda_A}U^\dagger$ and likewise for $B$. Scalar exponentials multiply on each diagonal entry, giving

$$
\boxed{e^Ae^B=Ue^{\Lambda_A}e^{\Lambda_B}U^\dagger=Ue^{\Lambda_A+\Lambda_B}U^\dagger=e^{A+B}.}
$$

The essential hypothesis is commutation; Hermiticity supplies this convenient diagonalization proof.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
