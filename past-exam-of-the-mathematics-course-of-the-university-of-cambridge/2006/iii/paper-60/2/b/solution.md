<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stated relation places every generator, and therefore the whole [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md), inside the standard [compact symplectic Lie algebra](../../../../../../compact-symplectic-lie-algebra.md) $\mathfrak{sp}(\ell)\subset\mathfrak{su}(2\ell)$. Indeed the relation is closed under linear combinations and [commutators](../../../../../../commutator.md), and differentiating evolution gives

$$
\frac d{dt}(U^TJU)=0,\qquad U^TJU=J.
$$

Thus it supplies a [symplectic dynamical symmetry in quantum control](../../../../../../symplectic-dynamical-symmetry-in-quantum-control.md), rather than a claim that $J$ commutes with every [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md).

For $\ell\ge2$, **b1 is false**: even the full [compact symplectic group](../../../../../../compact-symplectic-group.md) does not act transitively on every mixed-state spectral orbit. Its algebra has dimension $\ell(2\ell+1)<(2\ell)^2-1$. An explicit obstruction is the [symplectic invariant of a density operator](../../../../../../symplectic-invariant-of-a-density-operator.md)

$$
I_J(\rho)=\operatorname{Tr}(\rho J\rho^T J^\dagger),
$$

which is unchanged by a symplectic conjugation. For $N=4$ and the printed $J$, let $a,b>0$, $a\ne b$, $2a+2b=1$. The isospectral operators $\operatorname{diag}(a,a,b,b)$ and $\operatorname{diag}(a,b,a,b)$ have invariants $4ab$ and $2(a^2+b^2)$, respectively, and cannot be interconverted. For the exceptional case $\ell=1$, $\mathfrak{sp}(1)=\mathfrak{su}(2)$, so b1 cannot be decided from inclusion alone; equality gives density-state controllability.

**b2 is not implied by the displayed relation: more information is needed.** It permits the full symplectic algebra but also a single commuting generator, or even zero generators. The full $Sp(\ell)$ is [pure-state controllable](../../../../../../pure-state-controllability.md): identify $\mathbb C^{2\ell}$ with $\mathbb H^\ell$, extend any unit vector to a quaternionic orthonormal basis, and map one such basis to another. A one-axis diagonal subgroup, in contrast, cannot change [level populations](../../../../../../quantum-state-population.md).

The required extra information is the generated algebra, obtained by computing its real span of iterated [commutators](../../../../../../commutator.md). Within this specified symplectic inclusion, equality $\mathfrak g=\mathfrak{sp}(\ell)$ gives pure-state controllability; its dimension is $\ell(2\ell+1)$. The mere inclusion does not establish equality. For $N=2$, equality also answers b1 affirmatively. None of these strictly symplectic generators supplies arbitrary [global phase](../../../../../../global-phase.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
