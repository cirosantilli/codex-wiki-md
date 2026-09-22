<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

For a time-independent [Quantum Hamiltonian](../../../../../hamiltonian-quantum-mechanics.md), a [stationary state](../../../../../stationary-state.md) is an energy [eigenstate](../../../../../eigenstate.md). The [Schrödinger equation](../../../../../schrodinger-equation.md) separates its time dependence as

$$
\psi(x,t)=e^{-iEt/\hbar}\chi(x),\qquad \widehat H\chi=E\chi.
$$

Its probability density $|\psi(x,t)|^2=|\chi(x)|^2$ is time independent. Linearity of the [Schrödinger equation](../../../../../schrodinger-equation.md) gives

$$
\boxed{\psi(x,t)=\frac1{\sqrt2}\left(e^{-iE_1t/\hbar}\chi_1(x)+e^{-iE_2t/\hbar}\chi_2(x)\right).}
$$

Put $A_{jk}=\int_{-\infty}^{\infty}\chi_j^*\widehat A\chi_k\,dx$. The operator for a time-independent [observable](../../../../../observable.md) is a [Hermitian operator](../../../../../hermitian-operator.md), so $A_{21}=\overline{A_{12}}$. Substituting the evolved [wavefunction](../../../../../wave-function.md) into the [expectation value](../../../../../expectation-value.md) gives

$$
\langle\psi,\widehat A\psi\rangle=\frac12\left(A_{11}+A_{22}+e^{i(E_1-E_2)t/\hbar}A_{12}+e^{-i(E_1-E_2)t/\hbar}\overline{A_{12}}\right),
$$

and therefore, for a normalized state,

$$
\boxed{\langle A\rangle_\psi=\frac{A_{11}+A_{22}}2+\operatorname{Re}\!\left(e^{i(E_1-E_2)t/\hbar}A_{12}\right).}
$$

The normalization is automatic for orthogonal $\chi_1,\chi_2$, in particular when $E_1\neq E_2$: self-adjointness of $\widehat H$ gives $(E_1-E_2)\langle\chi_1,\chi_2\rangle=0$. If the energies coincide, normalization of the individual [eigenstates](../../../../../eigenstate.md) alone does not ensure normalization of their displayed sum; its squared [norm](../../../../../norm.md) is $1+\operatorname{Re}\langle\chi_1,\chi_2\rangle$. For a nonzero sum not having unit [norm](../../../../../norm.md), the physical [expectation value](../../../../../expectation-value.md) is the displayed numerator divided by this squared [norm](../../../../../norm.md). With orthonormal energy states, the stated formula holds in both the distinct and degenerate cases.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
