<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\Gamma=(-1)^F$ be [fermion parity](../../../../../../fermion-parity.md). It acts as $+1$ on [bosons](../../../../../../boson.md) and $-1$ on [fermions](../../../../../../fermion.md), and anticommutes with every odd [supercharge](../../../../../../supersymmetry-generator.md). In a finite physical [supermultiplet](../../../../../../supermultiplet.md) at fixed positive energy $E$, trace cyclicity gives

$$
\operatorname{Tr}\bigl[\Gamma\{Q_\alpha,Q_\alpha^\dagger\}\bigr]=0.
$$

Indeed, cycling $Q_\alpha$ in the second term and using $Q_\alpha\Gamma=-\Gamma Q_\alpha$ cancels the first term. Summing diagonal spinor components of the [Super-Poincaré algebra](../../../../../../super-poincare-algebra.md) gives $\sum_\alpha\{Q_\alpha,Q_\alpha^\dagger\}=4H$, since the Pauli matrices are traceless. Hence [supertrace pairing at positive energy](../../../../../../supertrace-pairing-at-positive-energy.md) yields

$$
4E\operatorname{Tr}\Gamma=4E(n_B-n_F)=0,\qquad\boxed{n_B=n_F\quad(E>0).}
$$

This is [boson-fermion degeneracy in a supermultiplet](../../../../../../boson-fermion-degeneracy-in-a-supermultiplet.md). Equivalently, a nonzero charge combination with positive anticommutator gives an invertible parity-changing map between the two sectors. The positive-energy qualification is important: a zero-energy supersymmetric vacuum may be a one-state bosonic representation and need not have a fermionic vacuum partner.

For any normalizable state $|v\rangle$, the same algebra gives [energy positivity in global supersymmetry](../../../../../../energy-positivity-in-global-supersymmetry.md):

$$
\langle v|H|v\rangle=\frac14\sum_{\alpha=1}^2\left(\|Q_\alpha|v\rangle\|^2+\|Q_\alpha^\dagger|v\rangle\|^2\right)\ge0.
$$

It vanishes exactly when every supercharge and its adjoint annihilates the state. In particular, for an existing translation-invariant vacuum, this proves

$$
\boxed{E_{\rm vac}=0\iff Q_\alpha|0\rangle=\bar Q_{\dot\alpha}|0\rangle=0\ \text{for all components};\qquad\text{spontaneously broken global SUSY}\iff E_{\rm vac}>0.}
$$

In infinite volume, interpret the statement as one about vacuum energy density, using finite-volume normalization first. The energy zero is fixed by the supersymmetry algebra; adding an arbitrary constant to the Hamiltonian while leaving that algebra unchanged is not allowed. For a canonical matter and gauge action, the same positivity is seen from $V=\sum_i|F_i|^2+\tfrac12\sum_aD_a^2$, so a nonzero auxiliary-field expectation breaks the symmetry. This global Minkowski statement does not apply unchanged to the [supergravity F-term potential](../../../../../../supergravity-f-term-potential.md), which can have negative-energy supersymmetric vacua.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
