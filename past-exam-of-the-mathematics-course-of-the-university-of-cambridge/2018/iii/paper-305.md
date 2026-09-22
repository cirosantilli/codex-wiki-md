# Paper 305

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_305.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_305.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $g^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ throughout. Taking the [Hermitian conjugation](../../../hilbert-space.md#hermitian-conjugation) of the massive [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) and using the [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) gives

$$
i(\partial_\mu\bar\psi)\gamma^\mu+m\bar\psi=0.
$$

Taking the [matrix transpose](../../../vector-space.md#transpose) and multiplying by the [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) matrix $C$ yields

$$
iC\gamma^{\mu T}C^{-1}\partial_\mu(C\bar\psi^T)+mC\bar\psi^T=0,
\qquad
-i\gamma^\mu\partial_\mu\psi^c+m\psi^c=0.
$$

Thus the [charge conjugation of a Dirac field](../../../quantum-field-theory.md#charge-conjugation-of-a-dirac-field) preserves the free massive [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation):

$$
\boxed{(i\gamma^\mu\partial_\mu-m)\psi^c=0.}
$$

The [unitarity](../../../vector-space.md#unitary-operator) of $C$ and $\gamma^0C^{-1}\gamma^0=-C^{-1}\gamma^{0T}$ also give

$$
\overline{\psi^c}=(C\bar\psi^T)^\dagger\gamma^0
=\psi^T\gamma^{0T}C^{-1}\gamma^0=-\psi^TC^{-1}.
$$

Consequently

$$
\boxed{\hat C\bar\psi(x)\hat C^{-1}=-\psi^T(x)C^{-1}.}
$$

Here $\hat C$ is the [unitary operator](../../../vector-space.md#unitary-operator) acting on the [relativistic quantum field](../../../relativistic-quantum-field.md), whereas $C$ acts on [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor) indices.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [bosonic annihilation operator](../../../quantum-mechanics.md#bosonic-annihilation-operator) $a^\lambda(p)$ removes a vector particle of [four-momentum](../../../special-relativity.md#four-momentum) $p$ and [polarization vector](../../../relativistic-quantum-field.md#polarization-vector) $\varepsilon^{\mu,\lambda}(p)$. The [bosonic creation operator](../../../quantum-mechanics.md#bosonic-creation-operator) $c^{\lambda\dagger}(p)$ creates its [antiparticle](../../../relativistic-quantum-field.md#antiparticle) with the same [four-momentum](../../../special-relativity.md#four-momentum) and polarization label. The [polarization vector](../../../relativistic-quantum-field.md#polarization-vector) describes the corresponding spin-one [mode expansion of a free field](../../../quantum-field-theory.md#mode-expansion-of-a-free-field).

Because [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) acts through a [unitary operator](../../../vector-space.md#unitary-operator), it leaves the numerical [polarization vector](../../../relativistic-quantum-field.md#polarization-vector) coefficients unchanged. Applying the specified [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) to the operators gives

$$
\hat C V^\mu(x)\hat C^{-1}
=\eta_C\sum_{p,\lambda}\left[\varepsilon^{\mu,\lambda}(p)c^\lambda(p)e^{-ip\cdot x}+\varepsilon^{\mu,\lambda *}(p)a^{\lambda\dagger}(p)e^{ip\cdot x}\right].
$$

Comparison with the [Hermitian conjugation](../../../hilbert-space.md#hermitian-conjugation) of the original expansion therefore gives

$$
\boxed{\hat C V^\mu(x)\hat C^{-1}=\eta_C V^{\mu\dagger}(x).}
$$

The factor $\eta_C$ is the [intrinsic charge-conjugation phase](../../../quantum-field-theory.md#intrinsic-charge-conjugation-phase).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) of a [fermion bilinear](../../../relativistic-quantum-field.md#fermion-bilinear), the result of part (a) and the [fermionic sign](../../../perturbative-quantum-field-theory.md#fermionic-sign) from interchanging the fields give

$$
\hat C(\bar\psi\Gamma\psi)\hat C^{-1}
=-\psi^T C^{-1}\Gamma C\bar\psi^T
=\bar\psi(C^{-1}\Gamma C)^T\psi.
$$

For the [Dirac current](../../../quantum-field-theory.md#dirac-current), $(C^{-1}\gamma^\mu C)^T=-\gamma^\mu$. For the [axial current](../../../relativistic-quantum-field.md#axial-current), the definition of $\gamma^5$ and the [gamma matrix](../../../algebra.md#gamma-matrices) identities imply

$$
C^{-1}\gamma^5C=\gamma^{5T},\qquad
(C^{-1}\gamma^\mu\gamma^5C)^T
=-\gamma^5\gamma^\mu=\gamma^\mu\gamma^5.
$$

Thus the [charge conjugation of fermion bilinears](../../../quantum-field-theory.md#charge-conjugation-of-fermion-bilinears) gives

$$
\boxed{\hat C(\bar\psi\gamma^\mu\psi)\hat C^{-1}=-\bar\psi\gamma^\mu\psi,\qquad
\hat C(\bar\psi\gamma^\mu\gamma^5\psi)\hat C^{-1}=+\bar\psi\gamma^\mu\gamma^5\psi.}
$$

The [Dirac current](../../../quantum-field-theory.md#dirac-current) is **odd under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation)**, and the [axial current](../../../relativistic-quantum-field.md#axial-current) is **even under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation)**. The [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) specifies the usual treatment of coincident-field contact terms.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For a real vector [relativistic quantum field](../../../relativistic-quantum-field.md), $V^\mu=V^{\mu\dagger}$. Its transformed field must also be a [Hermitian operator](../../../hilbert-space.md#hermitian-operator), so the [intrinsic charge-conjugation phase](../../../quantum-field-theory.md#intrinsic-charge-conjugation-phase) satisfies $\eta_C=\eta_C^*$; combined with $|\eta_C|=1$, this gives

$$
\boxed{\eta_C=\pm1.}
$$

The [quantum electrodynamics](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics) interaction is $-e\bar\psi\gamma^\mu\psi A_\mu$. Since the [Dirac electromagnetic current](../../../quantum-field-theory.md#dirac-electromagnetic-current) is odd under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) invariance of this interaction requires the [photon](../../../quantum-mechanics.md#photon) field to be odd too:

$$
\boxed{\eta_C(A)=-1,\qquad \hat C A^\mu\hat C^{-1}=-A^\mu.}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Write $J_V^\mu=\bar\psi\gamma^\mu\psi$ for the [Dirac current](../../../quantum-field-theory.md#dirac-current) and $J_A^\mu=\bar\psi\gamma^\mu\gamma^5\psi$ for the [axial current](../../../relativistic-quantum-field.md#axial-current). Under [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory), the [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor) phases cancel and

$$
\hat P J_V^\mu(x)\hat P^{-1}=\mathbb P^\mu{}_{\nu}J_V^\nu(x_P),\qquad
\hat P J_A^\mu(x)\hat P^{-1}=-\mathbb P^\mu{}_{\nu}J_A^\nu(x_P).
$$

The extra sign for the [axial current](../../../relativistic-quantum-field.md#axial-current) follows from $\gamma^0\gamma^5\gamma^0=-\gamma^5$. Combining these transformations with part (c), both currents transform under [CP symmetry](../../../quantum-field-theory.md#cp-symmetry) as $J_{V,A}^\mu(x)\mapsto-\mathbb P^\mu{}_{\nu}J_{V,A}^\nu(x_P)$. The vector [relativistic quantum field](../../../relativistic-quantum-field.md) transforms as $V^\mu(x)\mapsto\eta_C\mathbb P^\mu{}_{\nu}V^{\nu\dagger}(x_P)$. The two parity matrices cancel in the [tensor contraction](../../../linear-algebra.md#tensor-contraction), giving

$$
\boxed{(\widehat{CP})\left[\bar\psi\gamma^\mu(g_v-g_a\gamma^5)\psi V_\mu\right](x)(\widehat{CP})^{-1}
=-\eta_C\left[\bar\psi\gamma^\mu(g_v-g_a\gamma^5)\psi\right](x_P)V_\mu^\dagger(x_P).}
$$

For a real vector [relativistic quantum field](../../../relativistic-quantum-field.md) with $\eta_C=-1$, the interaction is **invariant under [CP symmetry](../../../quantum-field-theory.md#cp-symmetry)**. A complex vector [relativistic quantum field](../../../relativistic-quantum-field.md) instead maps to the conjugate-field interaction, which must be compared with its [Hermitian conjugation](../../../hilbert-space.md#hermitian-conjugation) partner.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The flavour-diagonal [weak neutral current](../../../standard-model.md#neutral-current) coupled to the real [Z boson](../../../standard-model.md#z-boson) has real vector and [axial current](../../../relativistic-quantum-field.md#axial-current) couplings. With $\eta_C(Z)=-1$, part (e) shows that this tree-level interaction is **invariant under [CP symmetry](../../../quantum-field-theory.md#cp-symmetry)**, although the simultaneous presence of the [Dirac current](../../../quantum-field-theory.md#dirac-current) and [axial current](../../../relativistic-quantum-field.md#axial-current) generally violates [charge conjugation](../../../quantum-field-theory.md#charge-conjugation) and [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory) separately. This conclusion concerns the tree-level [weak neutral current](../../../standard-model.md#neutral-current), rather than every interaction or radiative effect in the [Standard Model](../../../standard-model.md).

The [weak charged current](../../../standard-model.md#charged-current) couples distinct [quark](../../../standard-model.md#quark) flavours and involves the [Cabibbo-Kobayashi-Maskawa matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix):

$$
\mathcal L_{\rm cc}=-\frac{g}{\sqrt2}\bar u_{Li}\gamma^\mu V_{ij}d_{Lj}W_\mu^++\text{h.c.}
$$

Here $u_{Li}$ and $d_{Lj}$ are [left-handed](../../../relativistic-quantum-field.md#chirality-physics) [quark](../../../standard-model.md#quark) fields. A [CP symmetry](../../../quantum-field-theory.md#cp-symmetry) transformation exchanges the two conjugate-field operators; because it acts through a [unitary operator](../../../vector-space.md#unitary-operator), it does not complex-conjugate their numerical coefficients. Equality with the original interaction therefore requires a [Cabibbo-Kobayashi-Maskawa matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) that can be made real by [quantum field rephasings](../../../quantum-field-theory.md#quantum-field-rephasing). With three generations, a physical [CP-violating phase](../../../quantum-field-theory.md#cp-violating-phase) remains in general, measured by the [Jarlskog invariant](../../../standard-model.md#jarlskog-invariant). Therefore the [W boson](../../../standard-model.md#w-boson) interactions **can violate [CP symmetry](../../../quantum-field-theory.md#cp-symmetry)**. Merely seeing a complex coefficient is insufficient: the phase must survive [quantum field rephasing](../../../quantum-field-theory.md#quantum-field-rephasing), unlike the real two-generation [Cabibbo angle](../../../standard-model.md#cabibbo-angle) rotation.

## 2

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [scalar potential](../../../quantum-field-theory.md#scalar-potential) can be written as

$$
V=\frac{\lambda}{4}(\phi_a\phi_a-v^2)^2-\frac{\lambda v^4}{4},\qquad v^2=-\frac{m^2}{\lambda}.
$$

Its [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) is the sphere $\phi_a\phi_a=v^2$. The [Adjoint double cover from SU(2) to SO(3)](../../../lie-theory.md#adjoint-double-cover-from-su-2-to-so-3) rotates any nonzero [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) to $(0,0,v)$, with $v>0$. A local [unitary gauge](../../../standard-model.md#unitary-gauge) removes the two angular fluctuations, leaving $\phi=(0,0,v+\eta)$. This choice holds in a neighbourhood of the nonzero vacuum; a single global rotation cannot align arbitrary position-dependent fields, and topologically nontrivial configurations can obstruct a global [unitary gauge](../../../standard-model.md#unitary-gauge).

The generator $t^3$ fixes the [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value), while $t^1,t^2$ do not. Thus the [Higgs mechanism](../../../standard-model.md#higgs-mechanism) in this [SU(2) gauge theory with an adjoint Higgs field](../../../relativistic-quantum-field.md#su-2-gauge-theory-with-an-adjoint-higgs-field) gives

$$
\boxed{SU(2)\longrightarrow U(1).}
$$

The two angular [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson) become the longitudinal polarizations of two massive [gauge bosons](../../../relativistic-quantum-field.md#gauge-boson). Define physical fields

$$
A_\mu=B^3_\mu,\qquad W_\mu^\pm=\frac{B_\mu^1\mp iB_\mu^2}{\sqrt2}.
$$

These labels describe the fields of this model; they do not identify it with the [Standard Model](../../../standard-model.md). With the stated [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative),

$$
(D_\mu\phi)_1=-g(v+\eta)B_\mu^2,\quad (D_\mu\phi)_2=g(v+\eta)B_\mu^1,\quad (D_\mu\phi)_3=\partial_\mu\eta.
$$

To express all [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) terms in physical fields, introduce the [gauge field strengths](../../../relativistic-quantum-field.md#gauge-field-strength)

$$
f_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu,\quad
Q_{\mu\nu}=W_\mu^+W_\nu^--W_\nu^+W_\mu^-,\quad
\mathcal W^\pm_{\mu\nu}=(\partial_\mu\pm igA_\mu)W_\nu^\pm-(\partial_\nu\pm igA_\nu)W_\mu^\pm.
$$

Then $F^3_{\mu\nu}=f_{\mu\nu}+igQ_{\mu\nu}$ and $(F^1_{\mu\nu}\mp iF^2_{\mu\nu})/\sqrt2=\mathcal W^\pm_{\mu\nu}$. Dropping the constant vacuum energy, the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) is

$$
\begin{aligned}
\mathcal L={}&-\frac14(f_{\mu\nu}+igQ_{\mu\nu})(f^{\mu\nu}+igQ^{\mu\nu})-\frac12\mathcal W^+_{\mu\nu}\mathcal W^{-\mu\nu}
+\frac12\partial_\mu\eta\partial^\mu\eta\\
&-\lambda v^2\eta^2-\lambda v\eta^3-\frac\lambda4\eta^4+g^2(v+\eta)^2W_\mu^+W^{-\mu}.
\end{aligned}
$$

Taking the positive [gauge coupling](../../../relativistic-quantum-field.md#gauge-coupling) convention $g>0$, the canonically normalized [mass terms](../../../quantum-field-theory.md#mass-term) give

$$
\boxed{m_A=0,\qquad m_{W^+}=m_{W^-}=gv,\qquad m_\eta^2=2\lambda v^2=-2m^2.}
$$

The residual [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry) makes $W^\pm$ oppositely charged. The [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) terms supply interactions of $A$ with $W^\pm$ and four-vector interactions. The [Higgs mode](../../../quantum-field-theory.md#higgs-mode) has cubic and quartic self-interactions, together with $2g^2v\eta W^+\cdot W^-$ and $g^2\eta^2W^+\cdot W^-$ couplings; it is neutral under the surviving [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry).

Coupling [fermions](../../../quantum-mechanics.md#fermion) permits a massless electromagnetic [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) and massive charged mediators of the [weak interaction](../../../standard-model.md#weak-interaction); [fermion](../../../quantum-mechanics.md#fermion) couplings with [chirality](../../../relativistic-quantum-field.md#chirality-physics) can produce parity-violating [weak charged currents](../../../standard-model.md#charged-current). However, this model has **no massive neutral [Z boson](../../../standard-model.md#z-boson)**, and its only charge generator is $t^3$. A fundamental doublet has opposite charges, so it cannot reproduce the observed doublet charge assignments through an independent [hypercharge](../../../standard-model.md#hypercharge). The [Standard Model](../../../standard-model.md) instead has $SU(2)_L\times U(1)_Y\to U(1)_Q$, a complex [Higgs doublet](../../../standard-model.md#higgs-field), three absorbed [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson), a massive [Z boson](../../../standard-model.md#z-boson) and a [weak mixing angle](../../../standard-model.md#weinberg-angle).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

In the matrix expression, $t^a=\lambda^a/2$ denotes a fundamental generator, whereas the component [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative) uses adjoint generators. With $\operatorname{Tr}(t^dt^h)=\delta^{dh}/2$,

$$
[t^a,\Phi]=if^{acd}\phi_ct^d,\qquad
-g^2\operatorname{Tr}([t^a,\Phi][t^b,\Phi])B_\mu^aB^{b\mu}
=\frac{g^2}{2}f^{acd}f^{bed}\phi_c\phi_eB_\mu^aB^{b\mu}.
$$

Using antisymmetry to write $f^{acd}=f^{dac}$ and $f^{bed}=f^{dbe}$ gives exactly the component [mass term](../../../quantum-field-theory.md#mass-term). This is the [gauge-boson mass matrix from an adjoint scalar](../../../standard-model.md#gauge-boson-mass-matrix-from-an-adjoint-scalar).

For $\Phi_0=v\operatorname{diag}(1,1,-2)$, the [Gell-Mann matrices](../../../algebra.md#gell-mann-matrices) $t^1,t^2,t^3,t^8$ commute with $\Phi_0$. Their [gauge bosons](../../../relativistic-quantum-field.md#gauge-boson) are therefore massless. The generators $t^4,t^5,t^6,t^7$ connect the first two [eigenspaces](../../../linear-operator-theory.md#eigenspace) to the third; the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) difference is $3v$. Directly taking the [matrix trace](../../../linear-algebra.md#matrix-trace) gives

$$
\operatorname{Tr}([t^a,\Phi_0][t^b,\Phi_0])=-\frac{9v^2}{2}\delta^{ab},\qquad a,b\in\{4,5,6,7\},
$$

with all remaining entries zero. Thus

$$
\mathcal L_{\rm mass}=\frac{9g^2v^2}{2}\sum_{a=4}^7 B_\mu^aB^{a\mu},\qquad
\boxed{m_{1,2,3,8}=0,\qquad m_{4,5,6,7}=3g|v|.}
$$

The factor $1/2$ is the canonical real-vector [mass term](../../../quantum-field-theory.md#mass-term) normalization. The unbroken [Lie algebra](../../../lie-algebra.md) is $\mathfrak{su}(2)\oplus\mathfrak u(1)$, giving the usual description **SU(2) × U(1)**. More precisely, the [centralizer](../../../group-theory.md#centralizer) of the [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) inside $SU(3)$ is

$$
\boxed{S(U(2)\times U(1))\simeq (SU(2)\times U(1))/\mathbb Z_2.}
$$

This global quotient refines the [adjoint-Higgs breaking of SU(3) to SU(2) and U(1)](../../../standard-model.md#adjoint-higgs-breaking-of-su-3-to-su-2-and-u-1) without changing the local [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) spectrum.

## 3

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A leading short-distance [Standard Model](../../../standard-model.md) contribution to [neutral D-meson mixing](../../../physics.md#neutral-d-meson-mixing) is a [box Feynman diagram](../../../perturbative-quantum-field-theory.md#box-feynman-diagram) with two [W bosons](../../../standard-model.md#w-boson) and two internal down-type [quark](../../../standard-model.md#quark) lines:

<a id="3/a/image-short-distance-box-contribution-to-neutral-d-meson-mixing"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305-q3a.png)

**[Figure 1](#3/a/image-short-distance-box-contribution-to-neutral-d-meson-mixing). Short-distance box contribution to neutral D-meson mixing**.

The incoming $c\bar u$ pair becomes $u\bar c$; the internal labels run over the [down quark](../../../standard-model.md#down-quark), [strange quark](../../../standard-model.md#strange-quark) and [bottom quark](../../../standard-model.md#bottom-quark). Each corner is a [weak charged current](../../../standard-model.md#charged-current) vertex. Four such vertices make the contribution of order $g^4$. Summing the internal flavours produces [Cabibbo-Kobayashi-Maskawa matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) factors and the [Glashow-Iliopoulos-Maiani mechanism](../../../standard-model.md#glashow-iliopoulos-maiani-mechanism): the flavour-independent term cancels by $\sum_i V_{ci}^*V_{ui}=0$. This [box Feynman diagram](../../../perturbative-quantum-field-theory.md#box-feynman-diagram) is one contribution; long-distance intermediate [hadron](../../../physics.md#hadron) states can also contribute to [neutral D-meson mixing](../../../physics.md#neutral-d-meson-mixing).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $|1\rangle=|D^0\rangle$, $|2\rangle=|\bar D^0\rangle$. In the rest frame, the [CPT theorem](../../../quantum-field-theory.md#cpt-theorem) interchanges these states up to irrelevant phases. For the weak [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) $H'$, with $H'=H'^{\dagger}$, and its antiunitary [CPT symmetry](../../../quantum-field-theory.md#cpt-symmetry) operator $\Theta$,

$$
\langle\Theta1|H'|\Theta1\rangle=\langle1|H'|1\rangle^*.
$$

Its diagonal [matrix elements](../../../vector-space.md#matrix-element) are real by [Hermitian conjugation](../../../hilbert-space.md#hermitian-conjugation), so

$$
\boxed{R_{11}=R_{22}.}
$$

In the specified phase convention, the [CP symmetry](../../../quantum-field-theory.md#cp-symmetry) operator on this two-state subspace is $-\sigma_x$. If the [weak interaction](../../../standard-model.md#weak-interaction) preserves [CP symmetry](../../../quantum-field-theory.md#cp-symmetry), $\sigma_xR\sigma_x=R$, giving

$$
\boxed{R_{12}=R_{21}.}
$$

Independently, [Hermitian conjugation](../../../hilbert-space.md#hermitian-conjugation) gives $R_{21}=R_{12}^*$ for this $H'$. Hence [CP symmetry](../../../quantum-field-theory.md#cp-symmetry) makes the off-diagonal element real in this convention; that conjugation relation alone does not imply [CP symmetry](../../../quantum-field-theory.md#cp-symmetry).

For [neutral meson mixing](../../../physics.md#neutral-meson-mixing) described by the decay-effective [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) $R=M-i\Gamma/2$, the effective matrix is generally not a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). The [CPT constraints on neutral-meson mixing](../../../physics.md#cpt-constraints-on-neutral-meson-mixing) still give equality of the complex diagonal entries, expressing equal masses and total [decay widths](../../../relativistic-quantum-field.md#decay-width), and [CP symmetry](../../../quantum-field-theory.md#cp-symmetry) gives equality of the off-diagonal entries in the specified convention. One must not additionally impose $R_{21}=R_{12}^*$ on this decay-effective matrix.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [tree-level Feynman diagrams](../../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram) contain an unchanged [spectator quark](../../../standard-model.md#spectator-quark), of [up quark](../../../standard-model.md#up-quark) flavour and the two possible [weak charged current](../../../standard-model.md#charged-current) transitions of the [charm antiquark](../../../standard-model.md#charm-antiquark):

<a id="3/c/image-favoured-and-doubly-cabibbo-suppressed-anti-d-decays"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305-q3c.png)

**[Figure 2](#3/c/image-favoured-and-doubly-cabibbo-suppressed-anti-d-decays). Favoured and doubly Cabibbo-suppressed anti-D decays**.

For $\bar D^0\to K^+\pi^-$, $\bar c\to\bar sW^-$ and $W^-\to d\bar u$. The [spectator quark](../../../standard-model.md#spectator-quark) combines with $\bar s$ into the [kaon](../../../physics.md#kaon) $K^+=u\bar s$, while $d\bar u$ forms the [pion](../../../standard-model.md#pion) $\pi^-$. The [Cabibbo-Kobayashi-Maskawa matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) factor is $V_{cs}V_{ud}^*$.

For $\bar D^0\to K^-\pi^+$, $\bar c\to\bar dW^-$ and $W^-\to s\bar u$. The [spectator quark](../../../standard-model.md#spectator-quark) combines with $\bar d$ into the [pion](../../../standard-model.md#pion) $\pi^+=u\bar d$, while $s\bar u$ forms the [kaon](../../../physics.md#kaon) $K^-$. The [Cabibbo-Kobayashi-Maskawa matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) factor is $V_{cd}V_{us}^*$.

Neglecting [neutral D-meson mixing](../../../physics.md#neutral-d-meson-mixing) and assuming comparable [strong interaction](../../../standard-model.md#strong-interaction) [matrix elements](../../../vector-space.md#matrix-element), the relative direct [decay widths](../../../relativistic-quantum-field.md#decay-width) are

$$
\boxed{\frac{\Gamma(\bar D^0\to K^-\pi^+)}{\Gamma(\bar D^0\to K^+\pi^-)}
\approx\left|\frac{V_{cd}V_{us}^*}{V_{cs}V_{ud}^*}\right|^2\approx\tan^4\theta_C.}
$$

Here $\theta_C$ is the [Cabibbo angle](../../../standard-model.md#cabibbo-angle). The second process is **doubly [Cabibbo suppressed](../../../standard-model.md#cabibbo-suppression)**: it contains two small [Cabibbo suppression](../../../standard-model.md#cabibbo-suppression) factors in its amplitude. The [Cabibbo angle](../../../standard-model.md#cabibbo-angle) estimate assumes similar [Quantum chromodynamics](../../../standard-model.md#quantum-chromodynamics) [matrix elements](../../../vector-space.md#matrix-element); it is not an exact rate equality.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Both the [D meson](../../../physics.md#d-meson) and [kaon](../../../physics.md#kaon) are spin-zero [pseudoscalars](../../../quantum-mechanics.md#pseudoscalar). The [strong interaction](../../../standard-model.md#strong-interaction) states obey [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory). Consequently an [axial current](../../../relativistic-quantum-field.md#axial-current) [matrix element](../../../vector-space.md#matrix-element) between them would have to be a [pseudovector](../../../vector-space.md#pseudovector) formed from only $p$ and $k$, which is impossible: an [totally antisymmetric tensor](../../../linear-algebra.md#totally-antisymmetric-tensor) would require more [linearly independent vectors](../../../vector-space.md#linear-independence). Thus

$$
\langle K^+(k)|\bar c\gamma^\mu\gamma^5s|\bar D^0(p)\rangle=0.
$$

[Lorentz covariance](../../../special-relativity.md#lorentz-covariance) then leaves two [linearly independent vectors](../../../vector-space.md#linear-independence) for the [vector current](../../../relativistic-quantum-field.md#vector-current) [matrix element](../../../vector-space.md#matrix-element), giving the [pseudoscalar-to-pseudoscalar form factors](../../../physics.md#pseudoscalar-to-pseudoscalar-form-factor)

$$
\langle K^+(k)|\bar c\gamma^\mu s|\bar D^0(p)\rangle
=(p+k)^\mu f_+(q^2)+(p-k)^\mu f_-(q^2),\qquad q=p-k.
$$

The vanishing [axial current](../../../relativistic-quantum-field.md#axial-current) here follows from [strong interaction](../../../standard-model.md#strong-interaction) [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory), not [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory) of the [weak interaction](../../../standard-model.md#weak-interaction).

To obtain the requested decay formula, use [naive factorization of a nonleptonic meson decay](../../../quantum-field-theory.md#naive-factorization-of-a-nonleptonic-meson-decay): approximate the four-quark [matrix element](../../../vector-space.md#matrix-element) by the product of the $\bar D^0\to K^+$ current [matrix element](../../../vector-space.md#matrix-element) and the vacuum-to-[pion](../../../standard-model.md#pion) [matrix element](../../../vector-space.md#matrix-element). This is an additional hadronic approximation; tree-level weak vertices alone do not establish it, and nonfactorizable [Quantum chromodynamics](../../../standard-model.md#quantum-chromodynamics) effects can change the result. The vacuum-to-[pion](../../../standard-model.md#pion) [vector current](../../../relativistic-quantum-field.md#vector-current) [matrix element](../../../vector-space.md#matrix-element) vanishes by [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory), while the specified [pion decay constant](../../../standard-model.md#pion-decay-constant) normalization gives

$$
\langle\pi^-(q)|\bar d\gamma_\mu(1-\gamma^5)u|0\rangle=+i\sqrt2 F_\pi q_\mu.
$$

The $\sqrt2$ cancels the $1/\sqrt2$ in the [four-fermion interaction](../../../quantum-field-theory.md#four-fermion-interaction). Up to an irrelevant overall phase, the [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) is therefore

$$
\mathcal M=G_F V_{cs}V_{ud}^*F_\pi\left[(m_D^2-m_K^2)f_+(q^2)+q^2f_-(q^2)\right].
$$

For $m_\pi=0$, $q^2=0$, so only $f_+(0)$ survives. Integrating the [two-body decay phase space](../../../quantum-mechanics.md#two-body-decay-phase-space) in the [D meson](../../../physics.md#d-meson) rest frame gives

$$
|\boldsymbol k|=\frac{m_D^2-m_K^2}{2m_D},\qquad
\Gamma=\frac{|\boldsymbol k|}{8\pi m_D^2}|\mathcal M|^2.
$$

Hence

$$
\boxed{A=\frac{(m_D^2-m_K^2)^3}{16\pi m_D^3},\qquad
\Gamma=\frac{G_F^2(m_D^2-m_K^2)^3}{16\pi m_D^3}\left|V_{ud}^*V_{cs}F_\pi f_+(0)\right|^2.}
$$

This coefficient uses exactly the stated [pion decay constant](../../../standard-model.md#pion-decay-constant) convention and the stated massless-[pion](../../../standard-model.md#pion) approximation.

## 4

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [deep inelastic scattering](../../../standard-model.md#deep-inelastic-scattering) process contains a virtual [photon](../../../quantum-mechanics.md#photon) exchanged between the [Electron](../../../physics.md#electron) and the [hadron](../../../physics.md#hadron):

<a id="4/a/image-inclusive-electron-hadron-scattering-through-a-virtual-photon"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305-q4a.png)

**[Figure 3](#4/a/image-inclusive-electron-hadron-scattering-through-a-virtual-photon). Inclusive electron-hadron scattering through a virtual photon**.

Use an electromagnetic [vector current](../../../relativistic-quantum-field.md#vector-current) $J^\mu$ containing the dimensionless [quark](../../../standard-model.md#quark) charges, with the coupling $e$ factored out. The [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude), up to an irrelevant phase, is

$$
\mathcal M_X=\frac{e^2}{q^2}\bar u(p')\gamma_\mu u(p)\langle X|J^\mu|H\rangle.
$$

To match the printed prefactor, define the [leptonic tensor](../../../standard-model.md#leptonic-tensor) with a [spin sum](../../../relativistic-quantum-field.md#spin-sum) over both [Electron](../../../physics.md#electron) spins and keep the initial [spin average](../../../relativistic-quantum-field.md#spin-average) $1/2$ outside it. The [gamma-matrix trace](../../../relativistic-quantum-field.md#gamma-matrix-trace) gives

$$
\boxed{L_{\mu\nu}=\operatorname{Tr}(\not p'\gamma_\mu\not p\gamma_\nu)
=4\left(p_\mu p'_\nu+p_\nu p'_\mu-g_{\mu\nu}p\cdot p'\right).}
$$

For a stationary target and massless [Electron](../../../physics.md#electron), the [invariant flux factor](../../../quantum-mechanics.md#invariant-flux-factor) is $4ME$. The inclusive final-state [Lorentz-invariant phase-space measure](../../../quantum-mechanics.md#lorentz-invariant-phase-space-measure) and target [spin average](../../../relativistic-quantum-field.md#spin-average) are contained in $4\pi W_H^{\mu\nu}$. Thus the [differential scattering cross-section](../../../quantum-mechanics.md#differential-scattering-cross-section) is

$$
\frac{d\sigma}{d^3p'}=\frac1{4ME}\frac1{(2\pi)^3 2E'}\frac12\frac{e^4}{(q^2)^2}L_{\mu\nu}(4\pi W_H^{\mu\nu})
=\boxed{\frac{e^4}{8(2\pi)^2 MEE'(q^2)^2}L_{\mu\nu}W_H^{\mu\nu}.}
$$

Here $q^4$ means $(q^2)^2$. If the initial [spin average](../../../relativistic-quantum-field.md#spin-average) is instead built into the [leptonic tensor](../../../standard-model.md#leptonic-tensor), its normalization is $2(\cdots)$ and the displayed cross-section prefactor must be doubled. The two conventions give the same observable.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For an unpolarized electromagnetic target, [Lorentz covariance](../../../special-relativity.md#lorentz-covariance) and [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory) permit a symmetric [hadronic tensor](../../../standard-model.md#hadronic-tensor) built from $g^{\mu\nu}$, $P^\mu$ and $q^\mu$, where $P=P_H$. Its surviving general form is

$$
W^{\mu\nu}=a g^{\mu\nu}+bP^\mu P^\nu+cq^\mu q^\nu+d(P^\mu q^\nu+q^\mu P^\nu).
$$

The [totally antisymmetric tensor](../../../linear-algebra.md#totally-antisymmetric-tensor) structure $\epsilon^{\mu\nu\rho\sigma}P_\rho q_\sigma$ is excluded by electromagnetic [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory) for this unpolarized target. The other possible antisymmetric structure, $P^\mu q^\nu-q^\mu P^\nu$, cannot be transverse for generic scattering kinematics and hence is excluded by [current conservation](../../../quantum-field-theory.md#conserved-current). [Current conservation](../../../quantum-field-theory.md#conserved-current) gives the [Ward identities](../../../perturbative-quantum-field-theory.md#ward-identity) $q_\mu W^{\mu\nu}=q_\nu W^{\mu\nu}=0$, imposing

$$
b\nu+dq^2=0,\qquad a+cq^2+d\nu=0,\qquad \nu=P\cdot q.
$$

Two scalar functions remain. Taking $\widetilde P^\mu=P^\mu-\nu q^\mu/q^2$ gives the transverse basis

$$
\boxed{W_H^{\mu\nu}=\left(-g^{\mu\nu}+\frac{q^\mu q^\nu}{q^2}\right)F_1(x,q^2)+\widetilde P^\mu\widetilde P^\nu\frac{F_2(x,q^2)}{\nu},\qquad x=-\frac{q^2}{2\nu}.}
$$

These are the [deep-inelastic structure functions](../../../standard-model.md#deep-inelastic-structure-function); $x$ is [Bjorken x](../../../standard-model.md#bjorken-x). At fixed target mass, the two independent [Lorentz scalar](../../../special-relativity.md#lorentz-scalar) invariants can equivalently be chosen as $x,q^2$. In this paper $\nu=P\cdot q$ has dimensions of mass squared, rather than the alternative convention $\nu=P\cdot q/M$ used for energy transfer.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Use the [massless collinear parton approximation](../../../standard-model.md#massless-collinear-parton-approximation) in a high-energy frame: $P^2=0$, $k=\xi P$, and $k'=\xi P+q$ with $k'^2=0$. This neglects target-mass corrections to the [parton model](../../../standard-model.md#parton-model); it does not literally set a stationary massive target to a massless particle in the earlier flux formula.

For a [quark](../../../standard-model.md#quark) of dimensionless charge $Q_f$, the electromagnetic [vector current](../../../relativistic-quantum-field.md#vector-current) [matrix element](../../../vector-space.md#matrix-element) is $Q_f\bar u(k')\gamma^\mu u(k)$. The [spin average](../../../relativistic-quantum-field.md#spin-average) and [gamma-matrix trace](../../../relativistic-quantum-field.md#gamma-matrix-trace) give

$$
\frac12\sum_{\rm spins}J^\mu J^{\nu *}=2Q_f^2\left(k^\mu k'^\nu+k^\nu k'^\mu-g^{\mu\nu}k\cdot k'\right).
$$

Integrating the three-momentum [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) in the [parton](../../../standard-model.md#parton) [hadronic tensor](../../../standard-model.md#hadronic-tensor) leaves

$$
\widetilde W^{\mu\nu}=\frac{\delta(q^0+\xi E_P-E_{k'})}{2\xi E_{k'}}\left(k^\mu k'^\nu+k^\nu k'^\mu-g^{\mu\nu}k\cdot k'\right).
$$

Since $k\cdot k'=\xi\nu$, this is

$$
\widetilde W^{\mu\nu}=\frac{\delta(q^0+\xi E_P-E_{k'})}{E_{k'}}\left[\xi P^\mu P^\nu+\frac12(P^\mu q^\nu+q^\mu P^\nu)-\frac\nu2g^{\mu\nu}\right].
$$

For the massless [Electron](../../../physics.md#electron) momenta, $p^2=p'^2=0$ and $q=p-p'$. Substitution into the [leptonic tensor](../../../standard-model.md#leptonic-tensor) gives

$$
q^\mu L_{\mu\nu}=4\left[-(p\cdot p')p'_\nu+(p\cdot p')p_\nu-(p\cdot p')(p_\nu-p'_\nu)\right]=0,
$$

and likewise $q^\nu L_{\mu\nu}=0$. These [Ward identities](../../../perturbative-quantum-field-theory.md#ward-identity) eliminate every term with an exposed $q$ index in the contraction. Therefore

$$
\boxed{\widetilde W^{\mu\nu}\doteq\frac{\delta(q^0+\xi E_P-E_{k'})}{E_{k'}}\left[\xi P^\mu P^\nu-\frac{\nu}{2}g^{\mu\nu}\right].}
$$

Here $\doteq$ means equality **after contraction with the [leptonic tensor](../../../standard-model.md#leptonic-tensor)**. The shortened tensor is not itself conserved; the omitted terms restore [current conservation](../../../quantum-field-theory.md#conserved-current) in the full [hadronic tensor](../../../standard-model.md#hadronic-tensor).

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

On the physical positive-energy branch, put $\omega=q^0+\xi E_P$. The massless outgoing [parton](../../../standard-model.md#parton) obeys

$$
E_{k'}^2-\omega^2=-(\xi P+q)^2=-q^2-2\xi\nu=2\nu(x-\xi).
$$

Since $E_{k'}=\omega>0$ on the support and $\nu>0$, the [positive-energy on-shell delta function identity](../../../quantum-mechanics.md#positive-energy-on-shell-delta-function-identity) gives

$$
\frac{\delta(\omega-E_{k'})}{E_{k'}}=2\delta(E_{k'}^2-\omega^2)=\frac{\delta(x-\xi)}{\nu}.
$$

Insert this into the [parton model](../../../standard-model.md#parton-model) sum, and write

$$
S(x)=\sum_f Q_f^2\left[q_f(x)+\bar q_f(x)\right].
$$

The [parton distribution functions](../../../standard-model.md#parton-distribution-function) $q_f,\bar q_f$ are number densities in momentum fraction. The contributing tensor becomes

$$
W_H^{\mu\nu}\doteq S(x)\left[\frac{x}{\nu}P^\mu P^\nu-\frac12g^{\mu\nu}\right].
$$

Comparing with part (b), under the same [leptonic tensor](../../../standard-model.md#leptonic-tensor) contraction, gives

$$
F_1(x)=\frac12 S(x),\qquad F_2(x)=xS(x),\qquad
\boxed{F_2(x,q^2)=2xF_1(x,q^2).}
$$

This is the [Callan-Gross relation](../../../standard-model.md#callan-gross-relation) for massless [partons](../../../standard-model.md#parton) of [spin angular momentum](../../../quantum-mechanics.md#spin) $1/2$ at leading order. The [longitudinal deep-inelastic structure function](../../../standard-model.md#longitudinal-deep-inelastic-structure-function) is $F_L=F_2-2xF_1=0$ in this approximation. Target-mass effects and radiative [Quantum chromodynamics](../../../standard-model.md#quantum-chromodynamics) corrections can change the relation. The leading [parton model](../../../standard-model.md#parton-model) also gives [Bjorken scaling](../../../standard-model.md#bjorken-scaling): at this level the [deep-inelastic structure functions](../../../standard-model.md#deep-inelastic-structure-function) depend on $x$ alone.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
