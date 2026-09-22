# Paper 45

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_45.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_45.pdf)

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

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the metric $g^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and the usual [Dirac basis](../../../algebra.md#dirac-representation-of-the-gamma-matrices), with $(\gamma^0)^\dagger=\gamma^0$ and $(\gamma^i)^\dagger=-\gamma^i$. In this solution the sign of the [chirality matrix](../../../algebra.md#chirality-matrix) is the one specified in the paper, $\gamma^5=-i\gamma^0\gamma^1\gamma^2\gamma^3$. Define $t_0=1$ and $t_i=-1$, with no summation in componentwise transformation formulas.

Complex conjugation changes the explicit $-i$ to $+i$. Three spatial [gamma matrices](../../../algebra.md#gamma-matrices) each contribute another minus sign, so

$$
B\gamma^{5*}B^{-1}=i\gamma^0(-\gamma^1)(-\gamma^2)(-\gamma^3)=-i\gamma^0\gamma^1\gamma^2\gamma^3=\boxed{\gamma^5}.
$$

Also $(\gamma^5)^2=1$ and $\{\gamma^5,\gamma^\mu\}=0$ by the [Clifford algebra](../../../algebra.md#clifford-algebra).

The [quantum time-reversal operator](../../../quantum-mechanics.md#quantum-time-reversal-operator) is [antiunitary](../../../vector-space.md#antiunitary-operator): it conjugates numerical coefficients, including the [Dirac spinors](../../../relativistic-quantum-field.md#dirac-spinor) and plane-wave exponentials in the [mode expansion of a Dirac field](../../../relativistic-quantum-field.md#mode-expansion-of-a-dirac-field). To fix the spin phase explicitly, put $\epsilon_s=(-1)^{1/2-s}$ and use

$$
\hat T b^s(p)\hat T^{-1}=\epsilon_s b^{-s}(p_T),\qquad
\hat T d^{s\dagger}(p)\hat T^{-1}=\epsilon_s d^{-s\dagger}(p_T).
$$

This convention gives $\hat T^2=-1$ on a one-fermion state, since $\epsilon_s\epsilon_{-s}=-1$. In the transformed expansion, change variables from $(p,s)$ to $(p_T,-s)$. The [Lorentz-invariant phase-space measure](../../../quantum-mechanics.md#lorentz-invariant-phase-space-measure) is unchanged, and $p_T\cdot x=-p\cdot x_T$. The coefficient of $b^s(p)e^{-ip\cdot x_T}$ is therefore

$$
\epsilon_{-s}u^{-s*}(p_T)=-\epsilon_su^{-s*}(p_T)=\gamma^5Cu^s(p).
$$

The same calculation applies to the antiparticle coefficient. Thus, with this explicitly fixed spin convention,

$$
\boxed{B=\gamma^5C,\qquad \hat T\psi(x)\hat T^{-1}=B\psi(x_T).}
$$

The [spin phase in the Dirac time-reversal matrix](../../../quantum-field-theory.md#spin-phase-in-the-dirac-time-reversal-matrix) matters here: a common change of the one-particle time-reversal phase replaces $B$ by $-B$; the phase-independent relation is $B\propto\gamma^5C$. It changes neither the defining conjugation property nor any bilinear result below. Normalize $B$ to be a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix). In the [Dirac basis](../../../algebra.md#dirac-representation-of-the-gamma-matrices), $\gamma^0$ is real and commutes with $B$, so transforming the [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) gives

$$
\hat T\bar\psi(x)\hat T^{-1}=(B\psi(x_T))^\dagger\gamma^{0*}
=\psi^\dagger(x_T)B^{-1}\gamma^0
=\boxed{\bar\psi(x_T)B^{-1}}.
$$

Here complex conjugation of the matrix defining the [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) is essential. An explicit realization consistent with the sign of $\gamma^5$ used here is $C=i\gamma^2\gamma^0$ and $B=\gamma^1\gamma^3$; it has $B^{-1}=-B$, so conjugation by $B$ and by $B^{-1}$ coincides. The usual changes of [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor) basis by [unitary matrices](../../../linear-operator-theory.md#unitary-matrix) carry the adjoint and time-reversal matrix with them.

For the [charge-conjugation matrix](../../../quantum-field-theory.md#charge-conjugation-matrix), the [gamma matrix adjoint and transpose identities](../../../algebra.md#gamma-matrix-adjoint-and-transpose-identities) give $\gamma^{\mu T}=t_\mu\gamma^{\mu*}$. Consequently $B\gamma^{\mu T}B^{-1}=\gamma^\mu$. Since $C=\gamma^5B$ in the chosen phase convention,

$$
C\gamma^{\mu T}C^{-1}=\gamma^5B\gamma^{\mu T}B^{-1}\gamma^5
=\gamma^5\gamma^\mu\gamma^5=\boxed{-\gamma^\mu}.
$$

This proof uses a temporal [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) and spatial [skew-Hermitian matrices](../../../linear-operator-theory.md#skew-hermitian-matrix) explicitly; the transpose identity is preserved when $C$ is transformed appropriately with the [gamma matrices](../../../algebra.md#gamma-matrices).

For the [Fermi interaction](../../../quantum-field-theory.md#fermi-interaction), let $V_{pn}^\mu=\bar p\gamma^\mu n$ and $A_{pn}^\mu=\bar p\gamma^\mu\gamma^5 n$. In the displayed [Dirac basis](../../../algebra.md#dirac-representation-of-the-gamma-matrices), the inverse version of the conjugation relation also holds. [Antiunitarity](../../../vector-space.md#antiunitary-operator), $B^{-1}\gamma^{\mu*}B=t_\mu\gamma^\mu$ and $B^{-1}\gamma^{5*}B=\gamma^5$ give

$$
\hat T V_{pn}^\mu(x)\hat T^{-1}=t_\mu V_{pn}^\mu(x_T),\qquad
\hat T A_{pn}^\mu(x)\hat T^{-1}=t_\mu A_{pn}^\mu(x_T).
$$

The leptonic [weak charged current](../../../standard-model.md#charged-current) has the same component signs. In the contraction of leptonic and hadronic currents, the two $t_\mu$ factors cancel. Its two independent operators thus keep their form while their coefficients become $g_V^*$ and $g_A^*$. The Hermitian-conjugate term transforms separately; its presence does not remove a relative complex phase between the vector and axial couplings.

With all intrinsic phases fixed to one and a real positive [Fermi constant](../../../quantum-field-theory.md#fermi-constant), invariance requires real coefficients in that convention. A common phase of $g_V$ and $g_A$ can instead be absorbed into a rephasing of the nucleon fields, and hence into their intrinsic time-reversal phases. The convention-independent condition, for $g_V\ne0$, is

$$
\boxed{\operatorname{Im}(g_Ag_V^*)=0,\qquad g_A/g_V\in\mathbb R.}
$$

This is the [relative weak phase condition for time reversal](../../../quantum-field-theory.md#relative-weak-phase-condition-for-time-reversal). If one coefficient vanishes, there is no relative phase to constrain; the remaining common phase can be removed. A nonreal ratio violates [time-reversal symmetry](../../../quantum-field-theory.md#t-symmetry) even though the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) includes its Hermitian conjugate.

## 2

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take $D_\mu=\partial_\mu+iK_\mu$, with the [Pauli matrices](../../../algebra.md#pauli-matrices) acting on the [Higgs doublet](../../../standard-model.md#higgs-field). For [electroweak hypercharge](../../../standard-model.md#hypercharge) $Y=1/2$,

$$
K_\mu=\frac g2\tau^aW_\mu^a+\frac{g'}2 B_\mu I_2
=\frac12\begin{pmatrix}gW_\mu^3+g'B_\mu&g(W_\mu^1-iW_\mu^2)\\g(W_\mu^1+iW_\mu^2)&-gW_\mu^3+g'B_\mu\end{pmatrix}.
$$

This specifies every component of the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) for the [electroweak interaction](../../../standard-model.md#electroweak-interaction). Expanding the [gauge-covariant kinetic term](../../../quantum-field-theory.md#gauge-covariant-kinetic-term) makes its derivative, trilinear and quartic interactions explicit:

$$
(D_\mu\phi)^\dagger D^\mu\phi=(\partial_\mu\phi)^\dagger\partial^\mu\phi
+i\big[(\partial_\mu\phi)^\dagger K^\mu\phi-\phi^\dagger K_\mu\partial^\mu\phi\big]
+\phi^\dagger K_\mu K^\mu\phi,
$$

where the [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives

$$
\phi^\dagger K_\mu K^\mu\phi=
\frac{g^2}{4}W_\mu^aW^{a\mu}\phi^\dagger\phi
+\frac{g'^2}{4}B_\mu B^\mu\phi^\dagger\phi
+\frac{gg'}2W_\mu^aB^\mu\phi^\dagger\tau^a\phi.
$$

The antisymmetric Pauli contribution vanishes because $W_\mu^aW^{b\mu}$ is symmetric in $a,b$. Reversing the sign convention for $D_\mu$ reverses the linear gauge interactions consistently, without changing the masses.

A nonzero [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) requires $\mu^2<0$. Minimizing the [Higgs potential](../../../standard-model.md#higgs-field-potential) gives $v^2=-\mu^2/\lambda$. By an [gauge transformation](../../../electromagnetism.md#gauge-transformation) choose

$$
\langle\phi\rangle=\frac1{\sqrt2}\binom0v,\qquad
\phi(x)=\frac1{\sqrt2}\binom0{v+h(x)}
$$

in [unitary gauge](../../../standard-model.md#unitary-gauge). The [electroweak doublet gauge-boson mass matrix](../../../standard-model.md#electroweak-doublet-gauge-boson-mass-matrix) follows by inserting the [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) in the [gauge-covariant kinetic term](../../../quantum-field-theory.md#gauge-covariant-kinetic-term):

$$
\mathcal L_{\mathrm{mass}}=\frac{v^2}{8}\left[g^2\big(W_\mu^1W^{1\mu}+W_\mu^2W^{2\mu}\big)+(gW_\mu^3-g'B_\mu)^2\right].
$$

Define the charged [electroweak gauge bosons](../../../standard-model.md#electroweak-gauge-boson) and the neutral rotation through the [Weinberg angle](../../../standard-model.md#weinberg-angle) by

$$
W_\mu^\pm=\frac{W_\mu^1\mp iW_\mu^2}{\sqrt2},\qquad
s_W=\frac{g'}{\sqrt{g^2+g'^2}},\quad c_W=\frac g{\sqrt{g^2+g'^2}},
$$



$$
Z_\mu=c_WW_\mu^3-s_WB_\mu,\qquad
A_\mu=s_WW_\mu^3+c_WB_\mu,
$$

with inverse $W_\mu^3=c_WZ_\mu+s_WA_\mu$ and $B_\mu=-s_WZ_\mu+c_WA_\mu$. Then

$$
\mathcal L_{\mathrm{mass}}=m_W^2W_\mu^+W^{-\mu}+\frac12m_Z^2 Z_\mu Z^\mu,
\qquad
\boxed{m_W=\frac{gv}{2},\quad m_Z=\frac{v\sqrt{g^2+g'^2}}2,\quad m_A=0.}
$$

The factors differ because $W^+$ and $W^-$ are conjugate fields whereas $Z$ is real. The massless [photon](../../../quantum-mechanics.md#photon) corresponds to the unbroken [Lie algebra generator](../../../lie-algebra.md#lie-algebra-generator) $Q=T_3+Y$, which annihilates $\langle\phi\rangle$. Thus three of the four real [gauge bosons](../../../relativistic-quantum-field.md#gauge-boson) acquire mass, with $m_W=m_Zc_W$. The three would-be [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson) provide their longitudinal polarizations; the remaining scalar $h$ is the [Higgs boson](../../../standard-model.md#higgs-boson).

Introduce the left-handed [lepton](../../../standard-model.md#lepton) doublet $L=(\nu_{eL},e_L)^T$, with $Y_L=-1/2$, and the right-handed singlet $e_R$, with $Y_R=-1$. Use the [chiral projectors](../../../relativistic-quantum-field.md#chiral-projector) $P_L=(1-\gamma^5)/2$ and $P_R=(1+\gamma^5)/2$ in the course's convention. The minimal [Standard Model](../../../standard-model.md) has no right-handed neutrino. The [gauge-invariant](../../../relativistic-quantum-field.md#gauge-invariance) fermion terms are

$$
\mathcal L_{\ell}=\bar L i\gamma^\mu\left(\partial_\mu+i\frac g2\tau^aW_\mu^a-i\frac{g'}2B_\mu\right)L
+\bar e_Ri\gamma^\mu(\partial_\mu-ig'B_\mu)e_R
-\left(y_e\bar L\phi e_R+y_e^*\bar e_R\phi^\dagger L\right).
$$

The doublet contraction in the [Yukawa interaction](../../../standard-model.md#yukawa-interaction) is a singlet, and its total [hypercharge](../../../standard-model.md#hypercharge) is $+1/2+1/2-1=0$. A bare term $\bar e_Le_R$ would fail [electroweak gauge invariance](../../../standard-model.md#electroweak-gauge-invariance). The [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative) above already give all the requested fermion-gauge couplings. In terms of mass eigenstates, $e=gs_W=g'c_W$ and they become

$$
\mathcal L_{\mathrm{CC}}=-\frac g{\sqrt2}\left(W_\mu^+\bar\nu_{eL}\gamma^\mu e_L+W_\mu^-\bar e_L\gamma^\mu\nu_{eL}\right),\qquad
\mathcal L_{\mathrm{em}}=+eA_\mu\bar e\gamma^\mu e,
$$



$$
\mathcal L_Z=-\frac g{c_W}Z_\mu\left[\frac12\bar\nu_{eL}\gamma^\mu\nu_{eL}
+\left(-\frac12+s_W^2\right)\bar e_L\gamma^\mu e_L+s_W^2\bar e_R\gamma^\mu e_R\right].
$$

Thus the [weak charged current](../../../standard-model.md#charged-current) is chiral and the neutrino has zero [electric charge](../../../electromagnetism.md#electric-charge). The [gauge-invariant electron Yukawa mass](../../../standard-model.md#gauge-invariant-electron-yukawa-mass) follows from the [Yukawa interaction](../../../standard-model.md#yukawa-interaction) after [electroweak symmetry breaking](../../../standard-model.md#electroweak-symmetry-breaking):

$$
-\frac{v+h}{\sqrt2}\left(y_e\bar e_Le_R+y_e^*\bar e_Re_L\right).
$$

Rephase $e_R$ to make $y_e$ real and positive. It gives

$$
\boxed{m_e=\frac{|y_e|v}{\sqrt2},\qquad \mathcal L_{e,h}=-m_e\bar ee-\frac{m_e}{v}h\bar ee.}
$$

The electron [Dirac mass](../../../relativistic-quantum-field.md#dirac-mass-term) is therefore compatible with the original [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance) through the [Higgs mechanism](../../../standard-model.md#higgs-mechanism). The neutrino remains massless in this minimal renormalizable lepton sector.

## 3

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The strong-interaction matrix element between two spin-zero [pseudoscalar mesons](../../../physics.md#pseudoscalar-meson) has only $p^\mu$ and $k^\mu$ available. The product of the two intrinsic [parities](../../../quantum-mechanics.md#parity) is positive. An [axial current](../../../relativistic-quantum-field.md#axial-current) would require a [pseudovector](../../../vector-space.md#pseudovector) constructed from these momenta, but an expression involving the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) needs three independent four-vectors and therefore vanishes. This is a consequence of [parity conservation](../../../quantum-mechanics.md#parity-conservation) in the hadronic matrix element, not of parity conservation in the weak interaction. The [vector current](../../../relativistic-quantum-field.md#vector-current) can have the two independent structures $p+k$ and $p-k$. Its coefficients are [Lorentz scalars](../../../special-relativity.md#lorentz-scalar); with $p^2=m_K^2$ and $k^2=m_\pi^2$ fixed, their only varying invariant is $s=q^2$. Hence

$$
H^\mu=\langle\pi^+(k)|\bar u\gamma^\mu s|\bar K^0(p)\rangle
=(p+k)^\mu f_+(s)+q^\mu f_-(s).
$$

These are the [pseudoscalar-to-pseudoscalar form factors](../../../physics.md#pseudoscalar-to-pseudoscalar-form-factor). With relativistically normalized states they are dimensionless. The vanishing axial matrix element and this decomposition explain the two equalities separately.

Write $q_1$ and $q_2$ for the outgoing electron and antineutrino momenta. From the [Fermi interaction](../../../quantum-field-theory.md#fermi-interaction), an invariant [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude), up to an irrelevant overall sign or phase, is

$$
\mathcal M=\frac{G_FV_{us}}{\sqrt2}\,
\bar u(q_1)\gamma_\mu(1-\gamma^5)v(q_2)
\left[(p+k)^\mu f_+(s)+q^\mu f_-(s)\right].
$$

The [CKM matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) element $V_{us}$ multiplies the quark current in the convention of this interaction. Let $\ell_\mu=\bar u(q_1)\gamma_\mu(1-\gamma^5)v(q_2)$. For massless leptons, the [massless Dirac equation](../../../relativistic-quantum-field.md#massless-dirac-equation) and [chirality matrix](../../../algebra.md#chirality-matrix) anticommutation give

$$
q^\mu\ell_\mu=\bar u(q_1)(\not q_1+\not q_2)(1-\gamma^5)v(q_2)=0.
$$

In the second term move $\not q_2$ through the [chiral projector](../../../relativistic-quantum-field.md#chiral-projector) before applying $\not q_2v=0$. Since $p+k=2p-q$, this [transverse massless leptonic current](../../../standard-model.md#transverse-massless-leptonic-current) gives

$$
\boxed{\mathcal M=\sqrt2\,G_FV_{us}f_+(s)\,p^\mu\ell_\mu.}
$$

The disappearance of $f_-$ uses the massless approximation; for a massive charged lepton its contraction is proportional to the lepton mass.

Use the [fermion spin sum](../../../relativistic-quantum-field.md#fermion-spin-sum) and the supplied [gamma matrix trace identities](../../../algebra.md#gamma-matrix-trace-identities). The symmetric part of the [leptonic tensor](../../../standard-model.md#leptonic-tensor) is

$$
L_{\mu\nu}=8\left(q_{1\mu}q_{2\nu}+q_{1\nu}q_{2\mu}-g_{\mu\nu}q_1\cdot q_2\right)+L_{\mu\nu}^{\mathrm{antisym}}.
$$

The [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) term is antisymmetric and drops out when contracted with $p^\mu p^\nu$. Thus

$$
\sum_{\mathrm{spins}}|\mathcal M|^2=16G_F^2|V_{us}|^2|f_+(s)|^2
\left[2(p\cdot q_1)(p\cdot q_2)-m_K^2(q_1\cdot q_2)\right].
$$

There is no initial-spin average because the kaon is spinless. For the [integrated massless leptonic tensor](../../../standard-model.md#integrated-massless-leptonic-tensor), keep every factor of $2\pi$ explicit and define the unnormalized two-lepton [Lorentz-invariant phase space](../../../relativistic-quantum-field.md#lorentz-invariant-phase-space)

$$
I_{\mu\nu}=\int\frac{d^3q_1}{q_1^0}\frac{d^3q_2}{q_2^0}
\delta^{(4)}(q-q_1-q_2)q_{1\mu}q_{2\nu}
=\frac\pi3 q_\mu q_\nu+\frac\pi6 g_{\mu\nu}s.
$$

The leptons are massless, so $q_i^0=|\boldsymbol q_i|$. Its trace is $g^{\mu\nu}I_{\mu\nu}=\pi s$. Therefore

$$
2p^\mu p^\nu I_{\mu\nu}-m_K^2g^{\mu\nu}I_{\mu\nu}
=\frac{2\pi}{3}\left[(p\cdot q)^2-m_K^2s\right].
$$

The three [Lorentz-invariant phase-space measures](../../../quantum-mechanics.md#lorentz-invariant-phase-space-measure) and their momentum delta function contribute $1/[8(2\pi)^5]$, in addition to $1/(2m_K)$ in the [decay rate](../../../relativistic-quantum-field.md#decay-width). Combining them with the spin sum gives

$$
\boxed{\Gamma=\frac{G_F^2|V_{us}|^2}{48\pi^4m_K}
\int\frac{d^3k}{k^0}\left[(p\cdot q)^2-m_K^2q^2\right]|f_+(q^2)|^2,\quad
A=\frac{G_F^2|V_{us}|^2}{48\pi^4m_K}.}
$$

This [massless semileptonic pseudoscalar decay rate](../../../relativistic-quantum-field.md#massless-semileptonic-pseudoscalar-decay-rate) uses a two-lepton integral over future-timelike $q$ and the pion integral is restricted to the physically allowed region. The null endpoint follows by continuity. The coefficient has mass dimension $-5$, so the complete expression has mass dimension one, as a [decay rate](../../../relativistic-quantum-field.md#decay-width) must in natural units.

In the kaon [centre-of-momentum frame](../../../special-relativity.md#center-of-momentum-frame), put $E=k^0$ and $\kappa=|\boldsymbol k|$. Then

$$
s=m_K^2+m_\pi^2-2m_KE,\qquad
(p\cdot q)^2-m_K^2s=m_K^2(E^2-m_\pi^2)=m_K^2\kappa^2.
$$

The dimensionally consistent [Källén function](../../../special-relativity.md#kallen-function) is

$$
\lambda(s,m_K^2,m_\pi^2)=s^2+m_K^4+m_\pi^4-2sm_K^2-2sm_\pi^2-2m_K^2m_\pi^2,
\qquad \kappa=\frac{\sqrt\lambda}{2m_K}.
$$

The pion-only mass term must have fourth power: the second power printed in the PDF is dimensionally inconsistent. This repair also follows directly from squaring $E=(m_K^2+m_\pi^2-s)/(2m_K)$. Angular integration and the change of variable give

$$
\frac{d^3k}{k^0}=4\pi\frac{\kappa^2}{E}\,d\kappa
=-\frac{2\pi\kappa}{m_K}\,ds
=-\frac{\pi\sqrt\lambda}{m_K^2}\,ds,
$$

where the negative sign reverses the endpoints. Combining this with the bracket $\lambda/4$ yields

$$
\boxed{\Gamma=\frac{G_F^2|V_{us}|^2}{192\pi^3m_K^3}
\int_0^{(m_K-m_\pi)^2} ds\,\lambda(s,m_K^2,m_\pi^2)^{3/2}|f_+(s)|^2.}
$$

Thus $\boxed{B=G_F^2|V_{us}|^2/(192\pi^3m_K^3),\ a=0,\ b=(m_K-m_\pi)^2}$. The lower limit is the minimum invariant mass of two massless leptons; at the upper limit the pion is at rest. The coefficient has mass dimension $-7$, while $ds\,\lambda^{3/2}$ has dimension eight. The [Källén function](../../../special-relativity.md#kallen-function) also shows why the differential [decay rate](../../../relativistic-quantum-field.md#decay-width) vanishes at zero pion momentum.

## 4

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

At one loop, writing $t=\log\mu$ makes the [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) $dg_i/dt=b_i g_i^3$. For $b_i>0$ a positive [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling) grows towards high energies and decreases towards the infrared. Extrapolation of the one-loop expression gives a finite ultraviolet [Landau pole](../../../perturbative-quantum-field-theory.md#landau-pole); perturbation theory fails before it reaches that pole. For $b_i<0$, the coupling decreases towards high energies, giving [asymptotic freedom](../../../perturbative-quantum-field-theory.md#asymptotic-freedom), and grows towards the infrared. The formal infrared pole identifies a [strong-coupling scale](../../../perturbative-quantum-field-theory.md#strong-coupling-scale), where the weak-coupling approximation no longer applies. These conclusions concern the small-coupling branch; a pole in the perturbative solution does not establish a pole in the exact theory. If $b_i=0$, higher-order terms decide the running.

From $\alpha_i=g_i^2/(4\pi)$,

$$
\frac{d\alpha_i}{d\log\mu}=8\pi b_i\alpha_i^2,
\qquad \frac{d\alpha_i^{-1}}{d\log\mu}=-8\pi b_i.
$$

Integrating the one-loop [beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) gives

$$
\boxed{\alpha_i^{-1}(\mu)=\alpha_i^{-1}(m_Z)-8\pi b_i\log\frac\mu{m_Z},\qquad
\alpha_i(\mu)=\frac{\alpha_i(m_Z)}{1-8\pi b_i\alpha_i(m_Z)\log(\mu/m_Z)}.}
$$

These formulas retain the same particle content and neglect threshold corrections throughout the interval. For $b_i>0$, the formal pole is $\mu=m_Z\exp[1/(8\pi b_i\alpha_i(m_Z))]$; for $b_i<0$ the analogous scale lies below $m_Z$.

For [one-loop normalized hypercharge unification](../../../perturbative-quantum-field-theory.md#one-loop-normalized-hypercharge-unification), the normalized hypercharge coupling is $\alpha_Y^{\mathrm{GUT}}=(5/3)\alpha_1$, so its inverse and one-loop slope are $(3/5)\alpha_1^{-1}$ and $(3/5)b_1$. Define

$$
U_1=\frac35\alpha_1^{-1}(m_Z),\quad U_2=\alpha_2^{-1}(m_Z),\quad U_3=\alpha_3^{-1}(m_Z),\quad
L_G=\log\frac{M_{\mathrm{GUT}}}{m_Z}.
$$

Equality of the three normalized inverses at the unification scale gives

$$
U_1-U_2=8\pi\left(\frac35b_1-b_2\right)L_G,\qquad
U_3-U_2=8\pi(b_3-b_2)L_G.
$$

Eliminating $L_G$ proves

$$
\boxed{\alpha_3^{-1}(m_Z)=\alpha_2^{-1}(m_Z)+
\frac{b_3-b_2}{(3/5)b_1-b_2}
\left[\frac35\alpha_1^{-1}(m_Z)-\alpha_2^{-1}(m_Z)\right].}
$$

This expression assumes $(3/5)b_1\ne b_2$. If these slopes coincide, unification first requires $U_1=U_2$, and the displayed division is unavailable. A unification scale above $m_Z$ additionally requires the inferred $L_G$ to be positive. The relation is a consistency condition under the stated one-loop assumptions, not proof that the measured couplings unify without threshold effects.

For the two-loop [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling), the claimed logarithmic asymptotic concerns the [asymptotically free](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) branch with $\beta_0>0$ and $\mu/\Lambda\to\infty$. Set

$$
y=a^{-1},\qquad c=\frac{\beta_1}{\beta_0},\qquad L=\log\frac\mu\Lambda.
$$

The differential equation becomes $dy/dL=\beta_0+\beta_1/y=\beta_0(1+c/y)$. Separating variables yields

$$
y-c\log|y+c|=\beta_0L+K.
$$

A change of the [strong-coupling scale](../../../perturbative-quantum-field-theory.md#strong-coupling-scale) $\Lambda$ absorbs any additive constant $K$. Choose that scale so that $K=-c\log\beta_0$. On the large positive-$y$ branch the exact implicit relation is then

$$
y-c\log\frac{y+c}{\beta_0}=\beta_0L.
$$

It first gives $y\sim\beta_0L$. Substituting this back into the logarithm gives $y=\beta_0L+c\log L+o(1)$. To determine the error rather than assume it, write $y=\beta_0L+c\log L+r(L)$. Expansion of the exact implicit relation yields

$$
r(L)=\frac{c\,[c\log L+c+r(L)]}{\beta_0L}
+O\!\left(\frac{(\log L)^2}{L^2}\right)
=\frac{c^2}{\beta_0}\frac{\log L+1}{L}
+O\!\left(\frac{(\log L)^2}{L^2}\right).
$$

Consequently the mathematically correct two-loop asymptotic is

$$
\boxed{a^{-1}(\mu)=\beta_0L+\frac{\beta_1}{\beta_0}\log L
+O\!\left(\frac{\log L}{L}\right).}
$$

More precisely, the next term is $\boxed{\beta_1^2(\log L+1)/(\beta_0^3L)}$. For $\beta_1\ne0$ this is not $O(1/L)$: multiplying the remainder by $L$ makes it grow as $(\beta_1^2/\beta_0^3)\log L$. No fixed change of $\Lambda$ can remove this term. Such a change adds a constant to $L$ and changes only constant or $1/L$ contributions, rather than the coefficient of $\log L/L$. Thus the two leading terms requested are correct, but the literal remainder printed in the PDF is too small. This is the [two-loop inverse-coupling logarithmic remainder](../../../perturbative-quantum-field-theory.md#two-loop-inverse-coupling-logarithmic-remainder).

If $\beta_1=0$, the one-loop result $y=\beta_0L$ is exact after choosing $\Lambda$. If $\beta_0=0$, the displayed expansion is undefined and the differential equation instead gives $y^2=2\beta_1\log\mu+\text{constant}$. For $\beta_0<0$, a positive weak coupling does not approach zero at arbitrarily large $\mu$ along the branch used above. The asymptotic assumptions therefore matter as well as the remainder.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
