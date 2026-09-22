<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The two [density operators](../../../../../../density-matrix.md) have the same [eigenvalues](../../../../../../eigenvalue.md) $a,a,b,b$, so a permutation of basis vectors makes them [unitarily equivalent](../../../../../../unitary-equivalence.md). A dynamical equivalence must additionally respect the [symplectic dynamical symmetry in quantum control](../../../../../../symplectic-dynamical-symmetry-in-quantum-control.md).

Define the symplectic dual $\widetilde\rho=J\rho^TJ^\dagger$. For a unitary $U$ preserving $J$, both $U^TJU=J$ and $UJU^T=J$ hold. In particular $JU^*=UJ$, and therefore

$$
\widetilde{U\rho U^\dagger}=J U^*\rho^T U^T J^\dagger=U\widetilde\rho U^\dagger.
$$

It follows by cyclicity of the [trace](../../../../../../matrix-trace.md) that the [symplectic invariant of a density operator](../../../../../../symplectic-invariant-of-a-density-operator.md)

$$
I_J(\rho)=\operatorname{Tr}(\rho\widetilde\rho)
$$

is unchanged by every reachable [unitary conjugation](../../../../../../unitary-conjugation.md). The given $J$ reverses the diagonal order, so

$$
\widetilde\rho_0=\operatorname{diag}(b,b,a,a),\qquad\widetilde\rho_1=\operatorname{diag}(a,b,b,a)=\rho_1.
$$

Consequently

$$
I_J(\rho_0)=4ab,\qquad I_J(\rho_1)=2(a^2+b^2),\qquad I_J(\rho_1)-I_J(\rho_0)=2(a-b)^2>0.
$$

Hence **the states are not dynamically equivalent**, despite their identical ordinary spectra. This works for all the allowed values, including $a=0$, and for any subgroup satisfying the symmetry in part (c).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
