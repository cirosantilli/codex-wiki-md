<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Multiplying the [Arnoldi decomposition](../../../../../arnoldi-decomposition.md) by $Q_k^T$ shows that the leading square block is

$$
H_k=Q_k^TAQ_k.
$$

It is an [upper Hessenberg matrix](../../../../../upper-hessenberg-matrix.md) by the [Arnoldi iteration](../../../../../arnoldi-iteration.md). Because $A=A^T$, it is also a [symmetric matrix](../../../../../symmetric-matrix.md). Entries below the first subdiagonal vanish by the Hessenberg structure, and their reflected entries above the first superdiagonal vanish by symmetry. Consequently

$$
\boxed{T_k=Q_k^TAQ_k\text{ is symmetric tridiagonal}},\qquad
\boxed{AQ_k=Q_{k+1}\widetilde T_k}.
$$

The extra last row has only its final entry possibly nonzero. With the usual choice of positive normalization factors, the individual column relations are the three-term [Lanczos algorithm](../../../../../lanczos-algorithm.md) recurrence

$$
Aq_j=\beta_{j-1}q_{j-1}+\alpha_jq_j+\beta_jq_{j+1},
\qquad \alpha_j=q_j^TAq_j,\quad \beta_j>0,
$$

where the first term is omitted for $j=1$. This reduction is an exact-arithmetic statement; [round-off error](../../../../../round-off-error.md) can affect the [orthogonality](../../../../../orthogonal-vectors.md) in an implementation.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
