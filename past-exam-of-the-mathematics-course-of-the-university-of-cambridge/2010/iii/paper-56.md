# Paper 56

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper56.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper56.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use mostly-plus Lorentzian signature and $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$, with antisymmetrized gamma products of unit weight. A [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) obeys a reality condition under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation):

$$
\boxed{\psi^c=C\overline\psi^{\,T}=\psi,\qquad C\gamma^\mu C^{-1}=-(\gamma^\mu)^T.}
$$

A [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) instead has definite [chirality](../../../relativistic-quantum-field.md#chirality-physics),

$$
\boxed{P_\pm\psi=\psi,\qquad P_\pm=\tfrac12(1\pm\gamma_5).}
$$

A four-dimensional [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) has four real components, while a [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) has two complex components. [Charge conjugation](../../../quantum-field-theory.md#charge-conjugation) reverses [chirality](../../../relativistic-quantum-field.md#chirality-physics) in this signature, so a nonzero spinor cannot satisfy both conditions simultaneously.

For the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) $(\not\partial+m)\psi=0$, the derivative term reverses [chirality](../../../relativistic-quantum-field.md#chirality-physics) because $\gamma_5$ anticommutes with every [gamma matrix](../../../algebra.md#gamma-matrices), whereas the [mass](../../../classical-mechanics.md#mass) term preserves it. Projecting a purely chiral spinor equation onto its two chiralities therefore gives both $\not\partial\psi=0$ and $m\psi=0$. Thus **a nonzero four-component [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) satisfying this uncoupled [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) must be massless**. A [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) contains conjugate opposite-chirality components and can have a nonzero [mass](../../../classical-mechanics.md#mass). Its charge-conjugation reality condition identifies particle and antiparticle operators, so **a Majorana particle is its own antiparticle**. A Weyl field does not by itself impose that identification.

This does not forbid writing a [Majorana mass term](../../../relativistic-quantum-field.md#majorana-mass-term) for a neutral two-component Weyl field: such a term couples the field to its conjugate, and the resulting four-component massive field is Majorana, not a purely chiral solution of the uncoupled [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation).

For the [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field), set $\chi=\gamma^\mu\psi_\mu$ and $d=\partial^\mu\psi_\mu$. The antisymmetric kinetic operator is invariant under

$$
\delta\psi_\mu=\partial_\mu\eta,
$$

because commuting derivatives contract to zero against $\gamma^{\mu\nu\rho}$. Expanding its gamma product gives

$$
E^\mu=\gamma^{\mu\nu\rho}\partial_\nu\psi_\rho
=\not\partial\psi^\mu-\partial^\mu\chi+\gamma^\mu(\not\partial\chi-d).
$$

Gamma contraction gives $\gamma_\mu E^\mu=2(\not\partial\chi-d)$, so the equation implies $d=\not\partial\chi$ and $\not\partial\psi^\mu=\partial^\mu\chi$.

For a [Fourier mode](../../../fourier-analysis.md#fourier-mode) with [momentum](../../../classical-mechanics.md#momentum) $k$, if $k^2\ne0$ the latter identity gives $k^2\psi^\mu=k^\mu\not k\chi$. The mode is proportional to $k^\mu$ and hence pure gauge. Every physical nonzero-momentum mode therefore has **$k^2=0$**. For a null mode, choose an index with $k^\mu\ne0$. The same equation makes $\chi$ an element of the image of $\not k$, allowing a gauge choice with $\chi=0$. The field equations then reduce to

$$
\boxed{\gamma\cdot\psi=0,\qquad\partial\cdot\psi=0,\qquad\not\partial\psi_\mu=0.}
$$

Residual [gauge transformations](../../../electromagnetism.md#gauge-transformation) obey $\not\partial\eta=0$.

Take a null [momentum](../../../classical-mechanics.md#momentum) in the third spatial direction. Residual gauge freedom and transversality remove the temporal and longitudinal [vector](../../../vector-space.md#vector) components, leaving two transverse [vector](../../../vector-space.md#vector) polarizations. Their helicities are $\pm1$, while on-shell spinor helicities are $\pm1/2$. The gamma-trace constraint removes the two combinations of total [helicity](../../../special-relativity.md#helicity) $\pm1/2$ and retains the aligned combinations of [helicity](../../../special-relativity.md#helicity) $\pm3/2$. Explicitly, in a [chiral representation](../../../algebra.md#chiral-gamma-matrix-representation) the transverse gamma contractions use $\sigma_1\pm i\sigma_2$, which annihilate the correspondingly aligned [spin](../../../quantum-mechanics.md#spin) states and act nontrivially on the opposite states. Thus a Majorana [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field) has **two physical massless polarizations**. The Majorana assumption is the one relevant to simple [supergravity](../../../supersymmetry.md#supergravity); a complex vector-spinor has these helicities for its particle and independent antiparticle modes.

A consistent free massive deformation is the algebraic term

$$
\mathcal L_m=\frac m2\overline\psi_\mu\gamma^{\mu\nu}\psi_\nu
$$

added to a kinetic term $-\tfrac12\overline\psi_\mu\gamma^{\mu\nu\rho}\partial_\nu\psi_\rho$. Its equation is

$$
\gamma^{\mu\nu\rho}\partial_\nu\psi_\rho-m\gamma^{\mu\rho}\psi_\rho=0.
$$

For $m\ne0$, divergence and gamma contraction give, respectively,

$$
\gamma^{\mu\rho}\partial_\mu\psi_\rho=0,\qquad
2\gamma^{\nu\rho}\partial_\nu\psi_\rho-3m\gamma^\rho\psi_\rho=0.
$$

These imply the [massive Rarita-Schwinger constraints](../../../relativistic-quantum-field.md#massive-rarita-schwinger-constraints) $\chi=0$ and $d=0$, and the remaining equation is $(\not\partial+m)\psi_\mu=0$. Squaring gives $(\Box-m^2)\psi_\mu=0$ in the chosen signature. The [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) is lost. In the rest frame, transversality sets the temporal component to zero; three spatial [vector](../../../vector-space.md#vector) components times two on-shell spinor states give six states, and gamma trace removes the two spin-one-half states. The result is **four massive spin-$3/2$ states**, with [spin](../../../quantum-mechanics.md#spin) projections $\pm3/2,\pm1/2$. In [supergravity](../../../supersymmetry.md#supergravity) the additional longitudinal states can be supplied by the [super-Higgs mechanism](../../../supersymmetry.md#super-higgs-mechanism).

## 2

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Choose the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) convention

$$
[\nabla_\mu,\nabla_\nu]\psi=\frac14R_{\mu\nu ab}\gamma^{ab}\psi,\qquad
\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu},
$$

with positive [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) for a round sphere. The connection preserves the gamma matrices. If $D=\gamma^\mu\nabla_\mu$, its square is

$$
D^2\psi=\nabla^2\psi+\frac12\gamma^{\mu\nu}[\nabla_\mu,\nabla_\nu]\psi
=\nabla^2\psi+\frac18\gamma^{\mu\nu}R_{\mu\nu ab}\gamma^{ab}\psi.
$$

Here $\nabla^2$ is the [rough Laplacian](../../../fiber-bundle.md#rough-laplacian), including the connection on the derivative index. In the product of two antisymmetric gamma pairs, the fully antisymmetric four-gamma term vanishes by the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity). The two-gamma contractions vanish because the [Ricci tensor](../../../general-relativity.md#ricci-tensor) is symmetric, while the scalar contractions give $-2R$. Thus the [Lichnerowicz spinor-square formula](../../../relativistic-quantum-field.md#lichnerowicz-spinor-square-formula) is

$$
\boxed{D^2=\nabla^2-\frac R4.}
$$

Multiplying $(D+m)\psi=0$ by $-D+m$, with constant $m$, proves

$$
\boxed{-\nabla^2\psi+\frac R4\psi+m^2\psi=0.}
$$

In Riemannian signature $D$ in this positive-Clifford convention is formally [anti-self-adjoint](../../../functional-analysis.md#skew-adjoint-generator); the more usual [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) Dirac operator $iD$ has square $-\nabla^2+R/4$. Stating this convention avoids an apparent sign conflict between the two forms of the formula.

Now let $D\psi=0$ on the compact Riemannian [spin manifold](../../../riemannian-geometry.md#spin-manifold). Use the positive-definite spinor [inner product](../../../linear-algebra.md#inner-product) and integrate the squared equation. [Integration by parts](../../../calculus.md#integration-by-parts) has no boundary contribution, giving

$$
0=\int_M\left(\langle\psi,-\nabla^2\psi\rangle+\frac R4|\psi|^2\right)dV
=\int_M\left(|\nabla\psi|^2+\frac R4|\psi|^2\right)dV.
$$

Both terms are nonnegative. Smoothness then forces $\nabla\psi=0$ pointwise. Consequently **every harmonic spinor is parallel**, and $R|\psi|^2=0$. A nonzero parallel spinor has constant positive norm on its connected component, so its [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) vanishes there. This is [compact harmonic-spinor rigidity under nonnegative scalar curvature](../../../relativistic-quantum-field.md#compact-harmonic-spinor-rigidity-under-nonnegative-scalar-curvature).

The full Ricci conclusion follows from integrability, not merely from vanishing [scalar curvature](../../../second-fundamental-form.md#scalar-curvature). Since a parallel spinor has zero curvature for its [spin connection](../../../connection-1-form.md#spin-connection), contract its [Ricci identity](../../../general-relativity.md#curvature-commutator-on-a-covariant-tensor) with $\gamma^\nu$:

$$
0=\gamma^\nu[\nabla_\mu,\nabla_\nu]\psi
=\frac14R_{\mu\nu ab}\gamma^\nu\gamma^{ab}\psi
=-\frac12R_{\mu\nu}\gamma^\nu\psi.
$$

The three-gamma term vanishes by the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity); the remaining contractions give the displayed Ricci term. For each fixed $\mu$, put $v_\nu=R_{\mu\nu}$. [Clifford multiplication](../../../algebra.md#clifford-multiplication) twice gives

$$
0=(v_\nu\gamma^\nu)^2\psi=|v|^2\psi.
$$

Positive definiteness and $\psi\ne0$ imply $v=0$. Thus the [Riemannian parallel-spinor Ricci-flatness](../../../relativistic-quantum-field.md#riemannian-parallel-spinor-ricci-flatness) result is

$$
\boxed{R_{\mu\nu}=0.}
$$

On a connected manifold a nontrivial parallel solution is nowhere zero, so this holds everywhere. On a disconnected manifold it holds on every component supporting a nonzero spinor; the stated nowhere-vanishing hypothesis ensures all components are covered. The positive-definite [metric tensor](../../../general-relativity.md#metric-tensor) is essential to the last inference.

## 3

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the mostly-plus [Clifford algebra](../../../algebra.md#clifford-algebra) and [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) conventions of the preceding solutions, with $e=\det(e_\mu{}^a)$, $\kappa^2=8\pi G$, and a Majorana [gravitino](../../../supersymmetry.md#gravitino). An [action](../../../classical-mechanics.md#action) for [minimal four-dimensional supergravity](../../../supersymmetry.md#minimal-four-dimensional-supergravity) in the exact transformation normalization given is

$$
\boxed{S_0=\int d^4x\,e\left[\frac{R}{2\kappa^2}-2\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho\right]+O(\psi^4).}
$$

The kinetic coefficient is tied to the normalization of the [supersymmetry](../../../supersymmetry.md) transformations: if $\Psi_\mu=2\psi_\mu$ and $\eta=2\epsilon$, this becomes the canonical coefficient $-1/2$, with $\delta e_\mu{}^a=(\kappa/2)\bar\eta\gamma^a\Psi_\mu$ and $\delta\Psi_\mu=\nabla_\mu\eta/\kappa$. Mixing those two normalizations would spoil the cancellation.

To the retained order, use the torsion-free connection. More generally the [1.5-order formalism](../../../general-relativity.md#1-5-order-formalism) allows its variation to be omitted after imposing its own algebraic equation; the resulting contorsion is quadratic in [fermions](../../../quantum-mechanics.md#fermion) and first affects the displayed [action](../../../classical-mechanics.md#action) at quartic order. The [metric tensor](../../../general-relativity.md#metric-tensor) variation induced by the [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) is $\delta g_{\mu\nu}=4\kappa\bar\epsilon\gamma_{(\mu}\psi_{\nu)}$, so the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) varies as

$$
\delta S_{\rm EH}=-\frac2\kappa\int e\,G^{\mu\nu}\bar\epsilon\gamma_\mu\psi_\nu+\text{boundary}.
$$

For the fermionic [action](../../../classical-mechanics.md#action), varying both Majorana factors gives the same contribution after [integration by parts](../../../calculus.md#integration-by-parts) and the Grassmann bilinear interchange rule. Thus

$$
\delta S_{\rm RS}=-\frac4\kappa\int e\,(\nabla_\mu\bar\epsilon)\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho
=\frac4\kappa\int e\,\bar\epsilon\gamma^{\mu\nu\rho}\nabla_\mu\nabla_\nu\psi_\rho+\text{boundary}.
$$

The vector-index [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) contribution vanishes by the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity). The spin-index contribution is determined by

$$
\gamma^{\rho\mu\nu}\nabla_\mu\nabla_\nu\zeta
=\frac18\gamma^{\rho\mu\nu}R_{\mu\nu ab}\gamma^{ab}\zeta
=\frac12G^{\rho\sigma}\gamma_\sigma\zeta.
$$

For the last equality, expand the antisymmetric three-gamma/two-gamma product: the totally antisymmetric [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) terms vanish by Bianchi, and the surviving terms are the Ricci contraction minus half its trace. Hence

$$
\delta S_{\rm RS}=\frac2\kappa\int e\,G^{\mu\nu}\bar\epsilon\gamma_\mu\psi_\nu+\text{boundary},
$$

which cancels the gravitational variation. Variations of [vierbeins](../../../general-relativity.md#orthonormal-coframe-in-spacetime), gamma matrices and the connection in the fermionic kinetic term carry three dynamical [fermions](../../../quantum-mechanics.md#fermion). They lie beyond this linear-fermion cancellation and are cancelled by the omitted four-fermion completion. Thus the [action](../../../classical-mechanics.md#action) is invariant up to boundary terms at the order specified, rather than claiming that a truncated [action](../../../classical-mechanics.md#action) is exactly invariant at every [fermion](../../../quantum-mechanics.md#fermion) order.

For the cosmological extension, add a [gravitino](../../../supersymmetry.md#gravitino) [mass](../../../classical-mechanics.md#mass) parameter $m$ and deform the derivative:

$$
\boxed{S_m=\int e\left[\frac{R+6m^2}{2\kappa^2}-2\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho
+2m\bar\psi_\mu\gamma^{\mu\nu}\psi_\nu\right],\quad
\delta\psi_\mu=\frac1\kappa\mathcal D_\mu\epsilon,\quad
\mathcal D_\mu=\nabla_\mu+\frac m2\gamma_\mu.}
$$

Indeed the [fermion](../../../quantum-mechanics.md#fermion) terms combine as $-2\bar\psi_\mu\gamma^{\mu\nu\rho}\mathcal D_\nu\psi_\rho$ because $\gamma^{\mu\nu\rho}\gamma_\nu=-2\gamma^{\mu\rho}$. The modified spinor connection curvature is

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

This is the [Anti-de Sitter deformation of minimal supergravity](../../../supersymmetry.md#anti-de-sitter-deformation-of-minimal-supergravity). A cosmological term alone would leave its variation uncancelled; the [mass](../../../classical-mechanics.md#mass) term and the gamma shift of the [gravitino](../../../supersymmetry.md#gravitino) transformation are both necessary. A positive [cosmological constant](../../../cosmology.md#cosmological-constant) cannot arise from this real unbroken minimal deformation.

For electromagnetism, retain $\mathcal N=1$ and introduce an Abelian [vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet) $(A_\mu,\lambda)$, with Majorana [gaugino](../../../supersymmetry.md#gaugino) $\lambda$. A complete quadratic-fermion extension is

$$
\boxed{\mathcal L_{\rm vec}=e\left[-\frac14F_{\mu\nu}F^{\mu\nu}-\frac12\bar\lambda\gamma^\mu\nabla_\mu\lambda
-\frac\kappa2\bar\psi_\mu\gamma^{\nu\rho}\gamma^\mu\lambda\,F_{\nu\rho}\right],\qquad F=dA.}
$$

The accompanying leading transformations are

$$
\boxed{\delta A_\mu=\bar\epsilon\gamma_\mu\lambda,\qquad
\delta\lambda=-\frac12\gamma^{\mu\nu}F_{\mu\nu}\epsilon.}
$$

They preserve the rigid Maxwell-gaugino [action](../../../classical-mechanics.md#action) for constant $\epsilon$. For a local parameter, the variation contains

$$
\delta\mathcal L_{\rm rigid}=e(\nabla_\mu\bar\epsilon)j^\mu+\text{boundary},\qquad
j^\mu=\frac12F_{ab}\gamma^{ab}\gamma^\mu\lambda.
$$

To obtain this, vary $F^2$, vary both [gaugino](../../../supersymmetry.md#gaugino) factors, and use $\gamma^{ab}\gamma^\mu=\gamma^{ab\mu}+g^{b\mu}\gamma^a-g^{a\mu}\gamma^b$. The terms with $\nabla\lambda$ cancel between the two [actions](../../../classical-mechanics.md#action); integrating the three-gamma term uses $\nabla_{[\mu}F_{\nu\rho]}=0$, leaving exactly the displayed derivative of the parameter. The interaction is $-\kappa e\bar\psi_\mu j^\mu$, whose variation under $\delta\bar\psi_\mu=\nabla_\mu\bar\epsilon/\kappa$ cancels that term.

The other linear-fermion variation is also fixed. Put $\mathcal F=F_{ab}\gamma^{ab}$ and $T_{\rm EM}^{\mu\nu}=F^{\mu\rho}F^\nu{}_{\rho}-g^{\mu\nu}F^2/4$. [Clifford multiplication](../../../algebra.md#clifford-multiplication) gives

$$
\mathcal F\gamma^\mu\mathcal F=8T_{\rm EM}^{\mu\nu}\gamma_\nu.
$$

Varying $\lambda$ in the gravitino-current interaction then gives $2\kappa e T_{\rm EM}^{\mu\nu}\bar\psi_\mu\gamma_\nu\epsilon=-2\kappa eT_{\rm EM}^{\mu\nu}\bar\epsilon\gamma_\nu\psi_\mu$, which cancels the Maxwell [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) variation. This proves the required [supergravity coupling of an Abelian vector multiplet](../../../supersymmetry.md#supergravity-coupling-of-an-abelian-vector-multiplet) through the retained order.

Beyond that order one uses a supercovariant [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength), here $\widehat F_{\mu\nu}=F_{\mu\nu}-2\kappa\bar\psi_{[\mu}\gamma_{\nu]}\lambda$, and the associated higher-fermion transformation terms and four-fermion interactions. An auxiliary scalar may be retained for off-shell closure, or eliminated in this on-shell formulation. A [Maxwell field](../../../electromagnetism.md#electromagnetic-field) without a fermionic partner cannot be coupled by merely adding $-F^2/4$ while leaving all transformations unchanged. An alternative is an $\mathcal N=2$ gravity multiplet, where the [vector](../../../vector-space.md#vector) is a graviphoton and a second [gravitino](../../../supersymmetry.md#gravitino) supplies its extra fermionic states; the explicit construction above is the minimal $\mathcal N=1$ matter extension.

## 4

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Killing spinor](../../../supersymmetry.md#killing-spinor) is a nonzero spinor parameter for which the fermionic [supersymmetry](../../../supersymmetry.md) variations vanish on a bosonic background. In [minimal four-dimensional supergravity](../../../supersymmetry.md#minimal-four-dimensional-supergravity) without a cosmological term this means

$$
\boxed{\nabla_\mu\epsilon=0.}
$$

It is an overdetermined equation and expresses an unbroken [supersymmetry](../../../supersymmetry.md) of the background. In the cosmological deformation the corresponding equation is $\mathcal D_\mu\epsilon=0$; in theories with additional bosonic fields their contributions also enter the [fermion](../../../quantum-mechanics.md#fermion) variations.

For the undeformed theory the connection preserves both the spinor adjoint and gamma matrices. Consequently the [Dirac current](../../../quantum-field-theory.md#dirac-current)

$$
K^\mu=\bar\epsilon\gamma^\mu\epsilon
$$

obeys $\nabla_\nu K_\mu=0$. In particular $\nabla_{(\nu}K_{\mu)}=0$, so **$K$ is a [Killing vector](../../../general-relativity.md#killing-vector-field)**, and in fact is parallel. For the real cosmological deformation, $\nabla_\mu\epsilon=-(m/2)\gamma_\mu\epsilon$ and $\nabla_\mu\bar\epsilon=(m/2)\bar\epsilon\gamma_\mu$ instead give $\nabla_\mu K_\nu=(m/2)\bar\epsilon[\gamma_\mu,\gamma_\nu]\epsilon$, whose symmetric part again vanishes.

The causal property uses an ordinary commuting spinor. Take an orthonormal frame with $(\gamma^0)^\dagger=-\gamma^0$, $(\gamma^i)^\dagger=\gamma^i$, and $\bar\epsilon=\epsilon^\dagger\gamma^0$. Then $K^0=-\epsilon^\dagger\epsilon$. Reverse its time orientation and write $V=-K$, so

$$
V^0=\epsilon^\dagger\epsilon,\qquad V^i=\epsilon^\dagger\alpha^i\epsilon,\qquad\alpha^i=-\gamma^0\gamma^i.
$$

The matrices $\alpha^i$ are Hermitian and obey $\{\alpha^i,\alpha^j\}=2\delta^{ij}$. For every spatial [unit vector](../../../vector-space.md#unit-vector) $u$, $(u_i\alpha^i)^2=1$, whence $|u_iV^i|\le V^0$. Choose $u$ along the spatial part of $V$ to obtain

$$
\boxed{K_\mu K^\mu=V_\mu V^\mu=-(V^0)^2+|\mathbf V|^2\le0.}
$$

A nonzero [Killing spinor](../../../supersymmetry.md#killing-spinor) cannot vanish at an isolated point: its defining connection equation transports its value along every curve. Thus on a connected background this is a nonzero, nowhere-spacelike [causal Dirac spinor current](../../../quantum-field-theory.md#causal-dirac-spinor-current). The estimate does not need the Majorana condition, but it does need commuting components; Grassmann bilinears have no such ordinary positivity order.

For the [positive energy theorem](../../../general-relativity.md#positive-energy-theorem), take a complete asymptotically flat spacelike hypersurface with a [spin structure](../../../riemannian-geometry.md#spin-structure) $\Sigma$, with suitable decay, Einstein constraint equations, and matter satisfying the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition). Assume there are no inner boundaries, or that any inner-boundary contribution has the required nonnegative sign. The auxiliary commuting spinor approaches an arbitrary constant $\epsilon_\infty$ at spatial infinity. Define the real [Nester two-form](../../../general-relativity.md#nester-two-form)

$$
B^{\mu\nu}=\bar\epsilon\gamma^{\mu\nu\rho}\nabla_\rho\epsilon-\overline{\nabla_\rho\epsilon}\gamma^{\mu\nu\rho}\epsilon.
$$

Antisymmetry removes second derivatives except through the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor). Differentiation and the three-gamma [spinor curvature identity](../../../connection-1-form.md#spinor-curvature-identity) used above give

$$
\nabla_\nu B^{\mu\nu}=2(\nabla_\nu\bar\epsilon)\gamma^{\mu\nu\rho}\nabla_\rho\epsilon+G^{\mu\nu}K_\nu.
$$

The first term comes from differentiating the two spinor factors. For the second term, replace $\nabla_\nu\nabla_\rho$ by half their [commutator](../../../lie-algebra.md#commutator); its spin-curvature contraction is $G^{\mu\nu}\gamma_\nu/2$ from each conjugate term. This is the reason the [Einstein tensor](../../../general-relativity.md#einstein-tensor), and hence the matter energy density, enters the boundary-charge identity.

In an orthonormal frame adapted to the future normal of $\Sigma$, put $\chi_i=\nabla_i\epsilon$. Since $\gamma^0\gamma^{0ij}=-\gamma^{ij}$,

$$
2(\nabla_i\bar\epsilon)\gamma^{0ij}\nabla_j\epsilon=2\left(\sum_i|\chi_i|^2-\left|\sum_i\gamma^i\chi_i\right|^2\right).
$$

Here $\nabla_i$ is the spacetime [spin connection](../../../connection-1-form.md#spin-connection) pulled back to $\Sigma$, including its [extrinsic curvature](../../../differential-geometry.md#extrinsic-curvature). Choose the auxiliary spinor to solve the elliptic [Witten spinor equation](../../../general-relativity.md#witten-spinor-equation)

$$
\gamma^i\nabla_i\epsilon=0,\qquad\epsilon\longrightarrow\epsilon_\infty.
$$

The standard asymptotic-flatness and completeness hypotheses permit this boundary-value problem; the positivity identity also excludes a decaying homogeneous zero mode. It is this hypersurface equation that removes the negative square. A spacetime [Killing spinor](../../../supersymmetry.md#killing-spinor) is not assumed for a general initial-data set.

Stokes' theorem and $G_{\mu\nu}=\kappa^2T_{\mu\nu}$ now give

$$
Q[\epsilon_\infty]=\frac1{\kappa^2}\int_{S_\infty}B^{0i}dS_i
=\frac2{\kappa^2}\int_\Sigma|\nabla_i\epsilon|^2dV+\int_\Sigma T_{\mu\nu}n^\mu V^\nu dV\ge0.
$$

The [dominant energy condition](../../../general-relativity.md#dominant-energy-condition) makes the second integrand nonnegative because $n$ and $V$ are future causal. Evaluating the two-form with the asymptotic [spin connection](../../../connection-1-form.md#spin-connection) identifies its surface integral with the [ADM energy](../../../general-relativity.md#arnowitt-deser-misner-energy) and [momentum](../../../classical-mechanics.md#momentum):

$$
Q[\epsilon_\infty]=-P_\mu V_\infty^\mu
=\epsilon_\infty^\dagger\bigl(E\,1-P_i\alpha^i\bigr)\epsilon_\infty.
$$

For example its energy term uses $B^{0i}=\tfrac12(\partial_jh_{ij}-\partial_ih_{jj})|\epsilon_\infty|^2$ to first order in the asymptotic spatial [metric tensor](../../../general-relativity.md#metric-tensor) perturbation. With $\kappa^2=8\pi G$ this is exactly the ADM normalization. Since $P_i\alpha^i$ has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\pm|\mathbf P|$, positivity for every boundary spinor proves

$$
\boxed{E\ge|\mathbf P|\ge0.}
$$

[Killing spinors](../../../supersymmetry.md#killing-spinor) describe saturation: their spatial derivative term vanishes, and the contracted matter term must also vanish for the corresponding charge to be zero. They characterize preserved [supersymmetry](../../../supersymmetry.md) rather than being prerequisites for positivity. Under the usual rigidity hypotheses, zero total four-momentum makes the nonnegative integral vanish for a full basis of asymptotic spinors; their parallel extensions force a vanishing [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) and give the Minkowski vacuum. A single [Killing spinor](../../../supersymmetry.md#killing-spinor) with null current alone does not justify asserting that every component of the total [momentum](../../../classical-mechanics.md#momentum) vanishes.

## 5

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The gravitational variable and the fields held fixed in a variation must be specified. For bosonic matter a second-order [metric tensor](../../../general-relativity.md#metric-tensor) formulation is sufficient. For spinorial matter a [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) and a [spin connection](../../../connection-1-form.md#spin-connection) are needed to define the local Lorentz representation and its [covariant derivative](../../../general-relativity.md#covariant-derivative). “Second order” refers to a connection already expressed through derivatives of the [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime); “first order” treats that connection as an independent variable.

For a [metric tensor](../../../general-relativity.md#metric-tensor), a [scalar field](../../../quantum-field-theory.md#scalar-field) and an Abelian [gauge field](../../../relativistic-quantum-field.md#gauge-field), consider the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) with matter,

$$
S=\int d^4x\,e\left[\frac{R-2\Lambda}{2\kappa^2}-\frac12g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi-V(\phi)-\frac14F_{\mu\nu}F^{\mu\nu}\right],\qquad F=dA.
$$

Here $e=\sqrt{-g}$ and the connection in $R$ is Levi-Civita. The [metric tensor](../../../general-relativity.md#metric-tensor) variation uses $\delta e=-eg_{\mu\nu}\delta g^{\mu\nu}/2$ and

$$
\delta R=R_{\mu\nu}\delta g^{\mu\nu}+g^{\mu\nu}\delta R_{\mu\nu},\qquad
\delta R_{\mu\nu}=\nabla_\rho\delta\Gamma^\rho{}_{\mu\nu}-\nabla_\nu\delta\Gamma^\rho{}_{\mu\rho}.
$$

[Metric compatibility](../../../fiber-bundle.md#metric-compatibility) makes the last two terms a divergence. Thus

$$
\delta S=\frac12\int e\left[\kappa^{-2}(G_{\mu\nu}+\Lambda g_{\mu\nu})-T_{\mu\nu}\right]\delta g^{\mu\nu}+\text{matter variations}+\text{boundary},\qquad
T_{\mu\nu}=-\frac2e\frac{\delta S_{\rm matter}}{\delta g^{\mu\nu}}.
$$

Stationarity for arbitrary compactly supported variations gives

$$
\boxed{G_{\mu\nu}+\Lambda g_{\mu\nu}=\kappa^2T_{\mu\nu}.}
$$

Explicitly,

$$
T^{\phi}_{\mu\nu}=\partial_\mu\phi\partial_\nu\phi-g_{\mu\nu}\left[\frac12(\partial\phi)^2+V\right],\qquad
T^{A}_{\mu\nu}=F_{\mu\rho}F_\nu{}^\rho-\frac14g_{\mu\nu}F^2.
$$

[Scalar field](../../../quantum-field-theory.md#scalar-field) and gauge-potential variations give $\nabla^2\phi-V'=0$ and $\nabla_\mu F^{\mu\nu}=0$. Their equations imply [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation), consistently with the contracted [Bianchi identity](../../../fiber-bundle.md#bianchi-identity). If the boundary [metric tensor](../../../general-relativity.md#metric-tensor) is fixed instead of using compactly supported variations, add the [Gibbons–Hawking–York boundary term](../../../general-relativity.md#gibbons-hawking-york-boundary-term), $\kappa^{-2}\int_{\partial M}\varepsilon_{\partial M}\sqrt{|h|}K$, with the outward-normal orientation. Fixing the [metric tensor](../../../general-relativity.md#metric-tensor) alone does not otherwise remove the normal derivatives of its variation.

For spinorial matter, write $g_{\mu\nu}=e_\mu{}^ae_\nu{}^b\eta_{ab}$ and $\nabla_\mu\chi=\partial_\mu\chi+\omega_{\mu ab}\gamma^{ab}\chi/4$. In the second-order theory set $\omega=\omega(e)$ before varying. A symmetrized Dirac [action](../../../classical-mechanics.md#action), in the same no-$i$, mostly-plus convention as the earlier solutions, is

$$
S_\chi=\int e\left[-\frac12\left(\bar\chi\gamma^\mu\nabla_\mu\chi-(\nabla_\mu\bar\chi)\gamma^\mu\chi\right)-m\bar\chi\chi\right].
$$

Varying $\bar\chi$ and integrating by parts gives $(\not\nabla+m)\chi=0$; varying $\chi$ gives the adjoint equation. The spinor components held fixed in a gravitational variation are components in the [Lorentz frame](../../../general-relativity.md#lorentz-frame). Both $\gamma^\mu=e_a{}^\mu\gamma^a$ and $\omega(e)$ vary with the [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime). The former gives the canonical stress, and integrating the spin-connection variation supplies its spin-current improvement. On the [Dirac equations](../../../relativistic-quantum-field.md#dirac-equation) the resulting symmetric stress [tensor](../../../linear-algebra.md#tensor) is

$$
T^\chi_{\mu\nu}=\frac14\left[\bar\chi\gamma_\mu\overleftrightarrow\nabla_\nu\chi+\bar\chi\gamma_\nu\overleftrightarrow\nabla_\mu\chi\right],\qquad
\bar\chi\gamma_\mu\overleftrightarrow\nabla_\nu\chi=\bar\chi\gamma_\mu\nabla_\nu\chi-(\nabla_\nu\bar\chi)\gamma_\mu\chi.
$$

The off-shell expression also contains $g_{\mu\nu}\mathcal L_\chi/e$; this vanishes on the matter equations for the displayed symmetrized [action](../../../classical-mechanics.md#action). Treating the coordinate gamma matrices as fixed while varying the [metric tensor](../../../general-relativity.md#metric-tensor) would miss the displayed stress. Local Lorentz invariance removes the independent antisymmetric [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) equation, leaving the symmetric [Einstein field equations](../../../general-relativity.md#einstein-field-equations) with this matter source.

In a first-order [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) formulation, $e^a$ and an antisymmetric Lorentz connection $\omega^{ab}$ are independent. Define

$$
T^a=de^a+\omega^a{}_b\wedge e^b,\qquad R^{ab}=d\omega^{ab}+\omega^a{}_c\wedge\omega^{cb},
$$

and use $R(e,\omega)=e_a{}^\mu e_b{}^\nu R_{\mu\nu}{}^{ab}$. The [curvature form of a connection](../../../fiber-bundle.md#curvature-form) variation is $\delta R^{ab}=D_\omega\delta\omega^{ab}$. For the Einstein-Hilbert term, [integration by parts](../../../calculus.md#integration-by-parts) in form notation gives a connection equation proportional to

$$
\varepsilon_{abcd}\,T^c\wedge e^d=0
$$

when matter has no connection dependence. For an invertible [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) this forces $T^a=0$, so $\omega=\omega(e)$. The [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) equation then becomes the second-order [Einstein field equations](../../../general-relativity.md#einstein-field-equations). This applies to the scalar and Maxwell examples: use $F=dA$, which is independent of $\omega$ and remains gauge invariant even if torsion is present.

A [Dirac field](../../../relativistic-quantum-field.md#dirac-field) changes the connection equation. Directly varying its two [covariant derivatives](../../../general-relativity.md#covariant-derivative) gives

$$
\delta_\omega\mathcal L_\chi=-\frac e8\bar\chi\{\gamma^\mu,\gamma^{ab}\}\chi\,\delta\omega_{\mu ab}
=-\frac e4\bar\chi\gamma^{\mu ab}\chi\,\delta\omega_{\mu ab}.
$$

Thus its [spin](../../../quantum-mechanics.md#spin) density sources totally antisymmetric torsion. This is [Einstein-Cartan theory](../../../general-relativity.md#einstein-cartan-theory), and the connection equation is algebraic rather than a propagation equation for an extra field. To see both its solution and its effect, write

$$
\omega_{\mu ab}=\omega(e)_{\mu ab}+K_{\mu ab},\qquad K_{abc}=e_a{}^\mu K_{\mu bc},\qquad B^{abc}=\bar\chi\gamma^{abc}\chi.
$$

For the totally antisymmetric component sourced by this field, the [Ricci scalar](../../../general-relativity.md#ricci-scalar) is $R(e,\omega)=R(e)-K_{abc}K^{abc}$ up to a divergence. The other irreducible contorsion components have no spinor source and their connection equations set them to zero. The auxiliary part of the [Lagrangian](../../../calculus-of-variations.md#lagrangian) is therefore

$$
\mathcal L_K=-\frac e{2\kappa^2}K_{abc}K^{abc}-\frac e4K_{abc}B^{abc}.
$$

Its algebraic variation gives the [algebraic torsion of a Dirac field](../../../general-relativity.md#algebraic-torsion-of-a-dirac-field),

$$
\boxed{K_{abc}=-\frac{\kappa^2}{4}B_{abc},\qquad T_{abc}=-2K_{abc}=\frac{\kappa^2}{2}B_{abc}.}
$$

Here the first index of $K_{abc}$ labels the derivative, and the torsion convention is $T_{abc}=K_{bac}-K_{cab}$; specifying this convention fixes the sign. Eliminating $K$ leaves the second-order effective [action](../../../classical-mechanics.md#action) with contact interaction

$$
\boxed{\mathcal L_{\rm contact}=\frac{e\kappa^2}{32}(\bar\chi\gamma^{abc}\chi)(\bar\chi\gamma_{abc}\chi).}
$$

It is a local axial-current four-fermion interaction. Hence first-order gravity with Dirac [spin](../../../quantum-mechanics.md#spin) density is equivalent to torsion-free second-order gravity with this additional interaction. It is not equivalent to simply declaring the [spin connection](../../../connection-1-form.md#spin-connection) torsion-free and dropping the contact term. In the effective formulation the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) have the stress [tensor](../../../linear-algebra.md#tensor) of the full effective matter [action](../../../classical-mechanics.md#action). Before eliminating the connection, the antisymmetric stress and its [spin](../../../quantum-mechanics.md#spin) current are related by the local Lorentz Noether identity.

Finally, the [1.5-order formalism](../../../general-relativity.md#1-5-order-formalism) is a convenient way to vary this effective [action](../../../classical-mechanics.md#action). Let $\widehat\omega(e,\chi)$ solve the algebraic connection equation and let $S_2(e,\chi)=S_1(e,\widehat\omega(e,\chi),\chi)$. The chain rule gives

$$
\delta S_2=\left.\frac{\delta S_1}{\delta e}\right|_{\widehat\omega}\delta e+\left.\frac{\delta S_1}{\delta\chi}\right|_{\widehat\omega}\delta\chi+\left.\frac{\delta S_1}{\delta\bar\chi}\right|_{\widehat\omega}\delta\bar\chi+\underbrace{\left.\frac{\delta S_1}{\delta\omega}\right|_{\widehat\omega}}_{0}\delta\widehat\omega.
$$

Thus **vary as in first order, then insert the solved connection**. One does not need to calculate the complicated induced connection variation. This procedure is justified by its connection equation, not by discarding that variation arbitrarily. In [supergravity](../../../supersymmetry.md#supergravity) the [gravitino](../../../supersymmetry.md#gravitino) sources a contorsion quadratic in [fermions](../../../quantum-mechanics.md#fermion); substituting it generates the four-fermion terms, while the 1.5-order method simplifies the local [supersymmetry](../../../supersymmetry.md) cancellation through the lower orders considered above.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
