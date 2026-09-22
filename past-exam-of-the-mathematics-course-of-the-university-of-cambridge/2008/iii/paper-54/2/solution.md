<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [CPT theorem](../../../../../cpt-theorem.md) is a structural consequence of relativistic [quantum field theory](../../../../../quantum-field-theory-split.md). In flat spacetime, assume a positive physical state space, the [positive-energy spectrum condition](../../../../../positive-energy-spectrum-condition.md), [Lorentz invariance](../../../../../lorentz-invariance.md), [microcausality](../../../../../microcausality.md), the usual [Spin-statistics theorem](../../../../../spin-statistics-theorem.md), and a Hermitian dynamics. For ordinary field theories these are realized by a local Hermitian Lorentz-scalar [Lagrangian density](../../../../../lagrangian-density.md). There is then an [antiunitary operator](../../../../../antiunitary-operator.md) $\Theta$ implementing the combined [charge conjugation](../../../../../charge-conjugation.md), [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md) and [time-reversal symmetry](../../../../../t-symmetry.md), with a [CPT](../../../../../cpt-symmetry.md)-invariant vacuum. **The combined symmetry is required even when the three separate symmetries fail.**

Under the combined spacetime transformation, $x\mapsto-x$. A complex [scalar field](../../../../../scalar-field.md) can be taken to transform into its adjoint at $-x$; a Hermitian vector field transforms into minus itself at $-x$. A derivative contributes a minus sign through differentiation of its reflected argument. For a [Dirac field](../../../../../dirac-field.md) the transformation supplied in the paper may be written

$$
\Theta\psi(x)\Theta^{-1}=\gamma_5^T\psi^\dagger(-x)^T.
$$

Field phases are conventional and do not affect the physical conclusions. Crucially, [antiunitarity](../../../../../antiunitary-operator.md) means $\Theta i\Theta^{-1}=-i$ and conjugates every numerical coefficient. The reversal of time is compatible with positive energies because this conjugation changes $e^{-iHt}$ to $e^{iHt}$ while leaving the Hamiltonian invariant. Treating [time reversal](../../../../../t-symmetry.md) as a unitary change of coordinates would instead give incorrect signs.

One can see explicitly how the [CPT transformation of Dirac bilinears](../../../../../cpt-transformation-of-dirac-bilinears.md) works. Let $B_\Gamma(x)=:\psi^\dagger\gamma^0\Gamma\psi:$ be a Hermitian [fermion bilinear](../../../../../fermion-bilinear.md), with $\Gamma^\dagger=\gamma^0\Gamma\gamma^0$. The colons indicate normal ordering so that the graded reordering below has no vacuum contact term. Using the reflected fields and conjugating $\gamma^0\Gamma$, then interchanging the two [fermion](../../../../../fermion.md) factors, gives

$$
\begin{aligned}
\Theta B_\Gamma(x)\Theta^{-1}
&=:\psi^T\gamma_5^*(\gamma^0\Gamma)^*\gamma_5^T\psi^{\dagger T}:_{-x}\\
&=-:\psi^\dagger\gamma_5(\gamma^0\Gamma)^\dagger\gamma_5\psi:_{-x}\\
&=:\overline\psi\gamma_5\Gamma\gamma_5\psi:_{-x}.
\end{aligned}
$$

The last step uses the Dirac-Hermiticity condition and $\{\gamma^0,\gamma_5\}=0$. The identities for the [gamma matrices](../../../../../gamma-matrices.md) then give

$$
\begin{array}{c|c|c}
\text{bilinear}&\Gamma&\text{CPT sign}\\\hline
\text{scalar}&1&+\\
\text{pseudoscalar}&i\gamma_5&+\\
\text{vector}&\gamma^\mu&-\\
\text{axial vector}&\gamma^\mu\gamma_5&-\\
\text{tensor}&\frac{i}{2}[\gamma^\mu,\gamma^\nu]&+
\end{array}
$$

The pseudoscalar's sign is particularly instructive: its explicit $i$ must also be conjugated. The minus sign from exchanging [fermions](../../../../../fermion.md) is equally essential. These signs depend on the number of free vector indices, rather than on a field's separate parity assignment.

This supplies a [local Lagrangian argument for CPT invariance](../../../../../local-lagrangian-argument-for-cpt-invariance.md). Hermitian local field combinations with $r$ vector indices transform with sign $(-1)^r$, including the appropriate reordered derivative terms. A [Lorentz scalar](../../../../../lorentz-scalar.md) contracts those indices in pairs or with four-index invariant tensors, giving a positive total sign. For charged terms, the reflected conjugate fields and conjugated coefficients exchange a term with its Hermitian-conjugate partner. Thus

