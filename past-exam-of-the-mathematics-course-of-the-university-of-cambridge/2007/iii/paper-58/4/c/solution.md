<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the [phase gate](../../../../../../phase-gate.md)

$$
\boxed{U_1=S=\begin{pmatrix}1&0\\0&i\end{pmatrix}.}
$$

It is unitary. Acting on both qubits leaves $|00\rangle$ unchanged and multiplies $|11\rangle$ by $i^2=-1$, so $S\otimes S$ sends $\Psi_+$ to $\Psi_-$ with exactly the requested phase.

Using the [Hadamard gate](../../../../../../hadamard-gate.md) $H$, choose

$$
\boxed{U_2=HSH=\frac12\begin{pmatrix}1+i&1-i\\1-i&1+i\end{pmatrix}.}
$$

It is unitary and symmetric, and

$$
U_2^2=HS^2H=HZH=X.
$$

For any matrix $U$, applying $U\otimes U$ to $(|00\rangle+|11\rangle)/\sqrt2$ gives the coefficient matrix $UU^T/\sqrt2$. Here $U_2U_2^T=U_2^2=X$, hence

$$
(U_2\otimes U_2)|\Psi_+\rangle
=\frac{|01\rangle+|10\rangle}{\sqrt2}=|\Phi_+\rangle.
$$

Both displayed transformations are exact, not merely equal up to global phase. These common local unitaries permute the triplet Bell projectors while preserving the singlet projector by the preceding determinant identity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
