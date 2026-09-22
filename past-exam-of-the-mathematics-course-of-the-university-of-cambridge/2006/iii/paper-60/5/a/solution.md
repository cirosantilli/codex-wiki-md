<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work with real positive pulse envelopes and define $\Omega=\sqrt{\Omega_{12}^2+\Omega_{23}^2}>0$. Then $\cos\theta=\Omega_{12}/\Omega$ and $\sin\theta=\Omega_{23}/\Omega$. In the ordered basis $|1\rangle,|2\rangle,|3\rangle$, the candidate [dark state of a driven Hamiltonian](../../../../../../dark-state-of-a-driven-hamiltonian.md) has coordinates

$$
|D\rangle=\frac1\Omega\begin{pmatrix}-\Omega_{23}\\0\\\Omega_{12}\end{pmatrix}.
$$

Multiplication by the given [rotating-wave approximation](../../../../../../rotating-wave-approximation.md) matrix gives

$$
H^{\rm RWA}|D\rangle=\frac1\Omega\begin{pmatrix}0\\-\Omega_{12}\Omega_{23}+\Omega_{23}\Omega_{12}\\0\end{pmatrix}=0.
$$

Thus

$$
\boxed{|\Psi_0\rangle=\cos\theta|3\rangle-\sin\theta|1\rangle,\qquad\lambda_0=0.}
$$

Its absence of an excited-state component is the destructive interference that makes it dark. The orthogonal bright ground-state combination is $|B\rangle=\cos\theta|1\rangle+\sin\theta|3\rangle$. Since $H|B\rangle=\Omega|2\rangle$ and $H|2\rangle=\Omega|B\rangle$, the two remaining eigenstates are $(|B\rangle\pm|2\rangle)/\sqrt2$ with [eigenvalues](../../../../../../eigenvalue.md) $\pm\Omega$.

For signed envelopes, use a continuous two-argument angle with $\cos\theta=\Omega_{12}/\Omega$ and $\sin\theta=\Omega_{23}/\Omega$, rather than an ambiguous arctangent branch. When both fields vanish, every state has zero [eigenvalue](../../../../../../eigenvalue.md) and this formula does not select a unique dark vector.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
