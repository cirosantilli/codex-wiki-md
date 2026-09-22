# Local fermion density commutator with the Dirac Hamiltonian

↑ **Parent:** [Fermionic bilinear charge algebra](fermionic-bilinear-charge-algebra.md)

The equal-time [canonical anticommutation relations](canonical-anticommutation-relations.md) imply

$$
[n(\mathbf x),\psi_b^\dagger(\mathbf y)\psi_c(\mathbf z)]
=[\delta^{(3)}(\mathbf x-\mathbf y)-\delta^{(3)}(\mathbf x-\mathbf z)]\psi_b^\dagger(\mathbf y)\psi_c(\mathbf z),
\qquad n=\psi^\dagger\psi.
$$

Apply $-i\alpha^k_{bc}\partial_{z^k}+m\beta_{bc}$, set $\mathbf z=\mathbf y$, and integrate over $\mathbf y$. The [mass term](mass-term.md) cancels, leaving $i\int d^3y\,\psi^\dagger\alpha^k\psi\,\partial_{y^k}\delta^{(3)}(\mathbf x-\mathbf y)$. [Integration by parts](integration-by-parts.md) proves the title formula as a [distribution](distribution-mathematical-analysis.md) identity. The [Heisenberg equation of motion](heisenberg-equation-of-motion.md) then yields $\partial_t n=-\boldsymbol\nabla\cdot\mathbf j$ for the physical [Dirac current](dirac-current.md) $j^k=\bar\psi\gamma^k\psi$. The factor $-i$ is required because the [commutator](commutator.md) of [Hermitian operators](hermitian-operator.md) is anti-Hermitian.

## ↑ Ancestors (8)

1. [Fermionic bilinear charge algebra](fermionic-bilinear-charge-algebra.md)
2. [Canonical anticommutation relations](canonical-anticommutation-relations.md)
3. [Fermionic Fock space](fermionic-fock-space.md)
4. [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics-split.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
