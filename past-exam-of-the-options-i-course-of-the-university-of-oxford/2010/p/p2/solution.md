<h1 id="p/p2/solution">Solution</h1>

↑ **Parent:** [P2](../p2.md)

A [QR decomposition](../../../../qr-decomposition.md) is a factorization $A=QR$ with $Q^TQ=I$ and $R$ upper triangular. An orthogonal transformation preserves the Euclidean [norm](../../../../norm.md) because

$$
\boxed{\|Qx\|^2=x^TQ^TQx=x^Tx=\|x\|^2.}
$$

For the basic [QR algorithm](../../../../qr-algorithm.md), start with $A_0=A$ and repeatedly form

$$
A_k=Q_kR_k,\qquad A_{k+1}=R_kQ_k.
$$

In a convergent diagonal form, the diagonal entries give the eigenvalues; practical symmetric-[matrix](../../../../matrix.md) implementations use shifts and deflation to obtain and isolate such convergence. The basic unshifted iteration alone need not converge diagonally for every symmetric input.

At every step, however,

$$
\boxed{A_{k+1}=R_kQ_k=Q_k^TA_kQ_k.}
$$

Thus each iterate is orthogonally similar to its predecessor. Similar matrices have the same [characteristic polynomial](../../../../characteristic-polynomial.md) and eigenvalues, including multiplicities, so induction proves that every iterate has exactly the original eigenvalues. [Orthogonal similarity](../../../../orthogonal-similarity.md) also preserves symmetry.

## ↑ Ancestors (12)

1. [P2](../p2.md)
2. [P](../../p.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
