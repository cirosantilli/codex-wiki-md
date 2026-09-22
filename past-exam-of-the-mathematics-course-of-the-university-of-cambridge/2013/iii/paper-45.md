# Paper 45

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_45.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_45.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take real field coordinates $\phi^I$; for complex [scalar fields](../../../quantum-field-theory.md#scalar-field), split them into real and imaginary parts. Assume a smooth [scalar potential](../../../quantum-field-theory.md#scalar-potential) and positive, canonically normalized [kinetic terms](../../../quantum-field-theory.md#kinetic-term) in a relativistic theory. At a [classical vacuum](../../../quantum-field-theory.md#classical-vacuum), $V_I(\phi_0)=0$. The [Taylor expansion](../../../calculus.md#taylor-expansion) is

$$
V(\phi_0+\xi)=V(\phi_0)+\frac12\xi^I(M^2)_{IJ}\xi^J+O(\|\xi\|^3),\qquad (M^2)_{IJ}=\left.\frac{\partial^2 V}{\partial\phi^I\partial\phi^J}\right|_{\phi_0}.
$$

Thus the [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix) is the [Hessian matrix](../../../calculus.md#hessian-matrix), and its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) give squared masses of the linearized scalar excitations.

Put $X_a(\phi)=it^a\phi$. Infinitesimal invariance of the [scalar potential](../../../quantum-field-theory.md#scalar-potential) gives the identity $V_I X_a^I=0$ at every field value. Differentiate with respect to $\phi^J$ and evaluate at the [classical vacuum](../../../quantum-field-theory.md#classical-vacuum):

$$
(M^2)_{JI}X_a^I(\phi_0)+V_I(\phi_0)\partial_JX_a^I(\phi_0)=0,
\qquad\boxed{M^2(it^a\phi_0)=0.}
$$

Every nonzero infinitesimal symmetry direction therefore lies in the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of the [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix). This is the classical [Goldstone theorem](../../../quantum-field-theory.md#goldstone-theorem) expressed through [Goldstone directions in the scalar mass matrix](../../../quantum-field-theory.md#goldstone-directions-in-the-scalar-mass-matrix).

Let $H_0$ be the full [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) of $\phi_0$. The linear map from the [Lie algebra](../../../lie-algebra.md) of $G$ to field space, $T\mapsto iT\phi_0$, has kernel equal to the [Lie algebra](../../../lie-algebra.md) of $H_0$. The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives

$$
\boxed{\dim\operatorname{span}\{it^a\phi_0\}=\dim G-\dim H_0.}
$$

There are consequently **at least $\dim G-\dim H_0$ massless scalar directions**, namely the tangent directions to the symmetry orbit through the [classical vacuum](../../../quantum-field-theory.md#classical-vacuum). If the intended $H$ is $H_0$, these are the $\dim G-\dim H$ symmetry-required [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson). Exactly that many massless modes occur if the [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix) is positive definite on a complement of those tangent directions. A nonsingular positive field-space kinetic metric changes normalization, but not the number of zero masses.

Two qualifications are needed for the literal assumptions. A subgroup fixing the [classical vacuum](../../../quantum-field-theory.md#classical-vacuum) need not be the full [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup). For example, take $G=SO(3)$ acting on a real triplet and $V=\lambda(|\phi|^2-v^2)^2/8$ with $\lambda,v>0$. At $\phi_0=ve_3$, the [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix) is $\lambda v^2\operatorname{diag}(0,0,1)$: there are two massless modes. Choosing $H=\{1\}$ satisfies the printed invariance condition but would incorrectly predict three. The full [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) is $SO(2)$.

Even with the full [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup), symmetry does not exclude an [accidental massless scalar](../../../quantum-field-theory.md#accidental-massless-scalar). Take $G=SO(2)$ rotating $(x,y)$, with an invariant singlet $z$, and

$$
V(x,y,z)=\frac\lambda4(x^2+y^2-v^2)^2+\kappa z^4,\qquad\lambda,\kappa>0.
$$

At $(v,0,0)$ the full continuous stabilizer is trivial, but the [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix) is $\operatorname{diag}(2\lambda v^2,0,0)$. One zero direction is the [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson); the other is an [accidental massless scalar](../../../quantum-field-theory.md#accidental-massless-scalar) at quadratic order. **The proof establishes the symmetry-required count, not unconditional equality with the total number of massless fields.** The statement concerns global internal symmetry; gauging it changes the physical interpretation through the [Higgs mechanism](../../../standard-model.md#higgs-mechanism).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Assume $\lambda>0$ and $v>0$. The [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) is the sphere $|\phi|=v$. Choose $\phi_0=ve_3$. For the given generators, $t^3\phi_0=0$ whereas $t^1\phi_0$ and $t^2\phi_0$ are nonzero and independent. The [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) of [SU(2)](../../../topological-group.md#su-2-group) rotates this sphere, and the full connected [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) of $ve_3$ is generated by $t^3$. Hence the classical symmetry pattern is

$$
\boxed{SU(2)\longrightarrow U(1).}
$$

The central element of [SU(2)](../../../topological-group.md#su-2-group) acts trivially on the triplet and belongs to this stabilizer; it does not add a separate broken direction. The gauge-field-free representative has zero [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) and constant scalar magnitude. Locally near this nonzero [classical vacuum](../../../quantum-field-theory.md#classical-vacuum), [unitary gauge](../../../standard-model.md#unitary-gauge) aligns the triplet along the third axis.

First make the gauge normalization explicit. Write the gauge [kinetic term](../../../quantum-field-theory.md#kinetic-term) as $-\mathcal N F^a_{\mu\nu}F^{a\mu\nu}/4$, where $\operatorname{Tr}(t^at^b)=\mathcal N\delta^{ab}$ if $F=F^at^a$ is the matrix used inside the printed trace. [Canonical normalization of a gauge kinetic term](../../../relativistic-quantum-field.md#canonical-normalization-of-a-gauge-kinetic-term) gives

$$
\mathcal A^a_\mu=\sqrt{\mathcal N}\,A^a_\mu,\qquad g_c=\frac{g}{\sqrt{\mathcal N}},\qquad
\mathcal F^a_{\mu\nu}=\partial_\mu\mathcal A^a_\nu-\partial_\nu\mathcal A^a_\mu-g_c\epsilon^{abc}\mathcal A^b_\mu\mathcal A^c_\nu.
$$

For a conventionally normalized component trace, $\mathcal N=1$ and $g_c=g$. If the trace is the ordinary matrix trace in the displayed three-dimensional representation, $\operatorname{Tr}(t^at^b)=2\delta^{ab}$ and $\mathcal N=2$. The PDF does not specify which trace convention is intended; both are covered by this formula.

In [unitary gauge](../../../standard-model.md#unitary-gauge), the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) is

$$
D_\mu\phi=\bigl(-g_c(v+\eta)\mathcal A^2_\mu,\quad g_c(v+\eta)\mathcal A^1_\mu,\quad\partial_\mu\eta\bigr)^T.
$$

Expanding this [kinetic term](../../../quantum-field-theory.md#kinetic-term) and the [scalar potential](../../../quantum-field-theory.md#scalar-potential) gives the complete physical-field [Lagrangian](../../../calculus-of-variations.md#lagrangian)

$$
\mathcal L=-\frac14\mathcal F^a_{\mu\nu}\mathcal F^{a\mu\nu}
+\frac12(\partial_\mu\eta)(\partial^\mu\eta)
+\frac{g_c^2}{2}(v+\eta)^2\bigl[(\mathcal A^1_\mu)^2+(\mathcal A^2_\mu)^2\bigr]
-\frac{\lambda v^2}{2}\eta^2-\frac{\lambda v}{2}\eta^3-\frac\lambda8\eta^4.
$$

Here a square of a vector means its contraction with the [Minkowski metric](../../../special-relativity.md#minkowski-metric), in signature $(+---)$. The labels 1 and 2 represent massive vectors; 3 represents the surviving Abelian vector.

To display their charge and all interactions more clearly, put $a_\mu=\mathcal A^3_\mu$, $W^\pm_\mu=(\mathcal A^1_\mu\mp i\mathcal A^2_\mu)/\sqrt2$, and define

$$
f_{\mu\nu}=\partial_\mu a_\nu-\partial_\nu a_\mu,\qquad
C_{\mu\nu}=W^+_\mu W^-_\nu-W^+_\nu W^-_\mu,
$$



$$
G^\pm_{\mu\nu}=(\partial_\mu\pm ig_ca_\mu)W^\pm_\nu-(\partial_\nu\pm ig_ca_\nu)W^\pm_\mu.
$$

With the sign of [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) printed in the paper, $\mathcal F^3=f+ig_cC$ and $G^\pm=(\mathcal F^1\mp i\mathcal F^2)/\sqrt2$. Thus the same [Lagrangian](../../../calculus-of-variations.md#lagrangian) becomes

$$
\boxed{\begin{aligned}
\mathcal L={}&-\frac14(f_{\mu\nu}+ig_cC_{\mu\nu})(f^{\mu\nu}+ig_cC^{\mu\nu})
-\frac12G^+_{\mu\nu}G^{-\mu\nu}
+\frac12(\partial\eta)^2+g_c^2(v+\eta)^2W^+_\mu W^{-\mu}\\
&-\frac{\lambda v^2}{2}\eta^2-\frac{\lambda v}{2}\eta^3-\frac\lambda8\eta^4.
\end{aligned}}
$$

The **physical masses** are

$$
\boxed{m_a=0,\qquad m_{W^+}=m_{W^-}=g_cv,\qquad m_\eta=\sqrt\lambda\,v.}
$$

In particular, literal adjoint matrix trace gives $m_W=gv/\sqrt2$; the standard canonical component convention gives $m_W=gv$. These are descriptions with differently normalized couplings, not different physical spectra.

The complex vector pair carries opposite charges under the unbroken [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry). The [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) terms contain $aW^+W^-$ cubic interactions, $aaW^+W^-$ quartic interactions, and four-vector interactions involving the charged fields. There is no pure Abelian cubic or quartic self-interaction. The [Higgs mode](../../../quantum-field-theory.md#higgs-mode) $\eta$ has cubic and quartic scalar interactions and couples through $2g_c^2v\eta W^+W^-+g_c^2\eta^2W^+W^-$. It is neutral and has no tree-level $\eta aa$ interaction. This is the [physical charged-vector Lagrangian for an adjoint SU2 Higgs model](../../../relativistic-quantum-field.md#physical-charged-vector-lagrangian-for-an-adjoint-su2-higgs-model).

If the angular fields $\pi_1$ and $\pi_2$ were retained, their vanishing potential masses would identify the two [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson) of the ungauged triplet. In the [gauge theory](../../../quantum-field-theory.md#gauge-theory) they mix with the broken-direction [gauge fields](../../../relativistic-quantum-field.md#gauge-field) and can be removed by [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing); the [Higgs mechanism](../../../standard-model.md#higgs-mechanism) uses them as the longitudinal polarizations of the two massive vectors. They are not additional physical massless scalars. The physical degrees of freedom are conserved: $3+3\times2=9$ before rearrangement, and $1+2\times3+2=9$ afterwards.

**This is not the [Standard Model](../../../standard-model.md) [electroweak interaction](../../../standard-model.md#electroweak-interaction).** It has three original [gauge bosons](../../../relativistic-quantum-field.md#gauge-boson), leaving two massive charged vectors and one massless neutral vector, with no massive neutral [Z boson](../../../standard-model.md#z-boson). The [Standard Model](../../../standard-model.md) instead has $SU(2)_L\times U(1)_Y$, a complex [Higgs doublet](../../../standard-model.md#higgs-field), and three massive vectors plus the [photon](../../../quantum-mechanics.md#photon). Its charge is $Q=T_3+Y$, not just the surviving $T_3$. Adding [fermions](../../../quantum-mechanics.md#fermion) cannot supply the missing gauge generator or turn the surviving neutral vector into both a [photon](../../../quantum-mechanics.md#photon) and a [Z boson](../../../standard-model.md#z-boson). In particular, the usual right-handed [fermions](../../../quantum-mechanics.md#fermion) in the [Standard Model](../../../standard-model.md) are [SU(2)](../../../topological-group.md#su-2-group) singlets; they would have zero charge if only $T_3$ were available, instead of the charges produced by [hypercharge](../../../standard-model.md#hypercharge).

## 2

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use [natural units](../../../physics.md#natural-units) and the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $(+---)$, and work at tree level with on-shell final particles. Write $M=m_H$ and, for a final particle of mass $m$, $\beta_m=\sqrt{1-4m^2/M^2}$. In the [Higgs boson](../../../standard-model.md#higgs-boson) rest frame the [Lorentz-invariant phase-space measure](../../../quantum-mechanics.md#lorentz-invariant-phase-space-measure) reduces to

$$
d\Phi_2=\frac{|\boldsymbol k|}{16\pi^2M}\,d\Omega=\frac{\beta_m}{32\pi^2}\,d\Omega,
\qquad\int d\Phi_2=\frac{\beta_m}{8\pi}.
$$

To obtain this, integrate the momentum delta function to set $\boldsymbol k_2=-\boldsymbol k_1$; the energy delta function is $\delta(M-2\sqrt{k^2+m^2})$, whose radial Jacobian is $E/(2k)$. Hence for an angle-independent final-state [spin sum](../../../relativistic-quantum-field.md#spin-sum) $S=\sum|\mathcal M|^2$,

$$
\Gamma=\frac{\beta_m S}{16\pi M}.
$$

There is no initial-state spin average for a scalar, and neither charged-particle pair here requires an identical-particle factor of $1/2$.

For [Higgs decay to two W bosons](../../../standard-model.md#higgs-decay-to-two-w-bosons), the [Feynman vertex](../../../perturbative-quantum-field-theory.md#interaction-vertex) gives $\mathcal M=(2m_W^2/v)\varepsilon_1^*\!\cdot\varepsilon_2^*$, up to an overall phase. Contracting the two [massive vector polarization sums](../../../relativistic-quantum-field.md#polarization-sum-for-a-massive-vector-boson) gives

$$
S_W=\frac{4m_W^4}{v^2}\left[2+\frac{(k_1\cdot k_2)^2}{m_W^4}\right],\qquad
k_1\cdot k_2=\frac{M^2-2m_W^2}{2}.
$$

The constant 2 follows from $4-1-1$ in the contraction, with the last term coming from the two momentum projectors. Putting $x_W=m_W^2/M^2$, the **full massive result** is

$$
\boxed{\Gamma(H\to W^+W^-)=\frac{M^3}{16\pi v^2}\sqrt{1-4x_W}\,(1-4x_W+12x_W^2),\qquad M\geq2m_W.}
$$

The on-shell two-body width is zero below this threshold; decays through off-shell [W bosons](../../../standard-model.md#w-boson) into more particles are different channels.

For [Higgs decay to a fermion pair](../../../standard-model.md#higgs-decay-to-a-fermion-pair), put $y_b=m_b/v$. The amplitude is $\mathcal M=-y_b\bar u(k_1)v(k_2)$, up to an overall phase and a color Kronecker delta. The [fermion spin sums](../../../relativistic-quantum-field.md#fermion-spin-sum) and [gamma-matrix trace](../../../relativistic-quantum-field.md#gamma-matrix-trace) give

$$
S_b=N_cy_b^2\operatorname{tr}[(\not k_1+m_b)(\not k_2-m_b)]
=4N_cy_b^2(k_1\cdot k_2-m_b^2)
=2N_cy_b^2(M^2-4m_b^2).
$$

The [color multiplicity in a decay width](../../../standard-model.md#color-multiplicity-in-a-decay-width) is $N_c=3$: only a quark and antiquark with matching colors contribute, so the factor is three rather than nine. Therefore

$$
\boxed{\Gamma(H\to\bar b b)=\frac{3m_b^2M}{8\pi v^2}\left(1-\frac{4m_b^2}{M^2}\right)^{3/2},\qquad M\geq2m_b.}
$$

Again the on-shell two-body width is zero below threshold. This is a partonic tree-level answer with every mass retained; [hadronization](../../../standard-model.md#hadronization) is outside the specified calculation.

**The [W boson](../../../standard-model.md#w-boson) channel dominates for large $M$ within the tree-level comparison.** The widths scale as $M^3/v^2$ and $m_b^2M/v^2$, respectively, and

$$
\boxed{\frac{\Gamma(H\to W^+W^-)}{\Gamma(H\to\bar b b)}\sim\frac{M^2}{6m_b^2}.}
$$

The enhancement comes from [longitudinal polarization of a massive vector boson](../../../relativistic-quantum-field.md#longitudinal-polarization-of-a-massive-vector-boson): its polarization vector grows as momentum divided by $m_W$. Thus the longitudinal pair survives the apparently small $m_W^2$ factor in the interaction. At masses so large that the scalar sector is strongly coupled, the tree-level extrapolation itself needs corrections.

## 3

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $s=q^2>0$, neglect $m_e$, and average over the two spin states of each incoming particle. Only the single-[photon](../../../quantum-mechanics.md#photon) channel is being considered. The spectral-density symbol $\rho_h$ is not defined in the question, so specify its normalization before calculating. A useful photon-field convention is

$$
\begin{aligned}
W_A^{\mu\nu}(q)&=\sum_{X\,\mathrm{hadronic}}\int d\Pi_X\,(2\pi)^4\delta^{(4)}(q-p_X)
\langle0|A^\mu(0)|X\rangle\langle X|A^\nu(0)|0\rangle\\
&=2\pi\rho_h(s)\left(-g^{\mu\nu}+\frac{q^\mu q^\nu}{s}\right),\qquad q^0>0.
\end{aligned}
$$

Here $d\Pi_X$ is the product of final-particle measures $d^3k/[(2\pi)^3 2E]$, including the appropriate sums and symmetry factors. [Lorentz invariance](../../../special-relativity.md#lorentz-invariance) and [current conservation](../../../quantum-field-theory.md#conserved-current) give the transverse tensor form. In this convention $\rho_h$ is the [hadronic photon spectral density](../../../quantum-field-theory.md#hadronic-photon-spectral-density), with mass dimension $-2$, rather than a density of a stationary time series.

The electron annihilation amplitude can be written $e\bar v(p_+)\gamma_\mu u(p_-)\langle X|A^\mu|0\rangle$, up to an overall phase. The [leptonic tensor](../../../standard-model.md#leptonic-tensor) after the initial spin average is

$$
L_{\mu\nu}=\frac14\operatorname{tr}[\not p_+\gamma_\mu\not p_-\gamma_\nu]
=p_{+\mu}p_{-\nu}+p_{+\nu}p_{-\mu}-g_{\mu\nu}\,p_+\cdot p_-.
$$

It obeys $q^\mu L_{\mu\nu}=0$ and $g^{\mu\nu}L_{\mu\nu}=-s$. In the center-of-momentum frame, the flux denominator in the hint is $2s$, since the relative speed is 2 and each beam energy is $\sqrt s/2$. Contracting the tensors gives the **inclusive [relativistic cross-section](../../../quantum-mechanics.md#relativistic-scattering-cross-section)**

$$
\boxed{\sigma_h(s)=\frac{e^2}{2s}L_{\mu\nu}W_A^{\mu\nu}(q)=\pi e^2\rho_h(s)=4\pi^2\alpha\rho_h(s),\qquad\alpha=\frac{e^2}{4\pi}.}
$$

Here $\alpha$ is the [fine-structure constant](../../../perturbative-quantum-field-theory.md#fine-structure-constant). The $1/4$ in the initial spin average is essential because the hint's particles were spinless.

For the other common convention, define the hadronic electromagnetic current with the coupling omitted, $J_h^\mu=\sum_fQ_f\bar q_f\gamma^\mu q_f$, and write its inclusive tensor as

$$
W_J^{\mu\nu}=2\pi\rho_J(s)(q^\mu q^\nu-sg^{\mu\nu}).
$$

Equivalently, for $i\int d^4x\,e^{iqx}\langle0|T J_h^\mu(x)J_h^\nu(0)|0\rangle=(q^\mu q^\nu-q^2g^{\mu\nu})\Pi_J(q^2)$, one has $\rho_J=\operatorname{Im}\Pi_J/\pi$. At leading order in the electromagnetic interaction, $\langle X|A^\mu|0\rangle$ is proportional to $e\langle X|J_h^\mu|0\rangle/s$. Thus

$$
\rho_h(s)=\frac{e^2}{s}\rho_J(s),\qquad
\boxed{\sigma_h(s)=\frac{16\pi^3\alpha^2}{s}\rho_J(s).}
$$

If the symbol $\rho_h$ is instead used for this dimensionless [hadronic electromagnetic-current spectral density](../../../perturbative-quantum-field-theory.md#hadronic-electromagnetic-current-spectral-density), the last formula applies with $\rho_J$ renamed $\rho_h$. The normalization must not be silently switched between these formulas.

At $\sqrt s$ well above the [strong-coupling scale](../../../perturbative-quantum-field-theory.md#strong-coupling-scale) of [Quantum chromodynamics](../../../standard-model.md#quantum-chromodynamics), [asymptotic freedom](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) makes production over distances of order $1/\sqrt s$ perturbative. The electromagnetic current initially creates a [quark](../../../standard-model.md#quark)-[antiquark](../../../standard-model.md#antiquark) pair. Subsequent strong interactions produce [hadrons](../../../physics.md#hadron), but an inclusive sum over all hadronic final states is much less sensitive to this rearrangement than an exclusive channel. This is the regime in which [quark-hadron duality](../../../standard-model.md#quark-hadron-duality) motivates a leading [parton model](../../../standard-model.md#parton-model) calculation, with radiative and power-suppressed corrections. It is not a pointwise theorem at individual resonances or near thresholds; the comparison is most reliable for sufficiently inclusive or suitably averaged high-energy observables. This argument remains restricted to photon exchange, even where additional electroweak channels could also contribute.

For one active massless [quark](../../../standard-model.md#quark) flavor with charge $Q_fe$, the tree-level [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) is

$$
\mathcal M_f=\frac{e^2Q_f}{s}[\bar v(p_+)\gamma_\mu u(p_-)][\bar u(k_q)\gamma^\mu v(k_{\bar q})].
$$

The two [gamma-matrix traces](../../../relativistic-quantum-field.md#gamma-matrix-trace), the initial spin average, and the final [color charge](../../../standard-model.md#color-charge) sum yield

$$
\overline{\sum}|\mathcal M_f|^2=2N_ce^4Q_f^2\frac{t^2+u^2}{s^2}
=N_ce^4Q_f^2(1+\cos^2\theta),
$$

where $t=-s(1-\cos\theta)/2$ and $u=-s(1+\cos\theta)/2$. The massless [two-body Lorentz-invariant phase space](../../../relativistic-quantum-field.md#two-body-lorentz-invariant-phase-space) then gives

$$
\frac{d\sigma_f}{d\Omega}=\frac{N_c\alpha^2Q_f^2}{4s}(1+\cos^2\theta),\qquad
\int d\Omega\,(1+\cos^2\theta)=\frac{16\pi}{3}.
$$

Summing the distinct final flavors, rather than interfering amplitudes for them, gives

$$
\boxed{\sigma_h^{(0)}(s)=\frac{4\pi\alpha^2}{3s}N_c\sum_{f\,\mathrm{active}}Q_f^2.}
$$

According to the permitted approximation in the paper, active flavors satisfy $m_f^2<s$ and are treated as massless; the others are omitted. This is the stipulated step approximation, not the exact pair-production threshold $s\geq4m_f^2$.

The **[hadronic R ratio](../../../quantum-mechanics.md#hadronic-r-ratio)** is $R=N_c\sum Q_f^2$, relative to the massless muon-pair [relativistic cross-section](../../../quantum-mechanics.md#relativistic-scattering-cross-section) $4\pi\alpha^2/(3s)$. If $N_u$ and $N_d$ active flavors have charges $2/3$ and $-1/3$, respectively,

$$
R=\frac{N_c}{9}(4N_u+N_d).
$$

For $N_c=3$, the usual sets of three, four, five and six active flavors give $R=2,10/3,11/3,5$. In the two spectral conventions the same leading calculation gives

$$
\boxed{\rho_J^{(0)}(s)=\frac{N_c\sum_fQ_f^2}{12\pi^2},\qquad
\rho_h^{(0)}(s)=\frac{\alpha N_c\sum_fQ_f^2}{3\pi s}.}
$$

## 4

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

An **[effective field theory](../../../quantum-field-theory.md#effective-field-theory) is a controlled description of specified low-energy degrees of freedom at a chosen accuracy**. It does not require knowing all physics at arbitrarily short distances. If new particles or strong dynamics enter at a scale $M$, processes with characteristic energy and momentum transfers $E\ll M$ can be described using the light fields and interactions consistent with their symmetries. In [natural units](../../../physics.md#natural-units), four-dimensional [power counting in quantum field theory](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory) organizes a local [Lagrangian](../../../calculus-of-variations.md#lagrangian) as

$$
\mathcal L_{\mathrm{EFT}}=\mathcal L_{d\leq4}+\sum_{d>4}\sum_i\frac{C_i^{(d)}(\mu)}{M^{d-4}}\mathcal O_i^{(d)}.
$$

Here $\mathcal O_i^{(d)}$ has [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) $d$, the dimensionless $C_i^{(d)}$ are [Wilson coefficients](../../../quantum-field-theory.md#wilson-coefficient), and $\mu$ is a [renormalization scale](../../../perturbative-quantum-field-theory.md#renormalization-scale). In a relativistic vacuum with canonical fields, a typical insertion of a dimension-$d$ interaction contributes an additional power $(E/M)^{d-4}$, multiplied by its couplings and any light mass ratios. Additional expansions, such as a loop expansion, must also be specified. Symmetry or on-shell identities can postpone a particular observable's first correction.

The theory is useful when its retained states and expansion parameters adequately describe the experiment. It ceases to be a reliable truncated local description near an omitted particle's production threshold, near a heavy propagator pole, or where the retained dynamics become too strongly coupled for an assumed perturbative expansion. A light particle cannot be removed merely because one wants fewer variables: its propagation can produce nonanalytic momentum dependence that must be represented by retained light fields. [Heavy-field decoupling](../../../quantum-field-theory.md#heavy-field-decoupling) can shift renormalizable masses and couplings as well as generate suppressed interactions; those low-energy parameters must be measured or matched, not assumed unchanged. The [ultraviolet cutoff](../../../quantum-field-theory.md#ultraviolet-cutoff) is an organizational scale, while a calculation may use a regulator other than a hard momentum cutoff.

Construction starts by identifying the light particles, the hierarchy of scales, and the exact or approximate symmetries relevant to the problem. Form all allowed [local field operators](../../../quantum-field-theory.md#local-operator-physics) through the desired order in [power counting in quantum field theory](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory). Choose an [operator basis in effective field theory](../../../quantum-field-theory.md#operator-basis-in-effective-field-theory): remove equivalent terms by [integration by parts](../../../calculus.md#integration-by-parts), algebraic identities and allowed [field redefinitions](../../../perturbative-quantum-field-theory.md#field-redefinition). Operators proportional to lower-order [equations of motion](../../../classical-mechanics.md#equation-of-motion) can be [redundant operators](../../../perturbative-quantum-field-theory.md#redundant-operator) for on-shell amplitudes, provided coefficients are consistently transformed. This reduces bookkeeping without imposing additional physics assumptions.

If an [ultraviolet completion](../../../quantum-field-theory.md#ultraviolet-completion) is known, determine the [Wilson coefficients](../../../quantum-field-theory.md#wilson-coefficient) by [matching in effective field theory](../../../quantum-field-theory.md#matching-in-effective-field-theory): calculate low-energy amplitudes or appropriate correlation functions in both descriptions using the same infrared conventions, and adjust coefficients so they agree to the chosen order. Equivalently, [integrating out a field](../../../quantum-field-theory.md#integrating-out-a-field) performs its [path integral](../../../quantum-field-theory.md#path-integral) while retaining the light fields as backgrounds. Heavy propagators have an analytic expansion below their singularities, producing a [derivative expansion](../../../quantum-field-theory.md#derivative-expansion); heavy loops also generate local terms and logarithms in their coefficients. Without a specified [ultraviolet completion](../../../quantum-field-theory.md#ultraviolet-completion), the coefficients are parameters to be constrained by data.

An [effective field theory](../../../quantum-field-theory.md#effective-field-theory) remains predictive even when it contains [nonrenormalizable interactions](../../../perturbative-quantum-field-theory.md#nonrenormalizable-interaction). At each fixed order in energy and loops there are finitely many required coefficients and [counterterms](../../../perturbative-quantum-field-theory.md#counterterm). [Renormalization](../../../perturbative-quantum-field-theory.md#renormalization) absorbs divergences into that order's allowed operators. The [renormalization group](../../../critical-phenomenon.md#renormalization-group) evolves the [Wilson coefficients](../../../quantum-field-theory.md#wilson-coefficient) between matching and measurement scales, compensating scale dependence in matrix elements and, when appropriate, resumming large logarithms. The [truncation error in effective field theory](../../../perturbative-quantum-field-theory.md#truncation-error-in-effective-field-theory) is estimated from the first omitted orders, under a stated coupling-size assumption; it is separate from parameter uncertainty and cannot be inferred merely by writing down infinitely many terms.

A concrete example is [heavy scalar exchange in effective field theory](../../../quantum-field-theory.md#heavy-scalar-exchange-in-effective-field-theory). Take a light real [scalar field](../../../quantum-field-theory.md#scalar-field) $\varphi$ and a heavy real [scalar field](../../../quantum-field-theory.md#scalar-field) $S$, with

$$
\mathcal L_{\mathrm{UV}}=\frac12(\partial\varphi)^2-\frac{m^2}{2}\varphi^2-\frac\lambda{4!}\varphi^4
+\frac12(\partial S)^2-\frac{M^2}{2}S^2-\frac a2 S\varphi^2,\qquad M\gg m,E.
$$

The coupling $a$ has mass dimension one. The light-field symmetry is $\varphi\mapsto-\varphi$. For $m^2\geq0$ and $\lambda>3a^2/M^2$, the displayed [scalar potential](../../../quantum-field-theory.md#scalar-potential) is bounded below: completing the square in $S$ leaves a positive light quartic. Thus the example can be treated as a stable theory around $S=\varphi=0$, with weak enough couplings for the tree approximation.

At tree level the heavy [equation of motion](../../../classical-mechanics.md#equation-of-motion) is $(M^2+\Box)S=-a\varphi^2/2$. Substitute its solution back into the action, including both its quadratic and source terms, to obtain

$$
\Delta\mathcal L_{\mathrm{eff}}=\frac{a^2}{8}\varphi^2\frac1{M^2+\Box}\varphi^2
=\frac{a^2}{8M^2}\varphi^4-\frac{a^2}{8M^4}\varphi^2\Box\varphi^2+\frac{a^2}{8M^6}\varphi^2\Box^2\varphi^2+\cdots.
$$

This is a [derivative expansion](../../../quantum-field-theory.md#derivative-expansion) valid for small momentum transfers, not an exact local replacement near the pole. The first term gives **$\lambda_{\mathrm{eff}}=\lambda-3a^2/M^2$** in the $-\lambda_{\mathrm{eff}}\varphi^4/4!$ convention. After [integration by parts](../../../calculus.md#integration-by-parts), the next term is $+a^2(\partial_\mu\varphi^2)(\partial^\mu\varphi^2)/(8M^4)$; it is a dimension-six local operator. Writing $a=g_*M$ puts its coefficient in the usual $g_*^2/M^2$ form. These coefficients are a tree-level [matching in effective field theory](../../../quantum-field-theory.md#matching-in-effective-field-theory) result.

One can directly check the matching through the on-shell [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) for $\varphi\varphi\to\varphi\varphi$. With $s,t,u$ the [Mandelstam variables](../../../special-relativity.md#mandelstam-variables), the full theory has three heavy-exchange channels:

$$
\mathcal M_{\mathrm{UV}}=-\lambda+a^2\left(\frac1{M^2-s}+\frac1{M^2-t}+\frac1{M^2-u}\right).
$$

For $|s|,|t|,|u|\ll M^2$,

$$
\mathcal M_{\mathrm{UV}}=-\lambda+\frac{3a^2}{M^2}+\frac{a^2(s+t+u)}{M^4}
+\frac{a^2(s^2+t^2+u^2)}{M^6}+\cdots.
$$

The [effective field theory](../../../quantum-field-theory.md#effective-field-theory) reproduces these terms in order: a shifted quartic, then local derivative interactions. Since $s+t+u=4m^2$ on shell, the first derivative correction is a light-mass-dependent constant; it vanishes for $m=0$. This illustrates why an [operator basis in effective field theory](../../../quantum-field-theory.md#operator-basis-in-effective-field-theory) can trade some derivative operators for mass-dependent or higher-field interactions using [field redefinitions](../../../perturbative-quantum-field-theory.md#field-redefinition). For massless external particles, the first nonconstant correction in this four-point tree amplitude starts at the following order.

**The example exhibits the central logic: keep the light field, encode virtual heavy exchange in matched local coefficients, and control the error by expanding in momentum divided by the heavy scale.** No heavy particle is actually produced in the domain of the approximation. Near $s=M^2$, the full propagator is resonant and the truncated [effective field theory](../../../quantum-field-theory.md#effective-field-theory) fails; retaining $S$ or adopting a different description is then necessary. Light loops are computed within the [effective field theory](../../../quantum-field-theory.md#effective-field-theory), while higher-order matching supplies the corresponding heavy corrections.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
