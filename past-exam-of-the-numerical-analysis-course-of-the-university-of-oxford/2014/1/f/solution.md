<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let the real [QR shift](../../../../qr-shift.md) be $\mu$ and put $r=\sqrt{1+\mu^2}$. A valid [QR factorization](../../../../qr-decomposition.md), including the singular cases $\mu=\pm1$, is

$$
Q=\frac1r\begin{pmatrix}-\mu&-1\\1&-\mu\end{pmatrix},\qquad R=\begin{pmatrix}r&-2\mu/r\\0&(\mu^2-1)/r\end{pmatrix}.
$$

Here $Q^TQ=I$, and multiplying verifies $QR=A-\mu I$. Using this [orthogonality](../../../../orthogonal-vectors.md) in the shifted update gives

$$
A_1=Q^TAQ=\frac1{1+\mu^2}\begin{pmatrix}-2\mu&\mu^2-1\\\mu^2-1&2\mu\end{pmatrix}.
$$

It is diagonal exactly when $\mu^2-1=0$. Therefore **all real shifts giving the eigenvalues in one iteration are**

$$
\boxed{\mu=+1\quad\text{or}\quad\mu=-1.}
$$

The resulting diagonal is $(-1,1)$ or $(1,-1)$, respectively. Both [QR shifts](../../../../qr-shift.md) are exact [eigenvalues](../../../../eigenvalue.md). Sign changes in the [QR factorization](../../../../qr-decomposition.md) conjugate $A_1$ by a diagonal sign [matrix](../../../../matrix.md) and do not alter its zero pattern. This is [Exact-shift diagonalization of a two-state swap matrix](../../../../exact-shift-diagonalization-of-a-two-state-swap-matrix.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
