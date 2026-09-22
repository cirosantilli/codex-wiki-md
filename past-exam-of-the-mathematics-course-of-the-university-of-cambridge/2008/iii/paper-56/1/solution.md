<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Noether gauging procedure](../../../../../noether-gauging-procedure.md) starts by allowing a constant [symmetry](../../../../../symmetry-physics.md) parameter to depend on position. For an internal [symmetry](../../../../../symmetry-physics.md) written as $\delta\phi^i=\epsilon^AT_A\phi^i$, integration by parts identifies the [Noether current](../../../../../noether-current.md):

$$
\delta S_0=\int d^4x\,j_A^\mu\partial_\mu\epsilon^A
$$

up to a boundary term. Introduce a [gauge field](../../../../../gauge-field.md) $A_\mu^A$ and add $-gA_\mu^Aj_A^\mu$, with the inhomogeneous [gauge transformation](../../../../../gauge-transformation.md) $\delta A_\mu^A=g^{-1}\partial_\mu\epsilon^A+\cdots$. This cancels the displayed variation. The current coupling has its own variation, so one iterates: add the needed higher-order interactions and corrections to the [gauge transformations](../../../../../gauge-transformation.md), and require closure of the local [symmetry](../../../../../symmetry-physics.md) algebra. For an ordinary [gauge theory](../../../../../gauge-theory.md), this reorganizes derivatives into [gauge covariant derivatives](../../../../../gauge-covariant-derivative.md) and fixes the nonlinear [gauge field strength](../../../../../gauge-field-strength.md). Gauging is therefore more than replacing a constant parameter by a function.

For rigid [supersymmetry](../../../../../supersymmetry-split.md), the corresponding [Noether current](../../../../../noether-current.md) is the spinor-valued [supercurrent](../../../../../supercurrent.md) $S^\mu$. A local [Majorana spinor](../../../../../majorana-spinor.md) parameter gives a variation proportional to $(\partial_\mu\bar\epsilon)S^\mu$. A [gravitino](../../../../../gravitino.md) $\Psi_\mu$, with an inhomogeneous transformation $\delta\Psi_\mu\sim\kappa^{-1}\partial_\mu\epsilon$, cancels it through a coupling proportional to $\kappa\bar\Psi_\mu S^\mu$. The commutator of two rigid [supersymmetry](../../../../../supersymmetry-split.md) transformations is a translation. With local parameters, the translation parameter becomes position dependent, so the completion must also gauge translations: it introduces the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md), [diffeomorphism invariance of general relativity](../../../../../diffeomorphism-invariance-of-general-relativity.md), and [local Lorentz transformations](../../../../../local-lorentz-transformation.md). The [gravitino](../../../../../gravitino.md) and [graviton](../../../../../graviton.md) thus belong to the same [supergravity multiplet](../../../../../supergravity-multiplet.md).

For pure [minimal four-dimensional supergravity](../../../../../minimal-four-dimensional-supergravity.md), start with the free [massless Fierz-Pauli action](../../../../../massless-fierz-pauli-action.md) and the free [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) kinetic term. The [Noether gauging procedure](../../../../../noether-gauging-procedure.md) replaces the former by the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) and couples the latter to the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) and [spin connection](../../../../../spin-connection.md). In a canonical normalization the leading transformations can be written

$$
\delta e_\mu{}^a=\frac{\kappa}{2}\bar\epsilon\gamma^a\Psi_\mu,
\qquad
\delta\Psi_\mu=\kappa^{-1}\widetilde D_\mu\epsilon.
$$

An overall sign or phase changes with the curvature and [Majorana spinor](../../../../../majorana-spinor.md) conventions, but the relative normalization must be used consistently. To see why these terms fit together, first work to quadratic order in [fermions](../../../../../fermion.md), so the [spin connection](../../../../../spin-connection.md) is torsion free. Varying the [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) kinetic term under $\delta\Psi_\mu=\nabla_\mu\epsilon/\kappa$ produces an antisymmetric double [spinor covariant derivative](../../../../../spinor-covariant-derivative.md). The [spinor curvature identity](../../../../../spinor-curvature-identity.md) and the [Einstein tensor contraction of spin curvature](../../../../../einstein-tensor-contraction-of-spin-curvature.md) give, in the matching curvature convention,

