<h1 id="20d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Time-dependent Schrödinger equation](../../../../../../time-dependent-schrodinger-equation.md) is $i\hbar\partial_t\Psi=H\Psi$. The normalized eigenstates of the Hermitian [Hamiltonian](../../../../../../hamiltonian.md) $H_3$ with distinct [eigenvalues](../../../../../../eigenvalue.md) are orthogonal, so they form an orthonormal [basis](../../../../../../basis.md) of this two-state system. Substitute the expansion of $\Psi$ and compare the two coefficients:

$$
\boxed{i\hbar\dot a_0=-a_0,\qquad i\hbar\dot a_1=a_1}.
$$

Hence $a_0(t)=a_0(0)e^{it/\hbar}$ and $a_1(t)=a_1(0)e^{-it/\hbar}$. For the normalized test state $\phi=\alpha\chi_0+\beta\chi_1$, the [Born rule](../../../../../../born-rule.md) gives

$$
\boxed{P_\phi(t)=|\langle\phi,\Psi(t)\rangle|^2
=|\bar\alpha a_0(t)+\bar\beta a_1(t)|^2}.
$$

The complex conjugates are essential; relative phases can affect this probability even though the [energy](../../../../../../energy.md)-state populations remain constant under $H_3$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20D](../../20d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
