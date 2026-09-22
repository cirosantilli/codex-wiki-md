<h1 id="p/p4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Starting with $A_0=A$, choose real shifts $\sigma_j$, factor $A_j-\sigma_jI=Q_jR_j$, and set

$$
A_{j+1}=R_jQ_j+\sigma_jI=Q_j^TA_jQ_j.
$$

Each step is an [orthogonal](../../../../../orthogonal-vectors.md) similarity, so the eigenvalues are preserved and all iterates are similar. If $A_j^T=A_j$, transposing $Q_j^TA_jQ_j$ proves symmetry of $A_{j+1}$, completing the induction.

The given matrix is the [Householder reflection](../../../../../householder-transformation.md)

$$
A=I-\frac2n\mathbf1\mathbf1^T.
$$

It has [eigenvalue](../../../../../eigenvalue.md) $-1$ along $\mathbf1$ and $+1$ on its [orthogonal](../../../../../orthogonal-vectors.md) complement, hence $A^TA=I$. In the positive-diagonal QR convention its unshifted factorization is $Q=A$, $R=I$, so the next iterate is again $A$. Thus **unshifted QR is stationary**, despite the matrix generally having nonzero off-diagonal entries. If arbitrary diagonal signs are allowed in $R$, a step can instead replace $A$ by $DAD$ for a diagonal sign matrix $D$; every off-diagonal magnitude remains unchanged. Such sign changes still make no progress towards diagonalization.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
