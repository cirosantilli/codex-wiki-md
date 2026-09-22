<h1 id="35b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $H$ be the one-dimensional [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) and let

$$
E_0\leq E_1\leq E_2\leq\cdots
$$

be its discrete [energy eigenvalues](../../../../../../energy-eigenvalue.md). Expanding a normalized trial wavefunction in an orthonormal energy basis,

$$
|\psi\rangle=\sum_nc_n|n\rangle,
$$

gives

$$
\langle\psi|H|\psi\rangle
=\sum_n|c_n|^2E_n
\geq E_0\sum_n|c_n|^2
=E_0.
$$

Thus the [Rayleigh-Ritz variational principle](../../../../../../rayleigh-ritz-variational-principle.md) gives

$$
\boxed{
E_0\leq
\frac{\int_{\mathbb R}\psi^*(x)H\psi(x)\,dx}
{\int_{\mathbb R}|\psi(x)|^2\,dx}}
$$

for every nonzero admissible trial wavefunction. One chooses a parameterized family and minimizes the quotient.

When $V(x)=V(-x)$, parity commutes with $H$. In one dimension the nondegenerate ground state is even and the first excited state is odd. Restricting the trial family to odd wavefunctions makes every trial state orthogonal to the ground state, so

$$
\boxed{
E_1\leq
\frac{\langle\psi_{\rm odd}|H|\psi_{\rm odd}\rangle}
{\langle\psi_{\rm odd}|\psi_{\rm odd}\rangle}}.
$$

This is the [odd-state variational principle for an even potential](../../../../../../odd-state-variational-principle-for-an-even-potential.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [35B](../../35b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
