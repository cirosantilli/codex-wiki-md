<h1 id="section-c/c11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Hermitian operator](../../../../../../hermitian-operator.md) satisfies the adjoint symmetry condition

$$
\langle\phi|\widehat A\psi\rangle=\langle\widehat A\phi|\psi\rangle
$$

for vectors in its specified domain. For a finite matrix this means $A=A^\dagger$. For an unbounded differential operator, boundary conditions and domains matter: symmetry on a chosen domain is not alone sufficient for [self-adjointness](../../../../../../self-adjoint-operator.md). Physical observables require the corresponding [self-adjoint operator](../../../../../../self-adjoint-operator.md) and its spectral measure. This distinction prevents purely formal integration by parts from being mistaken for a complete operator definition.

**Real [eigenvalues](../../../../../../eigenvalue.md).** If $A|a\rangle=a|a\rangle$ with nonzero norm, Hermiticity implies

$$
a\langle a|a\rangle=\langle a|A|a\rangle
=\langle a|A|a\rangle^*=a^*\langle a|a\rangle,
$$

so $a=a^*$. Thus [eigenvalues](../../../../../../eigenvalue.md) representing measurement outcomes are real.

**[Orthogonality](../../../../../../orthogonal-vectors.md).** For eigenvectors $|a\rangle,|b\rangle$,

$$
a\langle b|a\rangle=\langle b|A|a\rangle
=\langle Ab|a\rangle=b\langle b|a\rangle.
$$

Hence $(a-b)\langle b|a\rangle=0$, and distinct [eigenvalues](../../../../../../eigenvalue.md) have orthogonal eigenvectors. Within a degenerate eigenspace, [Gram-Schmidt orthogonalization](../../../../../../gram-schmidt-process.md) can choose an [orthonormal basis](../../../../../../orthonormal-basis.md). In finite dimensions the [spectral theorem](../../../../../../spectral-theorem.md) gives a complete orthonormal eigenbasis and

$$
\boxed{A=\sum_a aP_a,\qquad I=\sum_aP_a,}
$$

where $P_a$ projects onto each eigenspace. In infinite dimensions a continuous spectrum may require a spectral integral rather than a normalizable eigenvector for every possible outcome; a [position operator](../../../../../../position-operator.md) on the full line is a familiar example.

**Measurements and probabilities.** In the discrete case the [Born rule](../../../../../../born-rule.md) assigns [probability](../../../../../../probability.md) $\langle\psi|P_a|\psi\rangle$ to the outcome $a$. For a nondegenerate eigenbasis, $|\psi\rangle=\sum_ac_a|a\rangle$ gives probabilities $|c_a|^2$, with

$$
\langle A\rangle=\sum_a a|c_a|^2\in\mathbb R,\qquad
(\Delta A)^2=\langle(A-\langle A\rangle)^2\rangle\ge0.
$$

The [variance](../../../../../../variance-split.md) vanishes precisely when the state lies in an eigenspace with a single sharp outcome. A repeatable ideal projective measurement prepares the corresponding eigenspace; superpositions of different [eigenvalues](../../../../../../eigenvalue.md) do not have a preassigned sharp value of that observable in this description.

**Compatibility and dynamics.** Commuting Hermitian matrices admit simultaneous diagonalization, permitting a common set of sharp labels. For example $L^2,L_z$ commute, whereas $L_x,L_y$ do not. In the differential-operator setting the corresponding spectral compatibility requires appropriate domain conditions. Noncommuting observables obey the [Robertson uncertainty principle](../../../../../../robertson-uncertainty-principle.md)

$$
\boxed{\Delta A\,\Delta B\ge\frac12|\langle[A,B]\rangle|.}
$$

The [canonical commutation relation](../../../../../../canonical-commutation-relation.md) then gives $\Delta x\Delta p\ge\hbar/2$.

The [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) represents [energy](../../../../../../energy-split.md). A self-adjoint $H$ generates [unitary time evolution](../../../../../../unitary-time-evolution.md), $U(t)=e^{-iHt/\hbar}$, preserving norm and total [probability](../../../../../../probability.md); its [eigenvalues](../../../../../../eigenvalue.md) determine stationary-state phases and transition energies. **Hermiticity supplies real outcomes and orthogonal eigenspaces, while self-adjointness and the spectral theorem make these measurement and evolution rules mathematically complete.**

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
