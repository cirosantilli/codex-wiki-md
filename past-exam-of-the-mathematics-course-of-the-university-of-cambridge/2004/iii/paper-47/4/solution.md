<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose a definite matrix convention: $A_\mu=A_\mu^aT_a$, $\omega=\omega^aT_a$, and $D_\mu=\partial_\mu+eA_\mu$. Matter transforms as $\psi'=U\psi$, so gauge covariance requires $D_\mu'=UD_\mu U^{-1}$. Applying both sides to a test field yields the [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md)

$$
\boxed{A_\mu'=UA_\mu U^{-1}-\frac1e(\partial_\mu U)U^{-1}.}
$$

Define the [Yang-Mills field strength](../../../../../gauge-field-strength.md) by $[D_\mu,D_\nu]=eF_{\mu\nu}$:

$$
\boxed{F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+e[A_\mu,A_\nu],\qquad
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a
+e f^{bca}A_\mu^bA_\nu^c.}
$$

Conjugating the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) [commutator](../../../../../commutator.md) proves $F_{\mu\nu}'=UF_{\mu\nu}U^{-1}$: unlike the connection, the [gauge field strength](../../../../../gauge-field-strength.md) has no inhomogeneous [derivative](../../../../../derivative.md) term. The trace normalization supplies an invariant color metric; its [Lie algebra structure constants](../../../../../structure-constant-of-a-lie-algebra.md) with all indices lowered are antisymmetric.

For $U=1+e\omega+O(\omega^2)$ and $U^{-1}=1-e\omega+O(\omega^2)$, expand the finite transformations:

$$
\delta A_\mu=e[\omega,A_\mu]-\partial_\mu\omega
=-D_\mu^{\mathrm{ad}}\omega,
\qquad
\delta F_{\mu\nu}=e[\omega,F_{\mu\nu}],
\qquad D_\mu^{\mathrm{ad}}\omega=\partial_\mu\omega+e[A_\mu,\omega].
$$

In components this is

$$
\boxed{\delta A_\mu^a=-\partial_\mu\omega^a-e f^{abc}A_\mu^b\omega^c,
\qquad\delta F_{\mu\nu}^a=-e f^{abc}F_{\mu\nu}^b\omega^c.}
$$

A convention using the opposite matter transformation or [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) sign changes these signs consistently. The formulas above all follow from the explicitly chosen $D_\mu$.

**Gauge reduction and the determinant.** A direct [integral](../../../../../integral.md) $\int\mathcal DA\,e^{iS[A]}$ integrates repeatedly over gauge-equivalent configurations. The [gauge group](../../../../../gauge-group.md) volume is infinite, and the ungauge-fixed quadratic operator has longitudinal zero directions, so it has no ordinary inverse [quantum field theory propagator](../../../../../propagator.md). Gauge-invariant observables require dividing out this redundancy rather than treating it as an ordinary physical fluctuation.

The finite-dimensional change-of-variables identity underlying [gauge fixing](../../../../../gauge-fixing.md) is precise. Suppose a condition $\chi(x^\alpha)=f$ has one solution in the group-coordinate patch and its [derivative](../../../../../derivative.md) matrix at the solution is nonsingular. Then

$$
\int d\alpha\,\delta^{(r)}(\chi(x^\alpha)-f)
\left|\det\frac{\partial\chi(x^\alpha)}{\partial\alpha}\right|=1.
$$

For several isolated solutions it instead counts those solutions. On the slice, the [Jacobian determinant](../../../../../jacobian-determinant.md) can be factored into the reciprocal of the orbit [integral](../../../../../integral.md) of the delta function. An invariant measure and invariant integrand then allow the group volume to factor out. In the functional version, group coordinates carry [Haar measure](../../../../../haar-measure.md) and the corresponding operator determinant replaces the matrix determinant.

For example, choose the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $\chi^a(A)=\partial^\mu A_\mu^a=f^a$. Its variation is $\delta\chi^a=-\partial^\mu(D_\mu^{\mathrm{ad}}\omega)^a$. Hence on the gauge slice the [Faddeev-Popov operator](../../../../../faddeev-popov-operator.md) and [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) are

$$
M^{ab}[A]=-\partial^\mu D_\mu^{ab}[A],\qquad
\Delta_{\mathrm{FP}}[A]=\det M[A].
$$

Its extension along each local [gauge orbit](../../../../../gauge-orbit.md) yields the [Faddeev-Popov gauge-orbit identity](../../../../../faddeev-popov-gauge-orbit-identity.md)

$$
1=\Delta_{\mathrm{FP}}[A]\int\mathcal DU\,
\delta[\partial^\mu A_\mu^U-f].
$$

For an unoriented finite-dimensional real [integral](../../../../../integral.md) the absolute determinant is required. In a perturbative gauge patch, its sign or phase is fixed and the constant convention is absorbed in normalization. Residual zero modes must be removed by boundary conditions or separate treatment. Multiple intersections, the [Gribov ambiguity](../../../../../gribov-ambiguity.md), prevent interpreting this as a globally unique gauge slice without additional work.

