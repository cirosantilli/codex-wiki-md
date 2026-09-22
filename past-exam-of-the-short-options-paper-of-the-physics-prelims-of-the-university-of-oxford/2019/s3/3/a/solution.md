<h1 id="s3/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Inside the [infinite square well](../../../../../infinite-square-well.md), $V=0$, and the [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2}=E\psi,\qquad\psi(0)=\psi(L)=0.
$$

For $E>0$, write $k^2=2mE/\hbar^2$ and $\psi=A\sin kx+B\cos kx$. The first [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) gives $B=0$, and the second requires $kL=n\pi$ for a nonzero state. The case $n=0$ is identically zero; negative $n$ only changes an overall [quantum phase](../../../../../quantum-phase.md). For $E=0$ a linear solution satisfying both walls is zero, and for $E<0$ the hyperbolic solutions likewise cannot satisfy both walls nontrivially.

[Wavefunction normalization](../../../../../wavefunction-normalization.md), $\int_0^L|\psi|^2dx=1$, fixes $|A|=\sqrt{2/L}$. The orthonormal [energy eigenstates](../../../../../energy-eigenstate.md) and [energy eigenvalues](../../../../../energy-eigenvalue-split.md) are therefore

$$
\boxed{\psi_n(x)=\sqrt{\frac2L}\sin\frac{n\pi x}L,\qquad E_n=\frac{n^2\pi^2\hbar^2}{2mL^2},\qquad n=1,2,\ldots.}
$$

Each state vanishes outside the well. Its stationary time-dependent form is $\Psi_n(x,t)=\psi_n(x)e^{-iE_nt/\hbar}$. General states are normalized [superpositions](../../../../../superposition-principle.md) of these modes, rather than additional single [energy eigenstates](../../../../../energy-eigenstate.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [S3](../../../s3.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
