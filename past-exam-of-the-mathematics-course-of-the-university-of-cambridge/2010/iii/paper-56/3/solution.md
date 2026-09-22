<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the mostly-plus [Clifford algebra](../../../../../clifford-algebra.md) and [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) conventions of the preceding solutions, with $e=\det(e_\mu{}^a)$, $\kappa^2=8\pi G$, and a Majorana [gravitino](../../../../../gravitino.md). An [action](../../../../../action.md) for [minimal four-dimensional supergravity](../../../../../minimal-four-dimensional-supergravity.md) in the exact transformation normalization given is

$$
\boxed{S_0=\int d^4x\,e\left[\frac{R}{2\kappa^2}-2\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho\right]+O(\psi^4).}
$$

The kinetic coefficient is tied to the normalization of the [supersymmetry](../../../../../supersymmetry-split.md) transformations: if $\Psi_\mu=2\psi_\mu$ and $\eta=2\epsilon$, this becomes the canonical coefficient $-1/2$, with $\delta e_\mu{}^a=(\kappa/2)\bar\eta\gamma^a\Psi_\mu$ and $\delta\Psi_\mu=\nabla_\mu\eta/\kappa$. Mixing those two normalizations would spoil the cancellation.

To the retained order, use the torsion-free connection. More generally the [1.5-order formalism](../../../../../1-5-order-formalism.md) allows its variation to be omitted after imposing its own algebraic equation; the resulting contorsion is quadratic in [fermions](../../../../../fermion.md) and first affects the displayed [action](../../../../../action.md) at quartic order. The [metric tensor](../../../../../metric-tensor.md) variation induced by the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) is $\delta g_{\mu\nu}=4\kappa\bar\epsilon\gamma_{(\mu}\psi_{\nu)}$, so the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) varies as

$$
\delta S_{\rm EH}=-\frac2\kappa\int e\,G^{\mu\nu}\bar\epsilon\gamma_\mu\psi_\nu+\text{boundary}.
$$

For the fermionic [action](../../../../../action.md), varying both Majorana factors gives the same contribution after [integration by parts](../../../../../integration-by-parts.md) and the Grassmann bilinear interchange rule. Thus

$$
\delta S_{\rm RS}=-\frac4\kappa\int e\,(\nabla_\mu\bar\epsilon)\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho
=\frac4\kappa\int e\,\bar\epsilon\gamma^{\mu\nu\rho}\nabla_\mu\nabla_\nu\psi_\rho+\text{boundary}.
$$

The vector-index [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) contribution vanishes by the [first Bianchi identity](../../../../../first-bianchi-identity.md). The spin-index contribution is determined by

$$
\gamma^{\rho\mu\nu}\nabla_\mu\nabla_\nu\zeta
=\frac18\gamma^{\rho\mu\nu}R_{\mu\nu ab}\gamma^{ab}\zeta
=\frac12G^{\rho\sigma}\gamma_\sigma\zeta.
$$

For the last equality, expand the antisymmetric three-gamma/two-gamma product: the totally antisymmetric [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) terms vanish by Bianchi, and the surviving terms are the Ricci contraction minus half its trace. Hence

$$
\delta S_{\rm RS}=\frac2\kappa\int e\,G^{\mu\nu}\bar\epsilon\gamma_\mu\psi_\nu+\text{boundary},
$$

which cancels the gravitational variation. Variations of [vierbeins](../../../../../orthonormal-coframe-in-spacetime.md), gamma matrices and the connection in the fermionic kinetic term carry three dynamical [fermions](../../../../../fermion.md). They lie beyond this linear-fermion cancellation and are cancelled by the omitted four-fermion completion. Thus the [action](../../../../../action.md) is invariant up to boundary terms at the order specified, rather than claiming that a truncated [action](../../../../../action.md) is exactly invariant at every [fermion](../../../../../fermion.md) order.

For the cosmological extension, add a [gravitino](../../../../../gravitino.md) [mass](../../../../../mass.md) parameter $m$ and deform the derivative:

$$
\boxed{S_m=\int e\left[\frac{R+6m^2}{2\kappa^2}-2\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho
+2m\bar\psi_\mu\gamma^{\mu\nu}\psi_\nu\right],\quad
\delta\psi_\mu=\frac1\kappa\mathcal D_\mu\epsilon,\quad
\mathcal D_\mu=\nabla_\mu+\frac m2\gamma_\mu.}
$$

Indeed the [fermion](../../../../../fermion.md) terms combine as $-2\bar\psi_\mu\gamma^{\mu\nu\rho}\mathcal D_\nu\psi_\rho$ because $\gamma^{\mu\nu\rho}\gamma_\nu=-2\gamma^{\mu\rho}$. The modified spinor connection curvature is

