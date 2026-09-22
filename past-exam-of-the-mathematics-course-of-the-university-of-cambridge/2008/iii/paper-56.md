# Paper 56

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper56.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper56.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Noether gauging procedure](../../../quantum-field-theory.md#noether-gauging-procedure) starts by allowing a constant [symmetry](../../../physics.md#symmetry-physics) parameter to depend on position. For an internal [symmetry](../../../physics.md#symmetry-physics) written as $\delta\phi^i=\epsilon^AT_A\phi^i$, integration by parts identifies the [Noether current](../../../quantum-field-theory.md#noether-current):

$$
\delta S_0=\int d^4x\,j_A^\mu\partial_\mu\epsilon^A
$$

up to a boundary term. Introduce a [gauge field](../../../relativistic-quantum-field.md#gauge-field) $A_\mu^A$ and add $-gA_\mu^Aj_A^\mu$, with the inhomogeneous [gauge transformation](../../../electromagnetism.md#gauge-transformation) $\delta A_\mu^A=g^{-1}\partial_\mu\epsilon^A+\cdots$. This cancels the displayed variation. The current coupling has its own variation, so one iterates: add the needed higher-order interactions and corrections to the [gauge transformations](../../../electromagnetism.md#gauge-transformation), and require closure of the local [symmetry](../../../physics.md#symmetry-physics) algebra. For an ordinary [gauge theory](../../../quantum-field-theory.md#gauge-theory), this reorganizes derivatives into [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative) and fixes the nonlinear [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength). Gauging is therefore more than replacing a constant parameter by a function.

For rigid [supersymmetry](../../../supersymmetry.md), the corresponding [Noether current](../../../quantum-field-theory.md#noether-current) is the spinor-valued [supercurrent](../../../supersymmetry.md#supercurrent) $S^\mu$. A local [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) parameter gives a variation proportional to $(\partial_\mu\bar\epsilon)S^\mu$. A [gravitino](../../../supersymmetry.md#gravitino) $\Psi_\mu$, with an inhomogeneous transformation $\delta\Psi_\mu\sim\kappa^{-1}\partial_\mu\epsilon$, cancels it through a coupling proportional to $\kappa\bar\Psi_\mu S^\mu$. The commutator of two rigid [supersymmetry](../../../supersymmetry.md) transformations is a translation. With local parameters, the translation parameter becomes position dependent, so the completion must also gauge translations: it introduces the [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime), [diffeomorphism invariance of general relativity](../../../general-relativity.md#diffeomorphism-invariance-of-general-relativity), and [local Lorentz transformations](../../../special-relativity.md#local-lorentz-transformation). The [gravitino](../../../supersymmetry.md#gravitino) and [graviton](../../../quantum-theory.md#graviton) thus belong to the same [supergravity multiplet](../../../supersymmetry.md#supergravity-multiplet).

For pure [minimal four-dimensional supergravity](../../../supersymmetry.md#minimal-four-dimensional-supergravity), start with the free [massless Fierz-Pauli action](../../../general-relativity.md#massless-fierz-pauli-action) and the free [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field) kinetic term. The [Noether gauging procedure](../../../quantum-field-theory.md#noether-gauging-procedure) replaces the former by the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) and couples the latter to the [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) and [spin connection](../../../connection-1-form.md#spin-connection). In a canonical normalization the leading transformations can be written

$$
\delta e_\mu{}^a=\frac{\kappa}{2}\bar\epsilon\gamma^a\Psi_\mu,
\qquad
\delta\Psi_\mu=\kappa^{-1}\widetilde D_\mu\epsilon.
$$

An overall sign or phase changes with the curvature and [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) conventions, but the relative normalization must be used consistently. To see why these terms fit together, first work to quadratic order in [fermions](../../../quantum-mechanics.md#fermion), so the [spin connection](../../../connection-1-form.md#spin-connection) is torsion free. Varying the [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field) kinetic term under $\delta\Psi_\mu=\nabla_\mu\epsilon/\kappa$ produces an antisymmetric double [spinor covariant derivative](../../../connection-1-form.md#spinor-covariant-derivative). The [spinor curvature identity](../../../connection-1-form.md#spinor-curvature-identity) and the [Einstein tensor contraction of spin curvature](../../../connection-1-form.md#einstein-tensor-contraction-of-spin-curvature) give, in the matching curvature convention,

$$
[\nabla_\rho,\nabla_\sigma]\epsilon
=\frac14R_{\rho\sigma ab}\gamma^{ab}\epsilon,
\qquad
\gamma^{\mu\rho\sigma}\nabla_\rho\nabla_\sigma\epsilon
=\frac12G^\mu{}_{\nu}\gamma^\nu\epsilon.
$$

The resulting [Einstein tensor](../../../general-relativity.md#einstein-tensor) term cancels the variation of the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) under $\delta e_\mu{}^a$. This is the essential first nontrivial cancellation in the construction.

At higher [fermion](../../../quantum-mechanics.md#fermion) order, the variations of the [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) and [spin connection](../../../connection-1-form.md#spin-connection) produce further terms. Treating the [spin connection](../../../connection-1-form.md#spin-connection) as independent makes its [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) algebraic. Its solution is a [gravitino-induced torsion](../../../supersymmetry.md#gravitino-induced-torsion) connection. With $\Psi_a=e_a{}^\mu\Psi_\mu$ and $\gamma^{ab}=[\gamma^a,\gamma^b]/2$, a conventional canonical normalization gives

$$
\widetilde\omega_{\mu ab}=\omega_{\mu ab}(e)+K_{\mu ab},
\qquad
K_{\mu ab}=\frac{\kappa^2}{4}
\left(\bar\Psi_\mu\gamma_a\Psi_b-\bar\Psi_\mu\gamma_b\Psi_a
+\bar\Psi_a\gamma_\mu\Psi_b\right).
$$

Equivalently, with $T^a=de^a+\widetilde\omega^a{}_b\wedge e^b$, the [torsion tensor](../../../fiber-bundle.md#torsion-tensor) obeys

$$
T_{\mu\nu}{}^a=\frac{\kappa^2}{2}\bar\Psi_\mu\gamma^a\Psi_\nu.
$$

The [Majorana Grassmann bilinear interchange](../../../relativistic-quantum-field.md#majorana-grassmann-bilinear-interchange) makes the right-hand side antisymmetric in $\mu,\nu$. Eliminating the [spin connection](../../../connection-1-form.md#spin-connection) generates the four-[fermion](../../../quantum-mechanics.md#fermion) completion. In the [1.5-order formalism](../../../general-relativity.md#1-5-order-formalism) one substitutes its solution but varies the other fields holding the connection fixed: the omitted chain-rule term is $(\delta S/\delta\omega)\delta\widetilde\omega=0$. The remaining cubic [fermion](../../../quantum-mechanics.md#fermion) variations cancel by the [Clifford algebra](../../../algebra.md#clifford-algebra) and [Fierz rearrangements](../../../quantum-field-theory.md#fierz-identity). This produces the displayed [supergravity](../../../supersymmetry.md#supergravity) action in its compact connection-dependent form. Calling this formulation [on shell](../../../quantum-field-theory.md#on-shell) means that no independent [auxiliary fields](../../../supersymmetry.md#auxiliary-field) have been retained and that closure of the [supersymmetry](../../../supersymmetry.md) algebra uses the propagating [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation); it does not mean that action invariance is obtained only by setting every variation to zero on a solution.

In the antisymmetrized kinetic term, $\Psi_\sigma$ is a spinor-valued one-form and the derivative is conventionally written

$$
\widetilde D_\rho\Psi_\sigma
=\partial_\rho\Psi_\sigma+\frac14\widetilde\omega_{\rho ab}\gamma^{ab}\Psi_\sigma,
\qquad \gamma_\nu=e_\nu{}^a\gamma_a.
$$

This is the Lorentz-covariant exterior-derivative convention for that term. If one instead uses the full affine [covariant derivative](../../../general-relativity.md#covariant-derivative) of a vector-spinor, a coordinate-index connection is also present and the antisymmetrization must include its [torsion tensor](../../../fiber-bundle.md#torsion-tensor) correction. The crucial physical distinction from pure metric [general relativity](../../../general-relativity.md) is **the spin connection contains gravitino-induced contorsion, rather than being the torsion-free Levi-Civita connection**. It reduces to the ordinary [spinor covariant derivative](../../../connection-1-form.md#spinor-covariant-derivative) when the [gravitino](../../../supersymmetry.md#gravitino) vanishes.

## 2

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the [Clifford algebra](../../../algebra.md#clifford-algebra) $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$ and unit-weight antisymmetrization. The duality identity between $\gamma_5\gamma_\nu$ and three antisymmetrized [gamma matrices](../../../algebra.md#gamma-matrices) turns the equation into

$$
E^\mu:=\gamma^{\mu\nu\rho}\partial_\nu\Psi_\rho=0,
\qquad \gamma^{\mu\nu\rho}=\gamma^{[\mu}\gamma^\nu\gamma^{\rho]}.
$$

The overall nonzero factor in this identity depends on the orientation and $\gamma_5$ convention and does not change its solutions. This [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field) equation has the [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance)

$$
\Psi_\mu\longmapsto\Psi_\mu+\partial_\mu\epsilon,
$$

since $\gamma^{\mu\nu\rho}\partial_\nu\partial_\rho\epsilon=0$. It is the free-field limit of local [supersymmetry](../../../supersymmetry.md), so it is suitable for the [gravitino](../../../supersymmetry.md#gravitino).

To check which [spin](../../../quantum-mechanics.md#spin) it propagates, put $A=\gamma^\mu\Psi_\mu$ and $B=\partial^\mu\Psi_\mu$. Expanding the three [gamma matrices](../../../algebra.md#gamma-matrices) using the [Clifford algebra](../../../algebra.md#clifford-algebra) gives

$$
E^\mu=\not\partial\Psi^\mu-\partial^\mu A
+\gamma^\mu(\not\partial A-B),
\qquad
\gamma_\mu E^\mu=2(\not\partial A-B)
$$

in four dimensions. Thus the [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) requires $B=\not\partial A$. Under the [gauge transformation](../../../electromagnetism.md#gauge-transformation), $A\mapsto A+\not\partial\epsilon$; locally one may choose gamma-trace [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing), $A=0$, by solving $\not\partial\epsilon=-A$. The [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) then yields

$$
\gamma^\mu\Psi_\mu=0,
\qquad \partial^\mu\Psi_\mu=0,
\qquad \not\partial\Psi_\mu=0.
$$

These are the [massless Dirac equation](../../../relativistic-quantum-field.md#massless-dirac-equation), transversality and gamma-trace constraints that remove the lower-[spin](../../../quantum-mechanics.md#spin) part of a vector-spinor.

For a more explicit [massless Rarita-Schwinger polarization count](../../../relativistic-quantum-field.md#massless-rarita-schwinger-polarization-count), take a positive-frequency [plane wave](../../../quantum-mechanics.md#plane-wave) with null momentum along the third axis, in signature $(-,+,+,+)$. Transversality relates its temporal and longitudinal components. Residual [gauge transformations](../../../electromagnetism.md#gauge-transformation) with $\not p\epsilon=0$ remove both. Write the surviving components as $u_1,u_2$; their gamma-trace condition reads $\gamma^1u_1+\gamma^2u_2=0$, hence

$$
u_2=\gamma^1\gamma^2u_1,
\qquad \not p\,u_1=0.
$$

The [massless Dirac equation](../../../relativistic-quantum-field.md#massless-dirac-equation) leaves two complex positive-frequency amplitudes in $u_1$. If $i\gamma^1\gamma^2u_1=s u_1$, $s=\pm1$, then $(u_1,u_2)$ is proportional to $(1,-is)$ in the transverse vector index. With spatial rotation generators $J_3^{\mathrm{vec}}{}_{12}=-i$ and $J_3^{\mathrm{spin}}=-i\gamma^1\gamma^2/2$, the vector has [helicity](../../../special-relativity.md#helicity) $-s$ and the [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) has [helicity](../../../special-relativity.md#helicity) $-s/2$, giving total [helicity](../../../special-relativity.md#helicity) $-3s/2$. The [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) condition fixes the negative-frequency coefficients from these amplitudes. Therefore **a massless gravitino has spin $3/2$, with the two physical helicities $\pm3/2$**. A complex vector-spinor would also have independent antiparticle modes.

The requested count is instead the [off-shell component count of minimal supergravity](../../../supersymmetry.md#off-shell-component-count-of-minimal-supergravity), before imposing any [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation). A four-dimensional [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) has four real components. Its vector index supplies four copies, and local [supersymmetry](../../../supersymmetry.md) supplies four real gauge functions:

$$
\boxed{n_{\mathrm{gravitino,off}}=4\times4-4=12.}
$$

One must not additionally subtract transversality and the [massless Dirac equation](../../../relativistic-quantum-field.md#massless-dirac-equation) in this count: those are [on shell](../../../quantum-field-theory.md#on-shell) conditions. The gamma-trace [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) already uses the same four gauge functions subtracted above. For the [graviton](../../../quantum-theory.md#graviton), a symmetric [metric tensor](../../../general-relativity.md#metric-tensor) has ten real components, with four [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) gauge functions. Equivalently, a [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) has sixteen real components, minus six [local Lorentz transformation](../../../special-relativity.md#local-lorentz-transformation) and four [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) functions:

$$
\boxed{n_{\mathrm{graviton,off}}=10-4=16-6-4=6.}
$$

The [gravitino](../../../supersymmetry.md#gravitino) and [graviton](../../../quantum-theory.md#graviton) each have two propagating states [on shell](../../../quantum-field-theory.md#on-shell), but their off-shell counts disagree by six.

An [auxiliary field](../../../supersymmetry.md#auxiliary-field) has an algebraic [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) and no propagating kinetic term. In [old-minimal supergravity](../../../supersymmetry.md#old-minimal-supergravity), a complex scalar $M$ contributes two real bosonic components and a real vector $b_\mu$ contributes four, so the bosonic count becomes $6+2+4=12$, matching the [gravitino](../../../supersymmetry.md#gravitino). Their [supersymmetry](../../../supersymmetry.md) transformations also absorb the terms that would otherwise require the propagating [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation) to close the local algebra. Thus **auxiliary fields allow off-shell supersymmetry closure and matching component counts without adding physical particles**. Eliminating them recovers an [on shell](../../../quantum-field-theory.md#on-shell) formulation.

## 3

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a single [chiral superfield](../../../supersymmetry.md#chiral-superfield), the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential), with $\kappa=m_p^{-1}$ restored, is

$$
V=e^{\kappa^2K}\left(K^{z\bar z}|D_zW|^2-3\kappa^2|W|^2\right),
\qquad D_zW=W_z+\kappa^2K_zW.
$$

The canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) has $K_{z\bar z}=K^{z\bar z}=1$, so the [Kähler covariant derivative of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) is

$$
D_zW=\mu m_p\left[1+\kappa^2\bar z(z+\beta)\right].
$$

Consequently the [Polonyi model](../../../supersymmetry.md#polonyi-model) has the [scalar potential](../../../quantum-field-theory.md#scalar-potential)

$$
\boxed{V=|\mu|^2m_p^2e^{\kappa^2|z|^2}
\left(\left|1+\kappa^2\bar z(z+\beta)\right|^2
-3\kappa^2|z+\beta|^2\right).}
$$

The negative term is essential; retaining only the square of the [supergravity auxiliary field](../../../supersymmetry.md#supergravity-auxiliary-field) would give the global [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential) rather than the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential).

Set $x=\kappa z=a+iy$ and $b=\kappa\beta=2-\sqrt3$. In this notation $V=|\mu|^2m_p^2e^{|x|^2}U$, where

$$
U=\left(1+a^2+y^2+ba\right)^2+b^2y^2
-3\left[(a+b)^2+y^2\right].
$$

At $a_0=\sqrt3-1$, $y=0$, one has $a_0+b=1$ and $1+a_0(a_0+b)=\sqrt3$, so $U=0$. To prove that this is a [local minimum](../../../analysis.md#local-minimum) in both real directions, rather than checking only the real axis, put $u=a-a_0$. Direct expansion gives the [stable zero-energy Polonyi vacuum](../../../supersymmetry.md#stable-zero-energy-polonyi-vacuum) identity

$$
U=\left(u^2+y^2+\sqrt3u\right)^2
+(2\sqrt3-3)u^2+(4-2\sqrt3)y^2.
$$

Every coefficient outside the square is strictly positive, and the exponential factor is positive. Thus $V\ge0$ everywhere and equality requires $u=y=0$, provided $\mu\ne0$. This proves the stronger conclusion

$$
\boxed{\langle z\rangle=(\sqrt3-1)m_p,\qquad V_{\min}=0,}
$$

a unique [global minimum](../../../analysis.md#global-minimum) of this [Polonyi model](../../../supersymmetry.md#polonyi-model). If $\mu=0$, the [scalar potential](../../../quantum-field-theory.md#scalar-potential) vanishes identically and this uniqueness and [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) conclusion do not hold.

For an independent local stability check, the [Hessian matrix](../../../calculus.md#hessian-matrix) of $U$ at this [global minimum](../../../analysis.md#global-minimum) is diagonal:

$$
U_{aa}=4\sqrt3,\qquad U_{yy}=8-4\sqrt3,\qquad U_{ay}=0.
$$

Since $U$ and its first derivatives vanish there, differentiating the exponential introduces no additional [Hessian matrix](../../../calculus.md#hessian-matrix) terms at the [global minimum](../../../analysis.md#global-minimum). For canonically normalized real fluctuations $z=z_0+(s+it)/\sqrt2$, the squared scalar [masses](../../../classical-mechanics.md#mass) are therefore

$$
m_s^2=2\sqrt3\,|\mu|^2e^{a_0^2},
\qquad
m_t^2=2(2-\sqrt3)|\mu|^2e^{a_0^2},
$$

which are both positive.

Although the vacuum energy is zero, the [supergravity auxiliary field](../../../supersymmetry.md#supergravity-auxiliary-field) is not. In the convention $F^z=-e^{\kappa^2K/2}\overline{D_zW}$, its [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) obeys

$$
|F^z|=\sqrt3\,|\mu|m_p e^{a_0^2/2}\ne0.
$$

The matter [fermion](../../../quantum-mechanics.md#fermion) transformation contains a term proportional to $F^z\epsilon$, so no nonzero constant [supersymmetry](../../../supersymmetry.md) parameter leaves this vacuum invariant. Hence **supersymmetry is spontaneously broken even though the vacuum energy vanishes**: the positive [auxiliary field](../../../supersymmetry.md#auxiliary-field) contribution cancels the negative gravitational term. The matter [fermion](../../../quantum-mechanics.md#fermion) supplies the [goldstino](../../../supersymmetry.md#goldstino), which is absorbed by the [gravitino](../../../supersymmetry.md#gravitino) in the [super-Higgs mechanism](../../../supersymmetry.md#super-higgs-mechanism).

Using the [gravitino mass from a superpotential](../../../supersymmetry.md#gravitino-mass-from-a-superpotential), and $z_0+\beta=m_p$, gives

$$
\boxed{m_{3/2}=\kappa^2 e^{\kappa^2K/2}|W|
=|\mu|e^{2-\sqrt3}
=\frac{|F^z|}{\sqrt3m_p}.}
$$

An [auxiliary field](../../../supersymmetry.md#auxiliary-field) $F^z$ has [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) two. Defining the [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) scale by $\Lambda_{\mathrm{SUSY}}=\sqrt{|F^z|}$, one obtains

$$
\frac{m_{3/2}}{\Lambda_{\mathrm{SUSY}}}
=\frac{\Lambda_{\mathrm{SUSY}}}{\sqrt3m_p}.
$$

Thus the [gravitino](../../../supersymmetry.md#gravitino) [mass](../../../classical-mechanics.md#mass) is small compared with the [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) scale when that scale is sub-Planckian, as in the usual hierarchy $|\mu|\ll m_p$. This smallness is gravitational suppression; it is not a conclusion valid for arbitrary choices of the mass parameter.

## 4

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use the scalar components of the three [chiral superfields](../../../supersymmetry.md#chiral-superfield), and set $a=|\phi_0|^2$, $b=|\phi_+|^2$, $c=|\phi_-|^2$ and $\Sigma=a+b+c$. We assume the physical sign $g>0$ and a nonzero coupling $\lambda$. The coefficient $g$ below is exactly the coefficient in the supplied [D-term scalar potential](../../../supersymmetry.md#d-term-scalar-potential); it should not be silently replaced by a differently normalized squared [gauge coupling](../../../relativistic-quantum-field.md#gauge-coupling). The canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) has identity [Kähler metric](../../../complex-geometry.md#kahler-metric), and the three [Kähler covariant derivatives of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) are

$$
\begin{aligned}
D_0W&=\lambda\phi_+\phi_-(1+\kappa^2a),\\
D_+W&=\lambda\phi_0\phi_-(1+\kappa^2b),\\
D_-W&=\lambda\phi_0\phi_+(1+\kappa^2c).
\end{aligned}
$$

Substitution in the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential) gives

$$
\begin{aligned}
V_F={}&|\lambda|^2e^{\kappa^2\Sigma}
\left[bc(1+\kappa^2a)^2+ac(1+\kappa^2b)^2
+ab(1+\kappa^2c)^2-3\kappa^2abc\right]\\
={}&|\lambda|^2e^{\kappa^2\Sigma}
\left[ab+ac+bc+3\kappa^2abc+\kappa^4abc\Sigma\right].
\end{aligned}
$$

In particular, the subtraction cancels only half of the six $\kappa^2abc$ terms contributed by the three squares. The full [scalar potential](../../../quantum-field-theory.md#scalar-potential) is

$$
\boxed{V=|\lambda|^2e^{\kappa^2\Sigma}
\left[ab+ac+bc+3\kappa^2abc+\kappa^4abc\Sigma\right]
+g(b-c-\zeta)^2\ge0.}
$$

Its nonnegativity follows term by term from $a,b,c\ge0$ and $g>0$. This is a special property of this cubic [superpotential](../../../supersymmetry.md#superpotential), not of a general [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential).

The [D-term vacuum branches of a cubic superpotential](../../../supersymmetry.md#d-term-vacuum-branches-of-a-cubic-superpotential) must be described as branches: there are not two isolated field-space minima. First suppose $\zeta>0$. Vanishing of $V_F$ requires $ab=ac=bc=0$, and vanishing of the [D-term scalar potential](../../../supersymmetry.md#d-term-scalar-potential) requires $b-c=\zeta$. Together these conditions give the [vacuum expectation values](../../../quantum-field-theory.md#vacuum-expectation-value)

$$
\boxed{\langle\phi_0\rangle=\langle\phi_-\rangle=0,
\qquad |\langle\phi_+\rangle|=\sqrt\zeta,
\qquad V=0.}
$$

The phase of $\phi_+$ lies on a [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit), and one may choose it positive and real. At this [global minimum](../../../analysis.md#global-minimum), all $D_iW$ and the real [auxiliary field](../../../supersymmetry.md#auxiliary-field) of the [vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet) vanish. It is a [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum), even though the internal [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) is spontaneously broken. For $\zeta<0$, interchange $\phi_+$ and $\phi_-$: the nonzero [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) has magnitude $\sqrt{-\zeta}$. For $\zeta=0$, the [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) is the entire family $\phi_+=\phi_-=0$, with $\phi_0$ arbitrary.

The other branch has $\phi_+=\phi_-=0$ and arbitrary $\phi_0$. Here $W=D_iW=0$ but the real [auxiliary field](../../../supersymmetry.md#auxiliary-field) is nonzero for $\zeta\ne0$, and

$$
V=g\zeta^2.
$$

Thus this branch has pure [D-term](../../../supersymmetry.md#d-term) [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) and a [flat direction of a scalar potential](../../../quantum-field-theory.md#flat-direction-of-a-scalar-potential) in the neutral scalar. It is not stable at every neutral-field value. At a fixed $a=|\phi_0|^2$, expansion in the charged scalars yields

$$
V=g\zeta^2
+\left(|\lambda|^2ae^{\kappa^2a}-2g\zeta\right)|\phi_+|^2
+\left(|\lambda|^2ae^{\kappa^2a}+2g\zeta\right)|\phi_-|^2
+O\left((b+c)^2\right).
$$

Hence the two charged squared [masses](../../../classical-mechanics.md#mass) and the stability condition are

$$
\boxed{m_\pm^2=|\lambda|^2ae^{\kappa^2a}\mp2g\zeta,
\qquad |\lambda|^2ae^{\kappa^2a}>2g|\zeta|.}
$$

Above this threshold, both charged directions have positive [mass](../../../classical-mechanics.md#mass) squared. Continuity makes them uniformly positive in a sufficiently small neighborhood of the chosen neutral-field value, so the stationary branch is a genuine, non-strict [local minimum](../../../analysis.md#local-minimum) valley. Its neutral direction stays flat. Below the threshold, a charged [mass](../../../classical-mechanics.md#mass) squared is negative and the branch is a [saddle point](../../../analysis.md#saddle-point). At equality it is a boundary of the stable valley, not a [local minimum](../../../analysis.md#local-minimum) in the full field space: changing $a$ slightly downward and switching on the unstable charged field lowers $V$. For example, for $\zeta>0$, put $a=a_c-\epsilon$, $b=\epsilon^2$, $c=0$. Since $M(a)=|\lambda|^2ae^{\kappa^2a}$ has $M'(a_c)>0$, one finds $V-g\zeta^2=-M'(a_c)\epsilon^3+O(\epsilon^4)<0$.

There are no further local-minimum branches under these generic assumptions. If $b+c>0$, the expression for $V_F$ is strictly increasing in $a$, so a stationary configuration with a charged condensate must have $a=0$. At $a=0$, an interior critical point with $b,c>0$ is impossible, because

$$
\partial_b V+\partial_c V
=|\lambda|^2e^{\kappa^2(b+c)}
\left(b+c+2\kappa^2bc\right)>0.
$$

On the boundary $c=0$, the relevant [scalar potential](../../../quantum-field-theory.md#scalar-potential) is $g(b-\zeta)^2$; on $b=0$ it is $g(c+\zeta)^2$. Their nonnegative-domain minima give exactly the [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) described above, or the origin of the charged-field branch. Thus, for nonzero $\zeta$, **the two types are the zero-energy supersymmetric gauge orbit and the positive-energy D-breaking minimum valley above the threshold**. If $\zeta=0$, the two types coalesce into the flat [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum); the literal two-minimum assertion needs this parameter qualification.

In the global [supersymmetry](../../../supersymmetry.md) limit $\kappa\to0$, the [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential) becomes $|\lambda|^2(ab+ac+bc)$ and the [D-term scalar potential](../../../supersymmetry.md#d-term-scalar-potential) retains its form. The same two types of branches occur, with the threshold $|\lambda|^2a>2g|\zeta|$. [Supergravity](../../../supersymmetry.md#supergravity) instead introduces the exponential and additional positive terms. The [goldstino](../../../supersymmetry.md#goldstino) of global [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) is a physical [fermion](../../../quantum-mechanics.md#fermion); in local [supersymmetry](../../../supersymmetry.md) it participates in the [super-Higgs mechanism](../../../supersymmetry.md#super-higgs-mechanism). A positive vacuum energy also gravitates in [supergravity](../../../supersymmetry.md#supergravity). In particular, the positive-energy branch here has $W=0$ and hence vanishing [gravitino mass from a superpotential](../../../supersymmetry.md#gravitino-mass-from-a-superpotential); it is not the tuned zero-energy broken vacuum of Question 3.

There is a further gauge-consistency qualification. In conventional two-derivative matter-coupled [supergravity](../../../supersymmetry.md#supergravity), a constant [Fayet–Iliopoulos term](../../../supersymmetry.md#fayet-iliopoulos-term) gauges an [R-symmetry](../../../supersymmetry.md#r-symmetry) and requires a corresponding nontrivial transformation of the [superpotential](../../../supersymmetry.md#superpotential). The apparent charges $0,+1,-1$ make the supplied cubic [superpotential](../../../supersymmetry.md#superpotential) neutral, so a nonzero independent constant $\zeta$ does not by itself specify a consistent conventional [supergravity](../../../supersymmetry.md#supergravity) action. The computed branches are those of the supplied [scalar potential](../../../quantum-field-theory.md#scalar-potential); a full embedding needs compatible charges or additional fields. This restriction is explained in [Van Proeyen's derivation of the superpotential gauge-covariance condition](https://arxiv.org/abs/hep-th/0410053).

More generally, the [supergravity moment-map constraint on D-term breaking](../../../supersymmetry.md#supergravity-moment-map-constraint-on-d-term-breaking) follows directly from gauge covariance. If $k^i\partial_iW=-\kappa^2rW$ and the [moment map](../../../symplectic-geometry.md#moment-map) is $\mathcal P=i(k^iK_i-r)$, then at a point with $W\ne0$,

$$
\mathcal P=i\kappa^{-2}\frac{k^iD_iW}{W}.
$$

Consequently all chiral [auxiliary fields](../../../supersymmetry.md#auxiliary-field) vanishing implies the [D-term](../../../supersymmetry.md#d-term) also vanishes there. This relation has no analogue forcing that implication in an arbitrary global [supersymmetry](../../../supersymmetry.md) model. Its $W\ne0$ hypothesis matters: the formal D-breaking branch above has $W=0$, so it does not contradict the identity. These conventional gauge-completion restrictions are additional to the elementary minimization calculation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
