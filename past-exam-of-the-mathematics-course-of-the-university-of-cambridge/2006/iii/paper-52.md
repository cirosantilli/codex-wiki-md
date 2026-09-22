# Paper 52

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper52.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper52.pdf)

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

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use natural units and the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$. A massive spin-one particle has three physical [particle polarizations](../../../special-relativity.md#particle-polarization), whereas a massless [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) has two. Giving a vector a mass must account for this extra longitudinal state while preserving a positive physical state space, controlled high-energy scattering and, if a fundamental perturbative theory is sought, [renormalizability](../../../perturbative-quantum-field-theory.md#renormalizable-quantum-field-theory).

At the free-field level there is no inconsistency. The [Proca action](../../../electromagnetism.md#proca-action)

$$
\mathcal L=-\frac14F_{\mu\nu}F^{\mu\nu}+\frac12m^2A_\mu A^\mu,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu
$$

gives the [Proca equation](../../../electromagnetism.md#proca-equation) $\partial_\nu F^{\nu\mu}+m^2A^\mu=0$. Taking its divergence gives $m^2\partial_\mu A^\mu=0$, and then $(\Box+m^2)A^\mu=0$. For $m>0$ the divergence constraint removes one of the four components, leaving three positive-norm physical modes. The time component is constrained, rather than an independent negative-norm propagating oscillator. The mass term does, however, change under $A_\mu\mapsto A_\mu+\partial_\mu\omega$, so the ordinary massless [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) is no longer manifest.

The difficulty becomes acute for generic interactions. Inverting the quadratic operator gives the [Proca propagator](../../../electromagnetism.md#proca-propagator)

$$
D_{\mu\nu}(k)=\frac{-i}{k^2-m^2+i0}\left(g_{\mu\nu}-\frac{k_\mu k_\nu}{m^2}\right).
$$

The longitudinal part approaches order $1/m^2$ at large momentum, rather than falling as $1/k^2$. Thus the usual ultraviolet [power counting](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory) deteriorates. There is a parallel external-state problem: for $p^\mu=(E,\mathbf p)$,

$$
\varepsilon_L^\mu(p)=\frac1m(|\mathbf p|,E\widehat{\mathbf p})=\frac{p^\mu}{m}+O(m/E).
$$

Longitudinal external legs can generate powers of $E/m$ in a [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude). These are the [high-energy obstruction for a hard vector mass](../../../electromagnetism.md#high-energy-obstruction-for-a-hard-vector-mass). Conserved Abelian currents can remove dangerous contractions, so one should not conclude that every massive-vector interaction is impossible.

For a massive non-Abelian vector with gauge-like cubic and quartic couplings, cancellations among diagrams remove the largest powers, but without a suitable additional sector longitudinal scattering still grows like $s/v^2$, where $v$ is the symmetry-breaking scale. A partial-wave coefficient is then of order $s/(16\pi v^2)$. [Partial-wave unitarity](../../../quantum-mechanics.md#partial-wave-unitarity) requires its real part to remain bounded, so perturbation theory fails at energies of order the electroweak scale times a modest loop factor, around the TeV scale for electroweak vectors. This is a limit on the perturbative description, not a proof that a low-energy massive-vector [effective field theory](../../../quantum-field-theory.md#effective-field-theory) is inconsistent.

The [Higgs mechanism](../../../standard-model.md#higgs-mechanism) supplies a weakly coupled completion. For an Abelian example, take a [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field) with

$$
\mathcal L=-\frac14F^2+|D_\mu\phi|^2-\lambda(|\phi|^2-v^2/2)^2,\qquad D_\mu=\partial_\mu-igA_\mu.
$$

Locally write $\phi=(v+h)e^{i\chi/v}/\sqrt2$. Its [gauge-covariant kinetic term](../../../quantum-field-theory.md#gauge-covariant-kinetic-term) becomes

$$
|D_\mu\phi|^2=\frac12(\partial_\mu h)^2+\frac12(v+h)^2(\partial_\mu\chi/v-gA_\mu)^2.
$$

The combination is invariant under $A_\mu\mapsto A_\mu+\partial_\mu\omega$, $\chi\mapsto\chi+gv\omega$. In [unitary gauge](../../../standard-model.md#unitary-gauge) $\chi=0$, it contains $m^2A_\mu A^\mu/2$ with $m=gv$, as well as the correlated $hAA$ and $hhAA$ interactions. The two original gauge polarizations and two real scalar components become three massive-vector polarizations and one radial [Higgs boson](../../../standard-model.md#higgs-boson). The would-be [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson) supplies the longitudinal state. This counting explains why the [Goldstone theorem](../../../quantum-field-theory.md#goldstone-theorem) for spontaneously broken global symmetries does not imply an extra physical massless particle here. Local [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) is a redundancy; choosing a Higgs background after [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) does not explicitly break the gauge invariance of the action.

The extra scalar interactions also repair high-energy scattering. By the [Goldstone-boson equivalence theorem](../../../standard-model.md#goldstone-boson-equivalence-theorem), the leading longitudinal-vector amplitude can be computed using the would-be [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson). For a charged-to-neutral channel in the linear scalar model, the scalar contact and radial-exchange terms give

$$
\mathcal M=-\frac{m_H^2}{v^2}-\frac{m_H^4}{v^2(s-m_H^2)}
=\frac{s}{v^2}-\frac{s^2}{v^2(s-m_H^2)}\longrightarrow-\frac{m_H^2}{v^2}.
$$

This [Higgs cancellation in longitudinal vector scattering](../../../standard-model.md#higgs-cancellation-in-longitudinal-vector-scattering) removes the uncontrolled $s/v^2$ growth. It also shows why a very large scalar self-coupling would itself make perturbation theory unreliable; introducing a scalar is not a license to ignore [partial-wave unitarity](../../../quantum-mechanics.md#partial-wave-unitarity).

Although the [unitary gauge](../../../standard-model.md#unitary-gauge) propagator looks like the badly behaved [Proca propagator](../../../electromagnetism.md#proca-propagator), renormalizability is conveniently established in an [R-xi gauge](../../../relativistic-quantum-field.md#r-xi-gauge). Using Cartesian scalar fluctuations, the quadratic mixing is $-mA_\mu\partial^\mu\chi$. The gauge-fixing term $-(\partial\cdot A+\xi m\chi)^2/(2\xi)$ cancels it and gives

$$
D_{\mu\nu}^{(\xi)}(k)=\frac{-i}{k^2-m^2+i0}\left[g_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2-\xi m^2+i0}\right].
$$

At fixed finite $\xi$ this falls as $1/k^2$. The would-be scalar modes and [Faddeev-Popov ghosts](../../../relativistic-quantum-field.md#faddeev-popov-ghost) remain in intermediate calculations. Gauge identities, organized through [BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry), make unphysical states cancel from physical amplitudes and constrain counterterms to the gauge-invariant renormalizable form. With a renormalizable scalar sector and cancellation of [gauge anomalies](../../../relativistic-quantum-field.md#gauge-anomaly), spontaneously broken gauge theory is renormalizable and unitary on its physical states; the bosonic construction is demonstrated in the [original massive Yang-Mills renormalizability proof](https://www.staff.science.uu.nl/~hooft101/gthpub/massive.pdf). The ultraviolet limit and $\xi\to\infty$ limit do not commute, so the unitary-gauge numerator alone is not a valid disproof of this result.

In the [Standard Model](../../../standard-model.md), a [Higgs doublet](../../../standard-model.md#higgs-field) breaks the manifest electroweak group from $SU(2)_L\times U(1)_Y$ to $U(1)_{\rm em}$. The scalar kinetic term yields

$$
\boxed{M_W=gv/2,\qquad M_Z=\frac v2\sqrt{g^2+g'^2},\qquad M_\gamma=0.}
$$

Three scalar directions supply the longitudinal polarizations of $W^\pm$ and $Z$, while the unbroken electromagnetic generator leaves the [photon](../../../quantum-mechanics.md#photon) massless. The radial [Higgs boson](../../../standard-model.md#higgs-boson) remains physical.

There is an important Abelian alternative. The [Stueckelberg mechanism](../../../relativistic-quantum-field.md#stueckelberg-mechanism) introduces a scalar with $\mathcal L_{\rm mass}=(mA_\mu-\partial_\mu\chi)^2/2$, invariant under $A\mapsto A+\partial\omega$, $\chi\mapsto\chi+m\omega$. With suitable conserved-current couplings this can describe a renormalizable massive Abelian gauge theory without a radial Higgs particle. A naive non-Abelian analogue involves a nonlinear group-valued scalar and derivative interactions suppressed by inverse powers of the symmetry-breaking scale; it is generally an [effective field theory](../../../quantum-field-theory.md#effective-field-theory), not a power-counting-renormalizable substitute. Strongly coupled or composite sectors can provide other completions. **A free vector mass is consistent; the central problem is obtaining the longitudinal state and its interactions in a theory with controlled ultraviolet behavior and physical unitarity.**

## 2

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A useful model of [spontaneous breaking of a Z2 scalar symmetry](../../../quantum-field-theory.md#spontaneous-breaking-of-a-z2-scalar-symmetry) is the four-dimensional real scalar theory

$$
\mathcal L=\frac12(\partial\phi)^2-\frac\lambda4(\phi^2-v^2)^2,\qquad\lambda>0,quad v>0.
$$

The action is invariant under the [Z2 symmetry](../../../quantum-field-theory.md#z2-symmetry) $\phi\mapsto-\phi$. Its classical [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) consists of the two values $\phi=\pm v$. In the broken quantum phase, choose a pure vacuum with $\langle\phi\rangle=v$; the symmetry maps it to a different vacuum with opposite expectation value, although it leaves the action unchanged. To distinguish quantum symmetry breaking from simply minimizing a classical potential, introduce a small source $J\phi$ and take the infinite-volume limit before $J\to0^+$. A finite-volume symmetry-preserving ground state can remain an even superposition because of tunneling, whereas the selected infinite-volume pure vacua have nonzero [vacuum expectation values](../../../quantum-field-theory.md#vacuum-expectation-value). The parameter $v$ below is the tree-level expectation, with its quantum value determined by renormalized parameters.

Writing $\phi=v+h$ gives

$$
V=\lambda v^2h^2+\lambda vh^3+\frac\lambda4h^4,\qquad
\boxed{m_h^2=2\lambda v^2.}
$$

The original sign symmetry relates expansions about the two vacua; in one expansion it acts as $h\mapsto-2v-h$. It is not a symmetry that fixes the chosen vacuum. Since the broken group is discrete, there is no continuous broken generator and no required [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson).

With relativistically normalized external states, the general two-body partial [decay width](../../../relativistic-quantum-field.md#decay-width) is

$$
\boxed{\Gamma_{1\to2}=\frac1{2m}\frac1{\mathcal S}\int d\Phi_2\,\overline{|\mathcal M|^2},\qquad
d\Phi_2=(2\pi)^4\delta^{(4)}(P-p_1-p_2)\prod_{i=1}^2\frac{d^3p_i}{(2\pi)^3,2E_i}.}
$$

Here the bar sums final spins and averages initial spins only if the initial ensemble is unpolarized. The [identical final-state symmetry factor](../../../quantum-mechanics.md#identical-particle-factor-in-a-final-state-phase-space-integral) is $\mathcal S=2!$ for two identical daughters and one for distinguishable daughters. Integrating the three-momentum delta function in the parent rest frame leaves $\mathbf p_2=-\mathbf p_1$. The energy delta function fixes $k=|\mathbf p_1|$ and has radial Jacobian $k(1/E_1+1/E_2)$. Hence the [two-body decay phase space](../../../quantum-mechanics.md#two-body-decay-phase-space) is

$$
d\Phi_2=\frac{k}{16\pi^2m}d\Omega,\qquad
k=\frac{\sqrt{[m^2-(m_1+m_2)^2][m^2-(m_1-m_2)^2]}}{2m}.
$$

Consequently

$$
\frac{d\Gamma}{d\Omega}=\frac{k}{32\pi^2m^2\mathcal S}\overline{|\mathcal M|^2},\qquad
\Gamma=\frac{k}{8\pi m^2\mathcal S}\overline{|\mathcal M|^2}
$$

when the spin-summed amplitude is angle independent.

For [Higgs decay to two W bosons](../../../standard-model.md#higgs-decay-to-two-w-bosons), the scalar parent has no spin average and the amplitude, up to an irrelevant phase, is $\mathcal M=gM_W\varepsilon_1^*\cdot\varepsilon_2^*$. Use the [massive vector polarization sum](../../../relativistic-quantum-field.md#polarization-sum-for-a-massive-vector-boson) with $p_i^2=M_W^2$:

$$
\begin{aligned}
\sum_{\lambda_1,\lambda_2}|\mathcal M|^2
&=g^2M_W^2\left(-g_{\mu\nu}+\frac{p_{1\mu}p_{1\nu}}{M_W^2}\right)
\left(-g^{\mu\nu}+\frac{p_2^\mu p_2^\nu}{M_W^2}\right)\\
&=g^2M_W^2\left[4-1-1+\frac{(p_1\cdot p_2)^2}{M_W^4}\right].
\end{aligned}
$$

Momentum conservation gives $p_1\cdot p_2=(M_H^2-2M_W^2)/2$. With the PDF's ratio $x=M_W/M_H$, this becomes

$$
\sum|\mathcal M|^2=\frac{g^2M_H^4}{4M_W^2}(1-4x^2+12x^4),\qquad
k=\frac{M_H}{2}\sqrt{1-4x^2}.
$$

The charged daughters are distinguishable. Combining the last two equations with $g^2/M_W^2=4\sqrt2G_F$ gives

$$
\boxed{\Gamma(H\to W^+W^-)=\frac{G_FM_H^3}{8\pi\sqrt2}\sqrt{1-4x^2}\,(1-4x^2+12x^4).}
$$

For [Higgs decay to two Z bosons](../../../standard-model.md#higgs-decay-to-two-z-bosons), the [Higgs boson coupling to Z bosons](../../../standard-model.md#higgs-boson-coupling-to-z-bosons) is $2iM_Z^2g_{\mu\nu}/v=igM_Z^2g_{\mu\nu}/M_W$, using $v=2M_W/g$. This compensates the changed powers of $M_Z$ in the polarization contraction, giving the same normalization of the squared amplitude with $x$ replaced by $y=M_Z/M_H$. The two [Z bosons](../../../standard-model.md#z-boson) are identical, so the phase-space symmetry factor supplies an additional half:

$$
\boxed{\Gamma(H\to ZZ)=\frac{G_FM_H^3}{16\pi\sqrt2}\sqrt{1-4y^2}\,(1-4y^2+12y^4).}
$$

Both expressions have mass dimension one, vanish at their two-body thresholds and approach the ratio $2:1$ for $M_H\gg M_Z$. The cubic large-mass behavior comes from longitudinal-vector polarizations. These are on-shell tree-level widths under the stated heavy-Higgs hypothesis; below threshold the physical off-shell multi-particle decays require a different calculation.

## 3

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $\bar\psi=\psi^\dagger\gamma^0$, the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $(+---)$ and $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$. Distinguish the numerical [charge-conjugation matrix](../../../quantum-field-theory.md#charge-conjugation-matrix) $C$ from the unitary operator $\widehat C$ acting on fields. The [adjoint Dirac equation](../../../relativistic-quantum-field.md#adjoint-dirac-equation) is $i(\partial_\mu\bar\psi)\gamma^\mu+m\bar\psi=0$. Transpose it and multiply by $C$; the identity $C\gamma^{\mu T}=-\gamma^\mu C$ gives

$$
iC\gamma^{\mu T}\partial_\mu\bar\psi^T+mC\bar\psi^T=0
\quad\Longrightarrow\quad
\boxed{(i\gamma^\mu\partial_\mu-m)\psi^c=0,\qquad\psi^c=C\bar\psi^T.}
$$

Thus the charge-conjugate field satisfies the same free [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation).

To compute its [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint), use $C^\dagger=C^{-1}$ and Hermitian $\gamma^0$ with $(\gamma^0)^2=1$. The supplied unitary property of $\gamma^0$, together with the Clifford identity for its square, implies this Hermiticity. Since $\gamma^{0T}C^{-1}=-C^{-1}\gamma^0$,

$$
\overline{\psi^c}=\psi^T(\gamma^0)^*C^{-1}\gamma^0
=\psi^T\gamma^{0T}C^{-1}\gamma^0=-\psi^TC^{-1}.
$$

Therefore [charge conjugation of the Dirac adjoint](../../../quantum-field-theory.md#charge-conjugation-of-the-dirac-adjoint) gives

$$
\boxed{\widehat C\bar\psi(x)\widehat C^{-1}=-\eta_C^*\psi(x)^TC^{-1}.}
$$

The intrinsic phase obeys $|\eta_C|=1$. Antisymmetry of $C$ also gives $(\psi^c)^c=-C(C^{-1})^T\psi=\psi$.

[Charge conjugation](../../../quantum-field-theory.md#charge-conjugation) exchanges electron and positron modes while preserving momentum and the spin label in a compatible spin basis. Write the [mode expansion of a Dirac field](../../../relativistic-quantum-field.md#mode-expansion-of-a-dirac-field) as

$$
\psi(x)=\sum_s\int d\Pi_p\,[a(p,s)u(p,s)e^{-ip\cdot x}+b^\dagger(p,s)v(p,s)e^{ip\cdot x}].
$$

Its charge conjugate is

$$
\psi^c(x)=\sum_s\int d\Pi_p\,[b(p,s)C\bar v(p,s)^Te^{-ip\cdot x}+a^\dagger(p,s)C\bar u(p,s)^Te^{ip\cdot x}].
$$

Choose the [charge-conjugate particle and antiparticle spinors](../../../quantum-field-theory.md#charge-conjugate-particle-and-antiparticle-spinors) so that

$$
\boxed{v(p,s)=C\bar u(p,s)^T,\qquad u(p,s)=C\bar v(p,s)^T.}
$$

This is legitimate: transposing $\bar u(\not p-m)=0$ shows $(\not p+m)C\bar u^T=0$, and the involution above supplies the inverse relation. Comparing the two independent frequency coefficients in $\widehat C\psi\widehat C^{-1}=\eta_C\psi^c$ then gives

$$
\boxed{\widehat Ca\widehat C^{-1}=\eta_Cb,\qquad
\widehat Cb\widehat C^{-1}=\eta_C^*a,\qquad
\widehat Ca^\dagger\widehat C^{-1}=\eta_C^*b^\dagger,\qquad
\widehat Cb^\dagger\widehat C^{-1}=\eta_Ca^\dagger.}
$$

Different conventional spinor phases can move the phases between these relations, but the exchange of particles and antiparticles is invariant.

For local [fermion bilinears](../../../relativistic-quantum-field.md#fermion-bilinear), understand the products as [normal-ordered](../../../perturbative-quantum-field-theory.md#normal-ordering) or equivalently use a consistent renormalized composite-operator prescription. The transformed product is initially $-\psi^TC^{-1}\Gamma C\bar\psi^T$. Reordering the fermions gives a second minus sign, hence

$$
\widehat C:\bar\psi\Gamma\psi:\widehat C^{-1}
=:\bar\psi(C^{-1}\Gamma C)^T\psi:.
$$

For $\Gamma=\gamma^\mu$, the transposed matrix is $-\gamma^\mu$, so the [vector current](../../../relativistic-quantum-field.md#vector-current) is C-odd:

$$
\boxed{\widehat Cj^\mu(x)\widehat C^{-1}=-j^\mu(x).}
$$

The [quantum electrodynamics](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics) interaction $-ej_\mu A^\mu$ is C-invariant when the [photon](../../../quantum-mechanics.md#photon) field is also odd, $\widehat CA^\mu\widehat C^{-1}=-A^\mu$. Its field strength is then odd and its quadratic kinetic term even.

For the [chirality matrix](../../../algebra.md#chirality-matrix), there is no complex conjugation of the numerical $i$ by this unitary field operation. Thus

$$
\begin{aligned}
C^{-1}\gamma^5C
&=i(-\gamma^{0T})(-\gamma^{1T})(-\gamma^{2T})(-\gamma^{3T})\\
&=i\gamma^{0T}\gamma^{1T}\gamma^{2T}\gamma^{3T}
=i\gamma^{3T}\gamma^{2T}\gamma^{1T}\gamma^{0T}=\gamma^{5T}.
\end{aligned}
$$

The reversal takes six swaps of mutually anticommuting [gamma matrices](../../../algebra.md#gamma-matrices), giving a positive sign. Therefore

$$
(C^{-1}\gamma^\mu\gamma^5C)^T=-\gamma^5\gamma^\mu=\gamma^\mu\gamma^5,
\qquad\boxed{\widehat Cj_5^\mu\widehat C^{-1}=+j_5^\mu.}
$$

The [axial current](../../../relativistic-quantum-field.md#axial-current) is C-even. Hence a photon-like interaction containing both currents transforms as

$$
\widehat C:(j_\mu-j_{5\mu})A^\mu\longmapsto(j_\mu+j_{5\mu})A^\mu.
$$

It is **not C-invariant when the axial part is present**; C symmetry of ordinary electromagnetic vector coupling does not extend to this chiral combination.

For [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory), taking the adjoint of the field transformation gives $\bar\psi(x)\mapsto\eta_P^*\bar\psi(x_P)\gamma^0$. The phases cancel in bilinears, and $\gamma^0\gamma^\mu\gamma^0=P^\mu{}_{\nu}\gamma^\nu$, with $P=\operatorname{diag}(1,-1,-1,-1)$. Since $\gamma^5$ anticommutes with $\gamma^0$,

$$
\boxed{j^\mu(x)\mapsto P^\mu{}_{\nu}j^\nu(x_P),\qquad
j_5^\mu(x)\mapsto-P^\mu{}_{\nu}j_5^\nu(x_P).}
$$

In components, the vector's time component is even and spatial components are odd; the axial time component is odd and its spatial components are even.

Combining the C and P transformations, both currents acquire the same overall minus sign:

$$
j^\mu(x)\xrightarrow{CP}-P^\mu{}_{\nu}j^\nu(x_P),\qquad
j_5^\mu(x)\xrightarrow{CP}-P^\mu{}_{\nu}j_5^\nu(x_P).
$$

Let the real vector transform as $V^\mu(x)\xrightarrow{CP}\xi P^\mu{}_{\nu}V^\nu(x_P)$, with $\xi=\pm1$. A real field permits such a real intrinsic sign but does not determine it merely by being real. The Lorentz contraction then gives the [CP invariance of a neutral chiral vector interaction](../../../quantum-field-theory.md#cp-invariance-of-a-neutral-chiral-vector-interaction) criterion:

$$
\boxed{(j_\mu-j_{5\mu})V^\mu(x)\xrightarrow{CP}-\xi[(j_\mu-j_{5\mu})V^\mu](x_P).}
$$

It is invariant for $\xi=-1$. With ordinary vector parity and the C-odd neutral-gauge-field assignment, this is precisely the usual transformation, $V^0\mapsto-V^0(x_P)$ and $\mathbf V\mapsto+\mathbf V(x_P)$.

The diagonal [Z boson](../../../standard-model.md#z-boson) couplings have the form $Z_\mu\bar f\gamma^\mu(g_V^f-g_A^f\gamma^5)f$ with real coefficients. The same calculation applies to any real vector and axial coefficients. Thus **the tree-level flavour-diagonal neutral-current Z interaction preserves CP although it violates C and P separately when both current structures occur**. This statement is about the neutral-current interaction, not a claim that the entire [Standard Model](../../../standard-model.md) preserves CP: complex charged-current [CKM matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) phases provide [CP violation](../../../quantum-field-theory.md#cp-violation).

## 4

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A renormalized coupling is specified by a [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition) at an auxiliary momentum scale $\mu$. Loop corrections contain logarithms of momentum ratios; changing that scale changes the part called the coupling and the part left in the explicit loop correction. The bare theory and exact physical amplitudes do not change. This is the meaning of a [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling), rather than an actual dependence of a physical observable on an arbitrary prescription.

For the dimensionless gauge coupling relevant here, the one-loop vertex and wave-function corrections shift $g$ at order $g^3$. For example a regulated relation has the schematic form

$$
g_{\rm bare}=g(\mu)+a g(\mu)^3\ln(\Lambda_{\rm UV}^2/\mu^2)+\cdots.
$$

Differentiating at fixed bare parameters gives $dg/d\ln\mu^2=ag^3+O(g^5)$, or $\mu\,dg/d\mu=cg^3+O(g^5)$ with $c=2a$. The [gauge-coupling beta function in logarithmic squared scale](../../../perturbative-quantum-field-theory.md#gauge-coupling-beta-function-in-logarithmic-squared-scale) follows by the chain rule:

$$
\frac{d\alpha}{d\ln\mu^2}
=\frac{g}{2\pi}\frac{dg}{d\ln\mu^2}
=\frac{cg^4}{4\pi}+O(g^6)
=\boxed{b_0\alpha^2+O(\alpha^3),\qquad b_0=4\pi c\in\mathbb R.}
$$

Here $\alpha=g^2/(4\pi)$. The reality of the coefficient reflects the real renormalization of a real gauge coupling. The leading cubic power for $g$ is a gauge-coupling statement, not a universal rule for every type of coupling in every quantum field theory.

At one loop, separate variables or differentiate the inverse coupling:

$$
\frac{d(\alpha^{-1})}{d\ln\mu^2}=-b_0,
\qquad
\boxed{\alpha(\mu^2)=\frac{\alpha_0}{1-b_0\alpha_0\ln(\mu^2/\mu_0^2)}.}
$$

When $b_0=-\beta_0<0$, define the [strong-coupling scale](../../../perturbative-quantum-field-theory.md#strong-coupling-scale) by

$$
\boxed{\ln\Lambda^2=\ln\mu_0^2-\frac{\alpha_0^{-1}}{\beta_0},\qquad
\Lambda=\mu_0e^{-1/(2\beta_0\alpha_0)}.}
$$

Logarithms of dimensionful scales here use the same fixed units; the equivalent ratio equation $\ln(\mu_0^2/\Lambda^2)=1/(\beta_0\alpha_0)$ is dimensionless. The [one-loop running of the strong coupling](../../../perturbative-quantum-field-theory.md#one-loop-running-of-the-strong-coupling) is therefore

$$
\boxed{\alpha(\mu^2)=\frac1{\beta_0\ln(\mu^2/\Lambda^2)},\qquad\mu>\Lambda.}
$$

This trades a dimensionless reference coupling for a dimensionful integration constant, an example of [dimensional transmutation](../../../perturbative-quantum-field-theory.md#dimensional-transmutation).

As $\mu^2\to\infty$, the coupling decreases logarithmically to zero: [asymptotic freedom](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) makes short-distance strong-interaction processes perturbatively accessible. As $\mu$ decreases toward $\Lambda$ from above, the coupling grows, and omitted higher orders become important before the formal pole. These are the [infrared limitations of one-loop QCD running](../../../perturbative-quantum-field-theory.md#infrared-limitations-of-one-loop-qcd-running). The pole is not a trustworthy prediction of an infinite physical interaction, and continuation below $\Lambda$ to negative $\alpha$ is invalid. Low-energy [QCD](../../../standard-model.md#quantum-chromodynamics) instead needs nonperturbative descriptions of [confinement](../../../standard-model.md#confinement), hadrons and related dynamics; the one-loop pole alone does not prove confinement. This interpretation and the dependence of $\Lambda$ on the running prescription are explained in the [QCD review, section 9.1.1](https://pdg.lbl.gov/2024/reviews/rpp2024-rev-qcd.pdf).

Physically the QCD scale is of hadronic order, conventionally a few hundred MeV rather than an electroweak mass. However, $\beta_0=O(1)$ alone cannot determine any absolute mass: $\mu_0$ and $\alpha_0$ or an empirical reference are also necessary. The exponential relation shows how a much smaller scale can arise; for illustrative inputs $\mu_0=100\,\mathrm{GeV}$, $\alpha_0=0.12$ and $\beta_0=0.6$, it gives $\Lambda\simeq0.096\,\mathrm{GeV}$. Different flavour counts, schemes and perturbative orders change the numerical value, so this is an order-of-magnitude illustration, not a parameter-free prediction.

In the [Standard Model](../../../standard-model.md), $N=3$ and the six [quark flavours](../../../standard-model.md#quark-flavor) are $u,d,s,c,b,t$. Above all six thresholds the supplied coefficient gives

$$
\boxed{\beta_0^{(6)}=\frac{33-12}{12\pi}=\frac7{4\pi}\simeq0.557.}
$$

The count is six Dirac flavours, not eighteen colour states or twelve Weyl fields. In lower-energy effective theories the active flavour count changes: near the bottom threshold $\beta_0^{(5)}=23/(12\pi)$ and $\beta_0^{(4)}=25/(12\pi)$; below charm the three-flavour value is $9/(4\pi)$.

For [matching the QCD scale across a quark threshold](../../../perturbative-quantum-field-theory.md#matching-the-qcd-scale-across-a-quark-threshold), impose the leading-order continuity at $\mu=m_b$:

$$
\frac1{\beta_0^{(5)}\ln(m_b^2/\Lambda_5^2)}
=\frac1{\beta_0^{(4)}\ln(m_b^2/\Lambda_4^2)}.
$$

Thus $\ln(m_b/\Lambda_5)=(25/23)\ln(m_b/\Lambda_4)$, and exponentiation gives

$$
\boxed{\Lambda_5=m_b\left(\frac{\Lambda_4}{m_b}\right)^{25/23}
=\Lambda_4\left(\frac{m_b}{\Lambda_4}\right)^{-2/23}.}
$$

The five- and four-flavour expressions apply on the respective sides near this threshold, before the next heavy-flavour threshold is crossed. The matched coupling is continuous at the order being used even though its one-loop slope changes. Higher-order decoupling corrections modify the matching beyond the question's approximation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
