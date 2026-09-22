<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [quantum bit-flip channel](../../../../quantum-bit-flip-channel.md) has [Kraus operators](../../../../kraus-operator.md)

$$
K_0=\sqrt p\,I,\qquad K_1=\sqrt{1-p}\,X,\qquad
\sum_jK_j^\dagger K_j=I.
$$

Thus

$$
\boxed{\rho_{\rm out}=\mathcal C(\rho_{\rm in})=p\rho_{\rm in}+(1-p)X\rho_{\rm in}X.}
$$

The orthonormal diagonal linear [polarizations](../../../../polarization-waves.md) $|D\rangle=(|H\rangle+|V\rangle)/\sqrt2$ and $|A\rangle=(|H\rangle-|V\rangle)/\sqrt2$ are the [Pauli X eigenstates](../../../../pauli-x-eigenstate.md). Each is transmitted perfectly as a [density operator](../../../../density-matrix-split.md) for every $p$; the possible minus sign on $|A\rangle$ is global. Encode a classical zero and one as $D$ and $A$, then measure in that basis at the receiver. This sends one classical bit per transmitted [qubit](../../../../qubit.md) without error. General superpositions of $D$ and $A$ need not be preserved, because their relative phase is randomized.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