$$
[\nabla_\rho,\nabla_\sigma]\epsilon
=\frac14R_{\rho\sigma ab}\gamma^{ab}\epsilon,
\qquad
\gamma^{\mu\rho\sigma}\nabla_\rho\nabla_\sigma\epsilon
=\frac12G^\mu{}_{\nu}\gamma^\nu\epsilon.
$$

The resulting [Einstein tensor](../../../../../einstein-tensor.md) term cancels the variation of the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) under $\delta e_\mu{}^a$. This is the essential first nontrivial cancellation in the construction.

At higher [fermion](../../../../../fermion.md) order, the variations of the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) and [spin connection](../../../../../spin-connection.md) produce further terms. Treating the [spin connection](../../../../../spin-connection.md) as independent makes its [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) algebraic. Its solution is a [gravitino-induced torsion](../../../../../gravitino-induced-torsion.md) connection. With $\Psi_a=e_a{}^\mu\Psi_\mu$ and $\gamma^{ab}=[\gamma^a,\gamma^b]/2$, a conventional canonical normalization gives

$$
\widetilde\omega_{\mu ab}=\omega_{\mu ab}(e)+K_{\mu ab},
\qquad
K_{\mu ab}=\frac{\kappa^2}{4}
\left(\bar\Psi_\mu\gamma_a\Psi_b-\bar\Psi_\mu\gamma_b\Psi_a
+\bar\Psi_a\gamma_\mu\Psi_b\right).
$$

Equivalently, with $T^a=de^a+\widetilde\omega^a{}_b\wedge e^b$, the [torsion tensor](../../../../../torsion-tensor.md) obeys

$$
T_{\mu\nu}{}^a=\frac{\kappa^2}{2}\bar\Psi_\mu\gamma^a\Psi_\nu.
$$

The [Majorana Grassmann bilinear interchange](../../../../../majorana-grassmann-bilinear-interchange.md) makes the right-hand side antisymmetric in $\mu,\nu$. Eliminating the [spin connection](../../../../../spin-connection.md) generates the four-[fermion](../../../../../fermion.md) completion. In the [1.5-order formalism](../../../../../1-5-order-formalism.md) one substitutes its solution but varies the other fields holding the connection fixed: the omitted chain-rule term is $(\delta S/\delta\omega)\delta\widetilde\omega=0$. The remaining cubic [fermion](../../../../../fermion.md) variations cancel by the [Clifford algebra](../../../../../clifford-algebra.md) and [Fierz rearrangements](../../../../../fierz-identity.md). This produces the displayed [supergravity](../../../../../supergravity.md) action in its compact connection-dependent form. Calling this formulation [on shell](../../../../../on-shell.md) means that no independent [auxiliary fields](../../../../../auxiliary-field.md) have been retained and that closure of the [supersymmetry](../../../../../supersymmetry-split.md) algebra uses the propagating [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md); it does not mean that action invariance is obtained only by setting every variation to zero on a solution.

In the antisymmetrized kinetic term, $\Psi_\sigma$ is a spinor-valued one-form and the derivative is conventionally written

$$
\widetilde D_\rho\Psi_\sigma
=\partial_\rho\Psi_\sigma+\frac14\widetilde\omega_{\rho ab}\gamma^{ab}\Psi_\sigma,
\qquad \gamma_\nu=e_\nu{}^a\gamma_a.
$$

This is the Lorentz-covariant exterior-derivative convention for that term. If one instead uses the full affine [covariant derivative](../../../../../covariant-derivative.md) of a vector-spinor, a coordinate-index connection is also present and the antisymmetrization must include its [torsion tensor](../../../../../torsion-tensor.md) correction. The crucial physical distinction from pure metric [general relativity](../../../../../general-relativity-split.md) is **the spin connection contains gravitino-induced contorsion, rather than being the torsion-free Levi-Civita connection**. It reduces to the ordinary [spinor covariant derivative](../../../../../spinor-covariant-derivative.md) when the [gravitino](../../../../../gravitino.md) vanishes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
