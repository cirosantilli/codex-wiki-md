<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

For a self-adjoint [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) bounded below, the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) says $E[\psi]=\langle\psi,H\psi\rangle/\langle\psi,\psi\rangle\ge E_0$. Expanding in energy [eigenstates](../../../../../eigenstate.md) proves this, since the quotient is a weighted average of energies. Optimize a tractable trial family to obtain an upper bound on the ground energy.

If $H\psi_0=E_0\psi_0$, a regular trial error $\psi=\psi_0+\epsilon\eta$ gives the exact cancellation

$$
E[\psi]-E_0=\frac{\epsilon^2\langle\eta,(H-E_0)\eta\rangle}{\|\psi_0+\epsilon\eta\|^2}=O(\epsilon^2).
$$

The linear terms vanish because $(H-E_0)\psi_0=0$. Here $\eta$ is a fixed finite-energy direction, or is uniformly bounded in the quadratic-form norm. A Hilbert-space norm bound alone is insufficient for an unbounded [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md): a norm-$\epsilon$ admixture of an [eigenstate](../../../../../eigenstate.md) with energy of order $\epsilon^{-2}$ can have order-one energy error. The usual quadratic-error claim therefore presupposes a controlled-energy perturbation.

For the first excited energy minimize the quotient on states orthogonal to the exact [ground state](../../../../../ground-state.md). Alternatively diagonalize $H$ in a trial subspace and use the min-max principle: its second Ritz [eigenvalue](../../../../../eigenvalue.md) is an upper bound for the second exact [eigenvalue](../../../../../eigenvalue.md). An arbitrary trial function without either [orthogonality](../../../../../orthogonal-vectors.md) or a min-max construction need not bound the first excited level.

The one-dimensional even potential has even [ground state](../../../../../ground-state.md) and odd [first excited state](../../../../../first-excited-state.md), by the Sturm oscillation ordering. Choose the automatically orthogonal odd trial function $\psi_a(x)=Nx e^{-ax^2/2}$, $a>0$. [Integration by parts](../../../../../integration-by-parts.md) gives the kinetic numerator $\int|\psi_a'|^2$, and the given Gaussian moments give

$$
E_1\le E(a)=\frac{3a}{2}+\frac3{2a}+\frac{15}{4a^2}.
$$

For example, the kinetic factor is $(I_0-2aI_2+a^2I_4)/I_2=3a/2$, while the potential factors are $I_4/I_2$ and $I_6/I_2$. Differentiation gives the unique positive minimizer $a^3-a-5=0$. Thus

$$
\boxed{a\approx1.90416,\qquad E_1\le E(a)\approx4.67824.}
$$

This is an upper estimate, not an exact [eigenvalue](../../../../../eigenvalue.md). Improve it with odd [polynomial](../../../../../polynomial-split.md)-Gaussian trial functions such as $(x+bx^3)e^{-ax^2/2}$, or a larger odd Ritz basis, and optimize the width. The [parity](../../../../../parity.md) restriction keeps all such states orthogonal to the even [ground state](../../../../../ground-state.md).

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