$$
\boxed{\Theta\mathcal L(x)\Theta^{-1}=\mathcal L(-x),\qquad
\Theta S_{\mathrm{action}}\Theta^{-1}=S_{\mathrm{action}}.}
$$

The integration variable $x\mapsto-x$ has unit absolute Jacobian. The general field-index argument is discussed in [Srednicki's treatment of discrete symmetries, section 40](https://web.physics.ucsb.edu/~mark/ms-qft-DRAFT.pdf).

For example, the scalar mass term $\overline\psi\psi$ is even. The [Dirac electromagnetic current](../../../../../dirac-electromagnetic-current.md) and vector potential are both odd, making their contracted interaction even. The Hermitian Dirac kinetic term $(i/2)\overline\psi\gamma^\mu\overleftrightarrow{\partial}_\mu\psi$ is also even: reflection and reordering interchange the two derivative placements, while [antiunitarity](../../../../../antiunitary-operator.md) conjugates its $i$. A complex [Yukawa coupling](../../../../../yukawa-interaction.md) and its Hermitian conjugate are exchanged rather than requiring the coupling itself to be real. Hence [CP violation](../../../../../cp-violation.md) in the [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) is compatible with exact [CPT](../../../../../cpt-symmetry.md). Renormalizability is not necessary: local Hermitian higher-dimensional Lorentz-scalar operators satisfy the same argument.

The axiomatic form of the [CPT theorem](../../../../../cpt-theorem.md) does not start by assuming a polynomial [Lagrangian density](../../../../../lagrangian-density.md). The [positive-energy spectrum condition](../../../../../positive-energy-spectrum-condition.md) provides analytic continuations of [Wightman functions](../../../../../wightman-function.md), and complexified [Lorentz transformations](../../../../../lorentz-transformation.md) relate configurations to their total spacetime inversions. At suitable spacelike configurations, [microcausality](../../../../../microcausality.md) permits reversal of the order of field operators with the signs dictated by the [Spin-statistics theorem](../../../../../spin-statistics-theorem.md). Uniqueness of [analytic continuation](../../../../../analytic-continuation.md) extends this relation to the correlators generally, from which the Hilbert-space [antiunitary operator](../../../../../antiunitary-operator.md) is obtained. This explains why locality and positive energy are genuine hypotheses, not incidental features of a particular interaction. The elementary argument above displays the mechanism for the scalar, spinor and vector fields relevant to the [Standard Model](../../../../../standard-model-split.md); it is not a substitute for all the analytic steps of the axiomatic proof.

For one-particle states, [CPT](../../../../../cpt-symmetry.md) reverses additive charges and spin projections. The spatial momentum is unchanged by the combination: [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md) and [time reversal](../../../../../t-symmetry.md) each reverse it. Thus, up to phases,

$$
\Theta|\boldsymbol p,s,q\rangle
=|\boldsymbol p,-s,-q\rangle.
$$

Since the energy-momentum spectrum is preserved, the [CPT constraints on particle properties](../../../../../cpt-constraints-on-particle-properties.md) give **equal particle-antiparticle masses, equal spin magnitudes, and opposite conserved additive charges**. Relating the corresponding two-point functions also fixes equal pole positions, so unstable conjugate particles have equal total [decay widths](../../../../../decay-width.md), hence equal lifetimes. Magnetic moments at the same chosen spin orientation have opposite signs. These are precise experimental tests of [CPT](../../../../../cpt-symmetry.md), not tests that every individual discrete symmetry is respected.

For scattering, [CPT](../../../../../cpt-symmetry.md) interchanges incoming and outgoing boundary conditions. The [antiunitary operator](../../../../../antiunitary-operator.md) identity $\langle a|b\rangle=\langle\Theta b|\Theta a\rangle$ relates $\langle f,\mathrm{out}|i,\mathrm{in}\rangle$ to the amplitude with transformed $f$ incoming and transformed $i$ outgoing. Thus the reversed process with antiparticles and reversed spins has the same transition probability. This is not, in general, equality with the forward CP-conjugate process. In particular, [CP violation](../../../../../cp-violation.md) can make corresponding partial [decay widths](../../../../../decay-width.md) different while their complete sums remain equal. With [CPT](../../../../../cpt-symmetry.md) preserved, genuine [CP violation](../../../../../cp-violation.md) requires corresponding [time-reversal symmetry](../../../../../t-symmetry.md) violation.

Finally, a proposed [CPT](../../../../../cpt-symmetry.md) violation requires revisiting at least one assumption: for example, a nonlocal interaction, a preferred spacetime direction violating [Lorentz invariance](../../../../../lorentz-invariance.md), or loss of unitary Hermitian dynamics. A generic curved background need not possess the global spacetime inversion used here. Those observations delimit the theorem; they do not weaken its prediction for the ordinary local [Standard Model](../../../../../standard-model-split.md) in Minkowski spacetime.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