Insert the identity, change variables along the orbit using invariance of the action and measure, and divide out the common [gauge group](../../../../../gauge-group.md) volume. Averaging $f$ with Gaussian weight $\exp[-i\int f^af^a/(2\xi)]$ produces the covariant gauge-fixed functional

$$
Z_{\mathrm{gf}}\propto\int\mathcal DA\,\det M[A]\,
\exp\left\{iS[A]-\frac{i}{2\xi}\int d^4x\,(\partial^\mu A_\mu^a)^2\right\}.
$$

The added term makes the quadratic gauge-field operator invertible after the stated residual-mode treatment.

**Ghost representation.** For a finite matrix $M$, the [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md) over independent anticommuting variables is proportional to its determinant:

$$
\int\prod_a d\overline c_a\,dc_a\,
\exp(i\overline c_aM_{ab}c_b)=\mathrm{constant}\times\det M.
$$

The constant is independent of $M$ and depends on ordering and factors of $i$. The functional counterpart introduces [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) $c^a$ and [antighost fields](../../../../../faddeev-popov-antighost-field.md) $\overline c^a$, with

$$
S_{\mathrm{gh}}=\int d^4x\,\overline c^aM^{ab}[A]c^b
=-\int d^4x\,\overline c^a\partial^\mu(D_\mu c)^a.
$$

Integration by parts writes its density as $(\partial^\mu\overline c^a)(D_\mu c)^a$, displaying a [kinetic term](../../../../../kinetic-term.md) and a gauge-field/ghost interaction. These are [Grassmann-valued fields](../../../../../grassmann-field.md) with scalar Lorentz transformation law. They represent the orbit [Jacobian determinant](../../../../../jacobian-determinant.md); their closed loops carry the fermionic minus sign, and they are not physical asymptotic particles. In the abelian case $D^{\mathrm{ad}}=\partial$, the determinant is gauge-field independent and the ghosts decouple. Nonabelian ghosts interact and are necessary for the consistent cancellation of unphysical gauge contributions.

**Physical-state reduction.** Let $Q$ be the [Hermitian](../../../../../hermitian-operator.md) [BRST charge](../../../../../brst-charge.md). Its key algebraic property is [BRST nilpotence](../../../../../brst-nilpotence.md), $Q^2=0$, and the gauge-fixed dynamics preserves it. Physical states are its [BRST cohomology](../../../../../brst-cohomology.md) at [ghost number](../../../../../ghost-number.md) zero:

$$
\boxed{\mathcal H_{\mathrm{phys}}=
\frac{\ker Q\,\big|_{\mathrm{gh}=0}}{\operatorname{im}Q\,\big|_{\mathrm{gh}=0}},
\qquad Q|\psi\rangle=0,
\qquad |\psi\rangle\sim|\psi\rangle+Q|\chi\rangle.}
$$

Here $|\chi\rangle$ has [ghost number](../../../../../ghost-number.md) $-1$. [BRST nilpotence](../../../../../brst-nilpotence.md) ensures that exact vectors lie in the [kernel](../../../../../kernel-of-a-linear-map.md), so the quotient is defined. Because $Q$ is [Hermitian](../../../../../hermitian-operator.md), an exact vector is orthogonal to every closed vector, $\langle\psi|Q\chi\rangle=\langle Q\psi|\chi\rangle=0$, and exact vectors are null, $\langle Q\chi|Q\chi\rangle=\langle\chi|Q^2\chi\rangle=0$. They therefore represent no independent physical state. Commutation of $Q$ with the [Hamiltonian](../../../../../hamiltonian.md) preserves these classes under time evolution.

The [covariant gauge](../../../../../covariant-gauge.md)/ghost space before reduction has an [indefinite inner product](../../../../../indefinite-hermitian-form.md). This is essential: [a Hermitian nilpotent BRST charge requires an indefinite auxiliary space](../../../../../a-hermitian-nilpotent-brst-charge-requires-an-indefinite-auxiliary-space.md) if it is nonzero. On an ordinary positive-definite [Hilbert space](../../../../../hilbert-space-split.md) the same norm identity would force $Q=0$. Positivity of the resulting physical space uses the gauge-theory structure in addition to the abstract [BRST nilpotence](../../../../../brst-nilpotence.md) identities.

For a nonzero on-shell photon momentum, the one-particle conclusion is

$$
\boxed{k^\mu\varepsilon_\mu=0,\qquad
\varepsilon_\mu\sim\varepsilon_\mu+\alpha k_\mu.}
$$

The second relation preserves the first because $k^2=0$. In four dimensions the transverse [kernel](../../../../../kernel-of-a-linear-map.md) has dimension three, and quotienting by its null longitudinal direction leaves two physical photon polarizations. This is the [positive one-particle BRST cohomology](../../../../../positive-one-particle-brst-cohomology.md) of the photon sector.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