$$
[\mathcal D_\nu,\mathcal D_\rho]=\frac14R_{\nu\rho ab}\gamma^{ab}+\frac{m^2}{2}\gamma_{\nu\rho},
$$

and contraction gives

$$
\gamma^{\mu\nu\rho}\mathcal D_\nu\mathcal D_\rho\epsilon
=\frac12(G^{\mu\nu}-3m^2g^{\mu\nu})\gamma_\nu\epsilon.
$$

The same action-variation cancellation therefore works with $G$ replaced by $G+\Lambda g$ precisely for

$$
\boxed{\Lambda=-3m^2.}
$$

This is the [Anti-de Sitter deformation of minimal supergravity](../../../../../anti-de-sitter-deformation-of-minimal-supergravity.md). A cosmological term alone would leave its variation uncancelled; the [mass](../../../../../mass.md) term and the gamma shift of the [gravitino](../../../../../gravitino.md) transformation are both necessary. A positive [cosmological constant](../../../../../cosmological-constant.md) cannot arise from this real unbroken minimal deformation.

For electromagnetism, retain $\mathcal N=1$ and introduce an Abelian [vector multiplet](../../../../../supersymmetric-vector-multiplet.md) $(A_\mu,\lambda)$, with Majorana [gaugino](../../../../../gaugino.md) $\lambda$. A complete quadratic-fermion extension is

$$
\boxed{\mathcal L_{\rm vec}=e\left[-\frac14F_{\mu\nu}F^{\mu\nu}-\frac12\bar\lambda\gamma^\mu\nabla_\mu\lambda
-\frac\kappa2\bar\psi_\mu\gamma^{\nu\rho}\gamma^\mu\lambda\,F_{\nu\rho}\right],\qquad F=dA.}
$$

The accompanying leading transformations are

$$
\boxed{\delta A_\mu=\bar\epsilon\gamma_\mu\lambda,\qquad
\delta\lambda=-\frac12\gamma^{\mu\nu}F_{\mu\nu}\epsilon.}
$$

They preserve the rigid Maxwell-gaugino [action](../../../../../action.md) for constant $\epsilon$. For a local parameter, the variation contains

$$
\delta\mathcal L_{\rm rigid}=e(\nabla_\mu\bar\epsilon)j^\mu+\text{boundary},\qquad
j^\mu=\frac12F_{ab}\gamma^{ab}\gamma^\mu\lambda.
$$

To obtain this, vary $F^2$, vary both [gaugino](../../../../../gaugino.md) factors, and use $\gamma^{ab}\gamma^\mu=\gamma^{ab\mu}+g^{b\mu}\gamma^a-g^{a\mu}\gamma^b$. The terms with $\nabla\lambda$ cancel between the two [actions](../../../../../action.md); integrating the three-gamma term uses $\nabla_{[\mu}F_{\nu\rho]}=0$, leaving exactly the displayed derivative of the parameter. The interaction is $-\kappa e\bar\psi_\mu j^\mu$, whose variation under $\delta\bar\psi_\mu=\nabla_\mu\bar\epsilon/\kappa$ cancels that term.

The other linear-fermion variation is also fixed. Put $\mathcal F=F_{ab}\gamma^{ab}$ and $T_{\rm EM}^{\mu\nu}=F^{\mu\rho}F^\nu{}_{\rho}-g^{\mu\nu}F^2/4$. [Clifford multiplication](../../../../../clifford-multiplication.md) gives

$$
\mathcal F\gamma^\mu\mathcal F=8T_{\rm EM}^{\mu\nu}\gamma_\nu.
$$

Varying $\lambda$ in the gravitino-current interaction then gives $2\kappa e T_{\rm EM}^{\mu\nu}\bar\psi_\mu\gamma_\nu\epsilon=-2\kappa eT_{\rm EM}^{\mu\nu}\bar\epsilon\gamma_\nu\psi_\mu$, which cancels the Maxwell [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) variation. This proves the required [supergravity coupling of an Abelian vector multiplet](../../../../../supergravity-coupling-of-an-abelian-vector-multiplet.md) through the retained order.

Beyond that order one uses a supercovariant [gauge field strength](../../../../../gauge-field-strength.md), here $\widehat F_{\mu\nu}=F_{\mu\nu}-2\kappa\bar\psi_{[\mu}\gamma_{\nu]}\lambda$, and the associated higher-fermion transformation terms and four-fermion interactions. An auxiliary scalar may be retained for off-shell closure, or eliminated in this on-shell formulation. A [Maxwell field](../../../../../electromagnetic-field.md) without a fermionic partner cannot be coupled by merely adding $-F^2/4$ while leaving all transformations unchanged. An alternative is an $\mathcal N=2$ gravity multiplet, where the [vector](../../../../../vector.md) is a graviphoton and a second [gravitino](../../../../../gravitino.md) supplies its extra fermionic states; the explicit construction above is the minimal $\mathcal N=1$ matter extension.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
