<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Each [endomorphism](../../../../../endomorphism.md) has three distinct [eigenvalues](../../../../../eigenvalue.md) in a three-dimensional [complex vector space](../../../../../complex-vector-space.md). Choose a nonzero [eigenvector](../../../../../eigenvector.md) for each [eigenvalue](../../../../../eigenvalue.md); these vectors are [linearly independent](../../../../../linear-independence.md) and hence form an [eigenbasis](../../../../../eigenbasis.md). Both operators are therefore [diagonalizable](../../../../../diagonalizable-matrix.md) with diagonal matrix $D=\operatorname{diag}(1,2,3)$.

Their [characteristic polynomials](../../../../../characteristic-polynomial.md) are

$$
\boxed{\chi_S(t)=\chi_T(t)=(t-1)(t-2)(t-3).}
$$

If a [polynomial](../../../../../polynomial-split.md) $p$ annihilates either operator, applying it to each [eigenvector](../../../../../eigenvector.md) gives $p(1)=p(2)=p(3)=0$. Thus its [minimal polynomial](../../../../../minimal-polynomial.md) must contain all three factors. Conversely, their product annihilates the diagonal matrix, so

$$
\boxed{m_S(t)=m_T(t)=(t-1)(t-2)(t-3).}
$$

Finally, send an ordered [eigenbasis](../../../../../eigenbasis.md) of $S$ to the correspondingly ordered [eigenbasis](../../../../../eigenbasis.md) of $T$. The resulting invertible map $C$ satisfies $CS=TC$, and hence **$T=CSC^{-1}$: the two endomorphisms are conjugate**.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
