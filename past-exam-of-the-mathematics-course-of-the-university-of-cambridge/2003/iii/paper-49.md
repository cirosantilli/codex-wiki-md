# Paper 49

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper49.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper49.pdf)

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

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Assume $\lambda>0$ and $v>0$. The minima of the [scalar potential](../../../quantum-field-theory.md#scalar-potential) have $|\phi|=v$. Choose the [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) $\phi_0=ve_3$. Its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) consists exactly of matrices $\operatorname{diag}(R_2,1)$ with $R_2\in O(2)$, so

$$
\boxed{O(3)\longrightarrow O(2).}
$$

The continuous [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) is $SO(3)\to SO(2)$ and has two broken generators. For the full orthogonal group, the cross-product notation requires the [gauge connection](../../../fiber-bundle.md#connection-vector-bundle) to transform in the adjoint, as an axial vector: $R[A]_\times R^{-1}=[(\det R)RA]_\times$. The [scalar field](../../../quantum-field-theory.md#scalar-field) transforms as the ordinary vector $R\phi$. This [axial transformation of orthogonal gauge connections](../../../standard-model.md#axial-transformation-of-orthogonal-gauge-connections) makes the stated [covariant derivative](../../../general-relativity.md#covariant-derivative) transform correctly even for $\det R=-1$; assigning an ordinary-vector transformation to the connection would fail.

Near this nonzero vacuum, [unitary gauge](../../../standard-model.md#unitary-gauge) removes the two angular [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson) and gives $\phi=(0,0,v+h)$. Put

$$
W_\mu^\pm=\frac{A_\mu^1\mp iA_\mu^2}{\sqrt2},\qquad A_\mu=A_\mu^3,\qquad f_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu.
$$

These are the physical charged [gauge bosons](../../../relativistic-quantum-field.md#gauge-boson), neutral massless [gauge boson](../../../relativistic-quantum-field.md#gauge-boson), and radial [scalar field](../../../quantum-field-theory.md#scalar-field). Directly substituting into the original [gauge field strengths](../../../relativistic-quantum-field.md#gauge-field-strength) gives

$$
\mathcal F_{\mu\nu}^\pm=(\partial_\mu\mp ieA_\mu)W_\nu^\pm-(\partial_\nu\mp ieA_\nu)W_\mu^\pm,\qquad \mathcal F_{\mu\nu}^3=f_{\mu\nu}-ie(W_\mu^+W_\nu^--W_\nu^+W_\mu^-).
$$

The [scalar field](../../../quantum-field-theory.md#scalar-field) [kinetic term](../../../quantum-field-theory.md#kinetic-term) has no radial-vector cross term, because $\partial_\mu\phi$ and $\mathbf A_\mu\times\phi$ lie in perpendicular internal directions. The complete physical gauge-scalar [Lagrangian](../../../calculus-of-variations.md#lagrangian) becomes

$$
\mathcal L=-\frac14\mathcal F^{3\mu\nu}\mathcal F^3_{\mu\nu}-\frac12\mathcal F^{+\mu\nu}\mathcal F^-_{\mu\nu}+\frac12(\partial h)^2+e^2(v+h)^2W_\mu^+W^{-\mu}-\frac12\lambda v^2h^2-\frac12\lambda vh^3-\frac18\lambda h^4.
$$

For each real vector the [mass term](../../../quantum-field-theory.md#mass-term) is $m^2A_\mu A^\mu/2$, while for the complex pair it is $m_W^2W_\mu^+W^{-\mu}$. Hence the [adjoint triplet Higgs spectrum](../../../standard-model.md#adjoint-triplet-higgs-spectrum) is

$$
\boxed{m_{W^+}=m_{W^-}=ev,\qquad m_A=0.}
$$

The radial scalar also has $m_h^2=\lambda v^2$ in the question's potential normalization. The two lost scalar modes supply the longitudinal polarizations of the massive vectors through the [Higgs mechanism](../../../standard-model.md#higgs-mechanism).

For the [lepton](../../../standard-model.md#lepton) [kinetic terms](../../../quantum-field-theory.md#kinetic-term) let $P_L=(1-\gamma^5)/2$, $P_R=(1+\gamma^5)/2$, and denote the left neutral triplet entry by $n_L=c_\alpha\nu_L+s_\alpha N_L$. The missing singlet is the perpendicular combination

$$
\boxed{L^S=P_L(-\nu_e\sin\alpha+N\cos\alpha).}
$$

Its overall sign is immaterial. The real [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) $\left(\begin{smallmatrix}c_\alpha&s_\alpha\\-s_\alpha&c_\alpha\end{smallmatrix}\right)$ is orthogonal, so the sum of the kinetic terms of $n_L$ and $L^S$ is $\bar\nu_Li\not\partial\nu_L+\bar N_Li\not\partial N_L$ with no mixed terms. Combining with the right triplet gives ordinary [Dirac field](../../../relativistic-quantum-field.md#dirac-field) [kinetic terms](../../../quantum-field-theory.md#kinetic-term) for $E^+,N,e$, and only a left-handed [kinetic term](../../../quantum-field-theory.md#kinetic-term) for the massless [neutrino](../../../standard-model.md#neutrino). This is [orthogonal completion of mixed neutral lepton kinetic terms](../../../standard-model.md#orthogonal-completion-of-mixed-neutral-lepton-kinetic-terms). The heavy charged field is $E^+$, as printed in the PDF, not the TeX's $N^+$.

To compute the charge commutator, the [canonical anticommutation relations](../../../quantum-mechanics.md#canonical-anticommutation-relations) imply

$$
[\psi_i^\dagger(\mathbf x)\psi_j(\mathbf x),\psi_k^\dagger(\mathbf y)\psi_l(\mathbf y)]=\delta^3(\mathbf x-\mathbf y)(\delta_{jk}\psi_i^\dagger\psi_l-\delta_{il}\psi_k^\dagger\psi_j).
$$

The quartic terms cancel on reordering the fermions. Thus well-defined normal-ordered integrated bilinears obey [fermionic bilinear charge algebra](../../../quantum-mechanics.md#fermionic-bilinear-charge-algebra), $[Q_C,Q_D]=Q_{[C,D]}$. Left/right mixed [commutators](../../../lie-algebra.md#commutator) vanish since $P_LP_R=0$.

In either triplet, write

$$
K=\begin{pmatrix}0&1&0\\0&0&1\\0&0&0\end{pmatrix},\qquad [K,K^\dagger]=\operatorname{diag}(1,0,-1).
$$

The displayed current has a factor two relative to the projected bilinears, since $1\mp\gamma^5=2P_{L,R}$. Consequently its charges are $T^+=2(Q_K^L+Q_K^R)$ and $T^-=(T^+)^\dagger$. The neutral combinations have canonical anticommutators because $c_\alpha^2+s_\alpha^2=1$. Applying the matrix commutator gives

$$
[T^+,T^-]=4\int d^3x:(E^{+\dagger}E^+-e^\dagger e):=\boxed{\frac4eQ_\ell},
$$

where $Q_\ell=e\int:(E^{+\dagger}E^+-e^\dagger e):$ is the electromagnetic charge in the lepton sector. The neutrino, heavy neutral lepton and singlet contribute zero. This establishes [triplet charged-current closure on electromagnetic charge](../../../quantum-mechanics.md#triplet-charged-current-closure-on-electromagnetic-charge), with the requested proportionality independent of normalization choices for the weak [Noether charges](../../../quantum-field-theory.md#noether-charge). The PDF correctly writes $J^-=(J^+)^\dagger$; the TeX repeats $J^+$ incorrectly. Equal-time algebra does not require conservation of the separate fermionic weak currents after symmetry breaking. For full gauge-theory charges, the corresponding charged-boson contributions must also be included.

## 2

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the source convention $Q=T_3+Y$, with electric charge measured in units of the positron charge. Expanding the [covariant derivative](../../../general-relativity.md#covariant-derivative) in the [fermion](../../../quantum-mechanics.md#fermion) [kinetic term](../../../quantum-field-theory.md#kinetic-term) gives interaction $-\bar f\gamma_\mu(gT_3A_3^\mu+g'YB^\mu)f$. Substituting the given neutral-field rotation, the coefficient of $Z^\mu$ is

$$
gc_WT_3-g's_WY=\frac g{c_W}(T_3-s_W^2Q),\qquad s_W=\sin\theta_W,\quad c_W=\cos\theta_W.
$$

The photon coefficient is $gs_W(T_3+Y)=eQ$, with $e=gs_W=g'c_W$. For a [Dirac field](../../../relativistic-quantum-field.md#dirac-field), $T_3$ acts only on its left-handed component. Thus

$$
T_3P_L-Qs_W^2=\frac12\bigl[(T_3-2Qs_W^2)-T_3\gamma^5\bigr].
$$

The [weak neutral current](../../../standard-model.md#neutral-current) interaction consequently has the requested form, with

$$
\boxed{c_v=T_3-2Qs_W^2,\qquad c_a=T_3.}
$$

The [electroweak representation and hypercharge table](../../../standard-model.md#electroweak-representation-and-hypercharge-table) gives the following values for one generation:

| Type | $T_3$ on left | $Q$ | $Y_L$ | $Y_R$ | $c_v$ | $c_a$ |
| --- | --- | --- | --- | --- | --- | --- |
| [Neutrino](../../../standard-model.md#neutrino) | $1/2$ | $0$ | $-1/2$ | absent | $1/2$ | $1/2$ |
| Charged [lepton](../../../standard-model.md#lepton) | $-1/2$ | $-1$ | $-1/2$ | $-1$ | $-1/2+2s_W^2$ | $-1/2$ |
| Up-type [quark](../../../standard-model.md#quark) | $1/2$ | $2/3$ | $1/6$ | $2/3$ | $1/2-4s_W^2/3$ | $1/2$ |
| Down-type [quark](../../../standard-model.md#quark) | $-1/2$ | $-1/3$ | $1/6$ | $-1/3$ | $-1/2+2s_W^2/3$ | $-1/2$ |

These [neutral-current vector and axial couplings](../../../standard-model.md#neutral-current-vector-and-axial-couplings) use the source's vertex prefactor $g/(2c_W)$. They are twice the coefficients used with prefactor $g/c_W$; the latter convention must not be mixed into this calculation. For the neutrino, the [chiral projector](../../../relativistic-quantum-field.md#chiral-projector) removes the inactive right-handed component automatically.

Set $G=g/(2c_W)$ and suppress the species label. For outgoing momenta $k_1,k_2$, the amplitude is, up to an irrelevant phase,

$$
\mathcal M=G\epsilon_\mu(p)\bar u(k_1)\gamma^\mu(c_v-c_a\gamma^5)v(k_2),\qquad p=k_1+k_2.
$$

The final-state [spin sum](../../../relativistic-quantum-field.md#spin-sum) is the [Dirac trace](../../../relativistic-quantum-field.md#gamma-matrix-trace) of $\not k_1\gamma^\mu(c_v-c_a\gamma^5)\not k_2\gamma^\nu(c_v-c_a\gamma^5)$. Anticommutation of $\gamma^5$ with the [gamma matrices](../../../algebra.md#gamma-matrices) makes its symmetric part

$$
T_{\mathrm{sym}}^{\mu\nu}=4(c_v^2+c_a^2)(k_1^\mu k_2^\nu+k_1^\nu k_2^\mu-g^{\mu\nu}k_1\cdot k_2).
$$

The vector-axial cross term is proportional to the antisymmetric [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol), so it contracts to zero with the symmetric [massive vector polarization sum](../../../relativistic-quantum-field.md#polarization-sum-for-a-massive-vector-boson) $-g_{\mu\nu}+p_\mu p_\nu/M_Z^2$. Since $k_1^2=k_2^2=0$, the symmetric tensor is transverse to $p$ as well. Only $-g_{\mu\nu}$ remains, and

$$
-g_{\mu\nu}T_{\mathrm{sym}}^{\mu\nu}=8(c_v^2+c_a^2)k_1\cdot k_2=4M_Z^2(c_v^2+c_a^2).
$$

Multiplying by $G^2$ proves the [massless fermion Z decay spin sum](../../../standard-model.md#massless-fermion-z-decay-spin-sum):

$$
\boxed{\sum_{\lambda,s_1,s_2}|\mathcal M|^2=\frac{g^2M_Z^2}{c_W^2}(c_v^2+c_a^2).}
$$

For the [decay width](../../../relativistic-quantum-field.md#decay-width), average over the three initial polarizations. Rotational invariance makes the integrated width the same for each initial spin state, so the [massive-vector spin average](../../../relativistic-quantum-field.md#massive-vector-spin-average) is legitimate even for a single prepared polarization. In the rest frame, the delta functions in [two-body Lorentz-invariant phase space](../../../relativistic-quantum-field.md#two-body-lorentz-invariant-phase-space) leave

$$
d\Phi_2=\frac{d\Omega}{32\pi^2},\qquad\int d\Phi_2=\frac1{8\pi}.
$$

This follows by setting $\mathbf k_2=-\mathbf k_1$ and integrating $\delta(M_Z-2|\mathbf k_1|)$; the radial integration supplies a factor $1/2$. Hence

$$
\Gamma_f=\frac1{2M_Z}\frac13\sum|\mathcal M|^2\frac1{8\pi}=\boxed{\frac{g^2M_Z}{48\pi c_W^2}(c_v^2+c_a^2)}.
$$

For a [quark](../../../standard-model.md#quark) species multiply by three colors, with strong-interaction radiative corrections when comparing with data. For one effectively massless active [neutrino](../../../standard-model.md#neutrino), $c_v=c_a=1/2$, so $\Gamma_\nu=g^2M_Z/(96\pi c_W^2)=G_FM_Z^3/(12\sqrt2\pi)$.

The total resonance width contains visible charged-lepton and hadron decays plus $N_\nu\Gamma_\nu$. Thus the measured invisible contribution determines

$$
\boxed{N_\nu=\frac{\Gamma_Z-\Gamma_{\mathrm{visible}}}{\Gamma_\nu}.}
$$

Early resonance measurements supported three light active [neutrino](../../../standard-model.md#neutrino) species, with experimental uncertainties; the [OPAL analysis of its 1989 data](https://inspirehep.net/files/afa87f449c4b3cb87894b53955b564da) explicitly compares the three- and four-species predictions. Under the question's assumption that every possible family has a massless [neutrino](../../../standard-model.md#neutrino) with ordinary weak couplings, this constrains the number of such families. The inference does not exclude additional neutrinos heavier than $M_Z/2$ or [gauge singlet](../../../representation-theory.md#gauge-singlet) sterile states with no ordinary $Z$ coupling. This is [light-neutrino counting from the Z width](../../../standard-model.md#light-neutrino-counting-from-the-z-width).

## 3

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $\varepsilon=i\sigma_2=\left(\begin{smallmatrix}0&1\\-1&0\end{smallmatrix}\right)$, so $\varepsilon^{-1}=-\varepsilon$. Direct multiplication of the [Pauli matrices](../../../algebra.md#pauli-matrices) gives $\varepsilon\sigma_i^*\varepsilon=\sigma_i$, equivalently $\varepsilon\sigma_i^*\varepsilon^{-1}=-\sigma_i$. For $U=\exp(i\theta_i\sigma_i/2)\in SU(2)$ this implies

$$
\varepsilon U^*\varepsilon^{-1}=U.
$$

Therefore $\phi^c=\varepsilon\phi^*$ transforms as the same weak [fundamental representation](../../../semisimple-lie-algebra.md#fundamental-representation) doublet as $\phi$, while complex conjugation reverses its [hypercharge](../../../standard-model.md#hypercharge) to $-1/2$. This is the [Higgs conjugate doublet](../../../standard-model.md#higgs-conjugate-doublet). The [Yukawa coupling](../../../standard-model.md#yukawa-interaction) product $\bar L\phi^cu_R$ is an $SU(2)$ singlet, and its hypercharges add to

$$
-\frac16-\frac12+\frac23=0.
$$

It is consequently [gauge-invariant](../../../relativistic-quantum-field.md#gauge-invariance) and can supply an up-[quark](../../../standard-model.md#quark) mass.

In [unitary gauge](../../../standard-model.md#unitary-gauge), $\phi^c=((v+H)/\sqrt2,0)^T$. Writing $y_u$ for the full arbitrary coefficient of the [Yukawa coupling](../../../standard-model.md#yukawa-interaction) term, its physical form is

$$
\mathcal L_Y=-y_u(v+H)\bar u_Lu_R+\text{Hermitian conjugate},\qquad\boxed{m_u=|y_u|v.}
$$

A one-generation field rephasing makes the mass positive, and its [Higgs boson](../../../standard-model.md#higgs-boson) coupling is $m_u/v$. The printed Yukawa expression has an additional trailing $m$ after $R^+$ which is never defined. If it denotes a constant, absorb it into $y_u=f^+m$; in the conventional dimensionless Yukawa notation without that factor, $y_u=f^+$. It does not affect the gauge-transformation argument.

For three families, use a [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) of the two mass matrices: $U_{uL}^\dagger M_uU_{uR}=D_u$ and $U_{dL}^\dagger M_dU_{dR}=D_d$, with positive diagonal entries. The original left-handed weak current then becomes a current between mass eigenstates with

$$
\boxed{V_{\mathrm{CKM}}=U_{uL}^\dagger U_{dL}.}
$$

A complex $3\times3$ matrix has eighteen real parameters, and $U^\dagger U=I$ imposes nine independent real conditions, leaving nine. A generic [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) can be built from three complex plane rotations and three diagonal phases: each plane rotation supplies one angle and one phase. Thus these are three rotation angles and six phases. Rephase each of the six Dirac quark mass eigenfields, applying the same phase to its two chiralities so the diagonal masses stay real. A common phase changes no entry of $V$, leaving five effective rephasings. Removing five of the six phases leaves **three angles and one physical phase**. This [CKM parameter counting](../../../standard-model.md#ckm-parameter-counting) assumes generic nondegenerate masses; degeneracies give additional basis freedom.

Exactly massless [neutrinos](../../../standard-model.md#neutrino) have an arbitrary unitary flavor rotation that changes no mass term. After diagonalizing the charged-[lepton](../../../standard-model.md#lepton) mass matrix, choose the neutrino basis with the same left-handed rotation. The apparent lepton charged-current mixing matrix becomes the identity. Thus [mixing of exactly massless neutrinos is removable](../../../standard-model.md#mixing-of-exactly-massless-neutrinos-is-removable); it is not an analogue of physical CKM mixing.

For the requested [CP symmetry](../../../quantum-field-theory.md#cp-symmetry) calculation, write $j_{ij}^\mu=\bar u_i\gamma^\mu(1-\gamma^5)d_j$. The supplied [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) transformations, with the fermion-reordering sign, give

$$
\bar u\Gamma d\xrightarrow C\bar d\,C\Gamma^TC^{-1}u.
$$

For $\Gamma=\gamma^\mu(1-\gamma^5)$, use $C(\gamma^5)^TC^{-1}=\gamma^5$ and the given [gamma matrix](../../../algebra.md#gamma-matrices) relation to obtain

$$
j_{ij}^\mu\xrightarrow C-\bar d_j\gamma^\mu(1+\gamma^5)u_i.
$$

Under [parity](../../../quantum-mechanics.md#parity), the current acquires the Lorentz parity matrix and $1+\gamma^5$ becomes $1-\gamma^5$. Under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) the charged vector also changes sign and becomes its conjugate. The two minus signs cancel, and the parity matrices cancel in the contracted operator. Consequently

$$
O_{ij}(x)=j_{ij}^\mu(x)W_\mu(x)\xrightarrow{CP}O_{ij}^\dagger(x_P).
$$

With $k=g/(2\sqrt2)$, the interaction is $-k\sum(V_{ij}O_{ij}+V_{ij}^*O_{ij}^\dagger)$. Therefore

$$
\mathcal L_{cc}(V)\xrightarrow{CP}\mathcal L_{cc}(V^*),\qquad\mathcal L_{cc}^{CP}-\mathcal L_{cc}=2ik\sum_{ij}\operatorname{Im}V_{ij}(O_{ij}-O_{ij}^\dagger),
$$

with the transformed density evaluated at $x_P$. This is the [CP transformation of a charged quark current](../../../standard-model.md#cp-transformation-of-a-charged-quark-current).

Physical noninvariance requires a phase that cannot be removed by quark rephasings. The invariant quartet

$$
J=\operatorname{Im}(V_{ud}V_{cs}V_{us}^*V_{cd}^*)=c_{12}c_{23}c_{13}^2s_{12}s_{23}s_{13}\sin\delta
$$

is the [Jarlskog invariant](../../../standard-model.md#jarlskog-invariant), where $s_{ij}=\sin\theta_{ij}$ and $c_{ij}=\cos\theta_{ij}$ in the standard three-angle parametrization. If $J\ne0$, no allowed row/column phases can make the matrix real, and the charged-current interaction violates [CP symmetry](../../../quantum-field-theory.md#cp-symmetry). For example all three angles $\pi/4$ with $\delta=\pi/2$ give $J=1/(8\sqrt2)\ne0$.

**The printed noninvariance claim is conditional on a nonzero physical phase.** Arbitrary Yukawa matrices do not force it: $V=I$, or any real [CKM matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix), gives a CP-invariant charged-current interaction. The correct statement is generic [CP violation](../../../quantum-field-theory.md#cp-violation) when the irreducible phase is nontrivial, as explained by [quark rephasing and CP conservation](../../../standard-model.md#quark-rephasing-and-cp-conservation).

Finally a [right-handed neutrino](../../../standard-model.md#right-handed-neutrino) has gauge representation $(\mathbf1,\mathbf1)_0$. Its Lorentz-invariant same-chirality bilinear with the field obtained by [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) is therefore a [gauge singlet](../../../representation-theory.md#gauge-singlet) and permits a [Majorana mass term](../../../relativistic-quantum-field.md#majorana-mass-term), conventionally

$$
-\frac12M\,\overline{\nu_R^c}\nu_R+\text{Hermitian conjugate}.
$$

The factor $1/2$ is the usual convention for a field paired with itself; it may be absorbed into the printed coefficient. A Higgs Yukawa interaction can independently give a [Dirac mass term](../../../relativistic-quantum-field.md#dirac-mass-term). The Majorana term violates [lepton number](../../../standard-model.md#lepton-number) by two units but preserves the gauge symmetries. Corresponding terms for the other charged [Standard Model](../../../standard-model.md) [fermions](../../../quantum-mechanics.md#fermion) carry nonzero [electric charge](../../../electromagnetism.md#electric-charge), and [quarks](../../../standard-model.md#quark) also carry nontrivial [color charge](../../../standard-model.md#color-charge). Thus this [gauge-invariant right-handed neutrino Majorana mass](../../../standard-model.md#gauge-invariant-right-handed-neutrino-majorana-mass) is allowed while those charged-fermion analogues are forbidden. Merely introducing a [right-handed neutrino](../../../standard-model.md#right-handed-neutrino) permits mass; vanishing mass coefficients would still leave it massless.

## 4

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [renormalized coupling](../../../perturbative-quantum-field-theory.md#renormalized-coupling) is defined by a subtraction or reference condition at a [renormalization scale](../../../perturbative-quantum-field-theory.md#renormalization-scale) $\mu$. [Radiative corrections](../../../perturbative-quantum-field-theory.md#radiative-correction) contain logarithms of momentum scales relative to $\mu$, so changing the reference scale changes the named coupling while leaving physical observables unchanged. Holding the bare parameters fixed gives a [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics). In a fixed [renormalization scheme](../../../perturbative-quantum-field-theory.md#renormalization-scheme), with a fixed active particle content and a single coupling or a specified one-coupling approximation, [perturbation theory](../../../analysis.md#perturbation-theory) gives a power series in that coupling. Its coefficients depend on the fields, representations and scheme; beyond the universal leading coefficients they need not be scheme independent. A theory with several couplings generally has coupled beta functions, so the question's scalar equation is schematic rather than literally the form of every quantum field theory. Also $d/d\ln\mu^2=\tfrac12d/d\ln\mu$, which fixes factors of two.

For the stated leading equation let $t=\ln(\mu^2/\mu_0^2)$. Differentiating the reciprocal gives $d(1/\alpha)/dt=-b_0$, hence

$$
\boxed{\alpha(\mu^2)=\frac{\alpha_0}{1-b_0\alpha_0\ln(\mu^2/\mu_0^2)}.}
$$

For $b_0=-\beta_0<0$, define

$$
\boxed{\Lambda^2=\mu_0^2e^{-1/(\beta_0\alpha_0)}.}
$$

Then $1/\alpha=\beta_0\ln(\mu^2/\Lambda^2)$, giving

$$
\boxed{\alpha(\mu^2)=\frac1{\beta_0\ln(\mu^2/\Lambda^2)},\qquad\mu>\Lambda.}
$$

This is [one-loop running of the strong coupling](../../../perturbative-quantum-field-theory.md#one-loop-running-of-the-strong-coupling), with $\beta_0$ here normalized exactly as in the source equation. At high energy the coupling tends to zero logarithmically: [asymptotic freedom](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) makes short-distance [parton](../../../standard-model.md#parton) scattering calculable perturbatively and produces logarithmic scaling violations in [deep inelastic scattering](../../../standard-model.md#deep-inelastic-scattering) and [particle jets](../../../standard-model.md#jet-particle-physics). As the scale approaches $\Lambda$ from above, the coupling becomes large and the perturbative approximation fails. Long-distance strong physics involves [confinement](../../../standard-model.md#confinement) and [hadronization](../../../standard-model.md#hadronization), not freely propagating colored particles. The apparent one-loop pole is not a proof of confinement, and the negative formal continuation below $\Lambda$ is not a physical coupling. These are the [infrared limitations of one-loop QCD running](../../../perturbative-quantum-field-theory.md#infrared-limitations-of-one-loop-qcd-running); the [Particle Data Group QCD review](https://pdg.lbl.gov/2023/reviews/rpp2022-rev-qcd.pdf) describes the distinction between perturbative running and its nonperturbative scale.

The expected rough [QCD scale](../../../standard-model.md#qcd-scale) is **of order a few hundred MeV**, comparable to the inverse hadronic length scale $\hbar c/(1\,\mathrm{fm})\simeq0.2\,\mathrm{GeV}$. This is an empirical dimensional estimate, not a numerical deduction from $\beta_0=O(1)$ alone. Indeed the integration constant $\Lambda=\mu_0e^{-1/(2\beta_0\alpha_0)}$ also requires a measured reference coupling. Its precise value depends on flavor number, perturbative order and renormalization scheme.

For $b_0=+\beta_0$, the same integrated solution instead increases with energy and has its perturbative [Landau pole](../../../perturbative-quantum-field-theory.md#landau-pole) at

$$
\boxed{\mu_L^2=\mu_0^2e^{1/(\beta_0\alpha_0)}.}
$$

The coupling decreases toward the infrared in this approximation; toward the ultraviolet, perturbation theory ceases to be reliable before reaching the pole. For the self-coupling-dominated Higgs approximation, use the conventional [Higgs potential](../../../standard-model.md#higgs-field-potential) $V=\lambda_H(\phi^\dagger\phi-v^2/2)^2$. Then

$$
m_H^2=2\lambda_Hv^2,\qquad\alpha_H=\lambda_H/(4\pi).
$$

This quartic normalization is separate from Q1's real-triplet normalization. A very large [Higgs boson](../../../standard-model.md#higgs-boson) mass requires a large initial self-coupling, so the logarithmic distance to the pole becomes small. Requiring a weakly coupled [Standard Model](../../../standard-model.md) up to a high scale $M$ demands approximately

$$
\alpha_H(\mu_0)<\frac1{\beta_0\ln(M^2/\mu_0^2)},
$$

with a stronger practical margin to keep the evolved coupling perturbative. This is the [Higgs self-coupling Landau-pole bound](../../../perturbative-quantum-field-theory.md#higgs-self-coupling-landau-pole-bound): a sufficiently heavy Higgs would make the perturbative [Standard Model](../../../standard-model.md) unreliable well before an arbitrarily high scale. The full [Standard Model](../../../standard-model.md) [Higgs boson](../../../standard-model.md#higgs-boson) [beta function](../../../complex-analysis.md#beta-function) also includes gauge and [Yukawa coupling](../../../standard-model.md#yukawa-interaction) terms, so positivity is a self-coupling-dominated assumption, not a general sign theorem.

For the requested bottom threshold, take the physical color number $N_c=3$. In the source normalization,

$$
\beta_4=\frac{25}{12\pi},\qquad\beta_5=\frac{23}{12\pi}.
$$

Continuity of the leading coupling at $\mu=m_b$ gives

$$
\beta_5\ln\frac{m_b^2}{\Lambda_5^2}=\beta_4\ln\frac{m_b^2}{\Lambda_4^2}.
$$

Divide by $2\beta_5$ to find $\ln(m_b/\Lambda_5)=(25/23)\ln(m_b/\Lambda_4)$. Rearranging and exponentiating yields

$$
\boxed{\Lambda_5=\Lambda_4\left(\frac{m_b}{\Lambda_4}\right)^{-2/23}.}
$$

This is [matching the QCD scale across a quark threshold](../../../perturbative-quantum-field-theory.md#matching-the-qcd-scale-across-a-quark-threshold). The named integration constant changes when the beta coefficient changes; the matched coupling itself stays continuous at leading order. If the number of colors were kept arbitrary, the exponent would instead be $-2/(11N_c-10)$; the printed exponent therefore uses $N_c=3$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
