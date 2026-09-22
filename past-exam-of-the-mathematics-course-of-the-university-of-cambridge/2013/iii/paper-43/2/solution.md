<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the usual normalization of the [Super-Poincaré algebra](../../../../../super-poincare-algebra.md), with $\sigma^\mu=(\mathbf1,\boldsymbol\sigma)$ and $\bar Q_{\dot\alpha}=Q_\alpha^\dagger$ under the corresponding index convention:

$$
\boxed{\{Q_\alpha,\bar Q_{\dot\beta}\}
=2\sigma^\mu_{\alpha\dot\beta}P_\mu.}
$$

The [supercharges](../../../../../supersymmetry-generator.md) are odd operators: they turn bosonic states into fermionic states and vice versa. If $\Pi=(-1)^F$ is [fermion parity](../../../../../fermion-parity.md), this statement is $\Pi Q_\alpha\Pi^{-1}=-Q_\alpha$, so

$$
\boxed{\{(-1)^F,Q_\alpha\}=0.}
$$

The same relation holds for the conjugate [supercharges](../../../../../supersymmetry-generator.md).

For a finite-dimensional physical [supermultiplet](../../../../../supermultiplet.md) at fixed four-momentum with energy $E>0$, let $n_B,n_F$ count physical bosonic and fermionic states. Cyclicity of the ordinary trace and the parity anticommutation imply

$$
\operatorname{Tr}\bigl(\Pi\{Q_\alpha,Q_\alpha^\dagger\}\bigr)=0:
\quad
\operatorname{Tr}(\Pi Q_\alpha^\dagger Q_\alpha)
=\operatorname{Tr}(Q_\alpha\Pi Q_\alpha^\dagger)
=-\operatorname{Tr}(\Pi Q_\alpha Q_\alpha^\dagger).
$$

Summing over the two spinor indices gives

$$
0=4E\operatorname{Tr}\Pi=4E(n_B-n_F),
\qquad\boxed{n_B=n_F.}
$$

This [supertrace pairing at positive energy](../../../../../supertrace-pairing-at-positive-energy.md) proves [boson-fermion degeneracy in a supermultiplet](../../../../../boson-fermion-degeneracy-in-a-supermultiplet.md) for massive as well as massless positive-energy representations. It counts on-shell polarizations, not merely the names of fields. The requirement $E>0$ matters: a zero-energy [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) can be a bosonic singlet without a paired fermionic vacuum.

If supersymmetry-breaking operators are explicitly added to the [Lagrangian](../../../../../lagrangian.md), the original [supercharges](../../../../../supersymmetry-generator.md) generally no longer commute with the full Hamiltonian. They are not conserved symmetries generating finite fixed-energy physical [supermultiplets](../../../../../supermultiplet.md); their original anticommutator does not equal the full translation generator with the breaking terms included. Thus the step replacing the parity-weighted anticommutator by $4E\Pi$ on a closed physical representation fails. The odd parity relation alone does not force energy degeneracy or an equal number of physical states at each mass.

This is [explicit versus spontaneous supersymmetry breaking](../../../../../explicit-versus-spontaneous-supersymmetry-breaking.md). In spontaneous breaking the action still has conserved [supercharges](../../../../../supersymmetry-generator.md), but the vacuum is not annihilated by them. Acting on particle excitations about that vacuum involves the broken-vacuum/Goldstino sector, so an ordinary finite particle multiplet above an invariant vacuum is no longer the correct pairing argument. The vacuum-energy statements below refer to an exact globally supersymmetric Hamiltonian, including the spontaneously broken case; they are not positivity claims for an arbitrary explicitly broken Hamiltonian.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
