<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The continuum Hamiltonian is that of a spinless one-dimensional p-wave [topological superconductor](../../../../../../topological-superconductor.md). Its topological phase has $\mu>0$, whereas the empty vacuum may be modeled as the trivial phase with $\mu<0$. With superconductor at $x<0$ and vacuum at $x>0$, this is

$$
\boxed{\operatorname{sgn}\mu(x)=-\operatorname{sgn}x.}
$$

Near the transition $\mu=0$, momenta are small and the quadratic term may be neglected. In Pauli-matrix notation, the long-wavelength [Bogoliubov--de Gennes Hamiltonian](../../../../../../bogoliubov-de-gennes-hamiltonian.md) is

$$
H_{\rm lw}=-\mu(x)\tau_z-i\hbar\Delta\tau_x\partial_x.
$$

The zero-energy equation becomes

$$
\partial_x\psi=\frac{\mu(x)}{\hbar\Delta}\tau_y\psi.
$$

Choose a constant spinor $\chi_+$ with $\tau_y\chi_+=\chi_+$. Then

$$
\boxed{
\psi(x)=\mathcal N
\exp\left(\int_0^x\frac{\mu(s)}{\hbar\Delta}\,ds\right)\chi_+}
$$

decays on both sides because $\mu$ changes from positive to negative. For asymptotically constant $|\mu|$, the [Continuum p-wave Majorana interface mode](../../../../../../continuum-p-wave-majorana-interface-mode.md) has width

$$
\boxed{\xi=\frac{\hbar\Delta}{|\mu|}.}
$$

Its characteristic momentum is $|p|\sim|\mu|/\Delta$. The neglected kinetic energy is small compared with $|\mu|$ when $|\mu|\ll m\Delta^2$ up to a factor of two, equivalently when $\xi\gg\hbar/(m\Delta)$.

In the Nambu basis, [Particle-hole symmetry of a Bogoliubov--de Gennes Hamiltonian](../../../../../../particle-hole-symmetry-of-a-bogoliubov-de-gennes-hamiltonian.md) lets a zero-energy eigenvector be chosen self-conjugate, $v(x)=u(x)^*$. The corresponding quasiparticle operator is

$$
\boxed{\gamma=\int dx\,[u(x)c(x)+u(x)^*c^\dagger(x)].}
$$

Taking the adjoint and interchanging the two terms gives $\gamma^\dagger=\gamma$. With the usual normalization it obeys $\{\gamma,\gamma\}=2$, so it is a [Majorana fermion operator](../../../../../../majorana-fermion-operator.md) localized at the interface.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
