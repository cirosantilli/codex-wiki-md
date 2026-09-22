# Paper 307

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_307.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_307.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
  - [vii](#1/vii)
    - [Solution](#1/vii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
  - [vi](#3/vi)
    - [Solution](#3/vi/solution)

## 1

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Choose $P_\mu=-i\partial_\mu$ and left Grassmann derivatives. A consistent differential realization of [four-dimensional N=1 supersymmetry](../../../supersymmetry.md#four-dimensional-n-1-supersymmetry) is

$$
\mathcal Q_\alpha=i\frac{\partial}{\partial\theta^\alpha}-(\sigma^\mu\bar\theta)_\alpha\partial_\mu,
\qquad
\overline{\mathcal Q}_{\dot\alpha}=-i\frac{\partial}{\partial\bar\theta^{\dot\alpha}}+(\theta\sigma^\mu)_{\dot\alpha}\partial_\mu.
$$

The signs can change with the definitions of $P_\mu$, Grassmann differentiation and the finite transformation, but these operators obey the convention-independent content of the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra),

$$
\{\mathcal Q_\alpha,\overline{\mathcal Q}_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu,
\qquad
\{\mathcal Q_\alpha,\mathcal Q_\beta\}
=\{\overline{\mathcal Q}_{\dot\alpha},\overline{\mathcal Q}_{\dot\beta}\}=0.
$$

They follow by expanding the finite transformation to first order and requiring a supersymmetry translation of the [superspace](../../../supersymmetry.md#superspace) coordinates.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A [vector superfield](../../../supersymmetry.md#vector-superfield) is a real [superfield](../../../supersymmetry.md#superfield),

$$
V=V^\dagger.
$$

For a non-Abelian gauge theory it is also Lie-algebra valued, $V=V^aT_a$. The reality condition permits the component expansion to be reduced to [Wess-Zumino gauge](../../../supersymmetry.md#wess-zumino-gauge), where the physical fields are a gauge field and gaugino together with a real auxiliary field.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

A [chiral superfield](../../../supersymmetry.md#chiral-superfield) is annihilated by the antichiral [supersymmetric covariant derivative](../../../supersymmetry.md#supersymmetric-covariant-derivative):

$$
\overline{\mathcal D}_{\dot\alpha}\Phi=0.
$$

Equivalently, it depends on $(y^\mu,\theta)$ with $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$, and has the finite expansion $\Phi=\phi+\sqrt2\theta\psi+\theta^2F$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

The [gauge-transformation superfield](../../../supersymmetry.md#gauge-transformation-superfield) $\Lambda=\Lambda^aT_a$ is a dimensionless [chiral superfield](../../../supersymmetry.md#chiral-superfield):

$$
[\Lambda]=0,
\qquad
\overline{\mathcal D}_{\dot\alpha}\Lambda=0.
$$

It takes values in the complexified $\mathfrak{su}(3)$ Lie algebra. It need not be real; its Hermitian conjugate is antichiral. This complexification is necessary because a general [superspace](../../../supersymmetry.md#superspace) gauge transformation must preserve chirality.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

With canonical normalization, the renormalizable [supersymmetric gauge theory](../../../supersymmetry.md#supersymmetric-gauge-theory) has

$$
\mathcal L=
\int d^4\theta\,\Phi^\dagger e^{2V}\Phi
+\left[\frac1{16g^2}\int d^2\theta\,
\operatorname{Tr}(W^\alpha W_\alpha)+\mathrm{h.c.}\right].
$$

The first term is the gauge-covariant [Kähler potential](../../../supersymmetry.md#kahler-potential) and the second is the [Supersymmetric Yang-Mills action](../../../supersymmetry.md#supersymmetric-yang-mills-action). A holomorphic [superpotential](../../../supersymmetry.md#superpotential) would also be integrated as $\int d^2\theta\,\mathcal W(\Phi)+\mathrm{h.c.}$, but one commuting field in the fundamental representation of $SU(3)$ admits no nonconstant renormalizable gauge-invariant superpotential: the apparent cubic $\epsilon_{ijk}\Phi^i\Phi^j\Phi^k$ vanishes.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

Under $\Phi'=e^{-2i\Lambda}\Phi$, the conjugate field transforms as $\Phi'{}^\dagger=\Phi^\dagger e^{2i\Lambda^\dagger}$. Invariance of the canonical Kähler term therefore requires

$$
e^{2i\Lambda^\dagger}e^{2V'}e^{-2i\Lambda}=e^{2V},
$$

or

$$
\boxed{e^{2V'}=e^{-2i\Lambda^\dagger}e^{2V}e^{2i\Lambda}}.
$$

This is the finite non-Abelian [supergauge transformation](../../../supersymmetry.md#supergauge-transformation) of the vector superfield.

<h3 id="1/vii">vii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#1/vii)

The relation in part vi gives

$$
\Phi'{}^\dagger e^{2V'}\Phi'
=\Phi^\dagger e^{2i\Lambda^\dagger}
e^{-2i\Lambda^\dagger}e^{2V}e^{2i\Lambda}e^{-2i\Lambda}\Phi
=\Phi^\dagger e^{2V}\Phi,
$$

so the full-superspace term has [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance). The [chiral field-strength superfield](../../../supersymmetry.md#chiral-field-strength-superfield) transforms covariantly,

$$
W_\alpha' =e^{-2i\Lambda}W_\alpha e^{2i\Lambda}.
$$

Cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace) then gives $\operatorname{Tr}(W'{}^\alpha W'_\alpha)=\operatorname{Tr}(W^\alpha W_\alpha)$. Both superspace integrals, and hence the entire Lagrangian density, are invariant.

## 2

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [hierarchy problem](../../../standard-model.md#hierarchy-problem) is visible in the one-loop top-quark contribution to the [Higgs boson](../../../standard-model.md#higgs-boson) mass parameter,

$$
\delta m_H^2\sim-\frac{3|y_t|^2}{8\pi^2}\Lambda^2.
$$

In a supersymmetric theory the corresponding [stop](../../../supersymmetry.md#top-squark) loop has the opposite quadratic term. If supersymmetry is softly broken, the remaining correction is roughly

$$
|\delta m_H^2|\sim\frac{3|y_t|^2}{8\pi^2}m_{\widetilde t}^2
\log\frac{\Lambda}{m_{\widetilde t}}.
$$

The two relevant one-loop [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram) are a Higgs two-point function with a closed top-quark loop and the analogous stop loop. Requiring the residual correction not to exceed the electroweak scale by many orders of magnitude gives the [naturalness](../../../standard-model.md#naturalness-physics) expectation $m_{\widetilde t}$, and broadly other [sparticle](../../../supersymmetry.md#sparticle) masses, at a few TeV or below. This is an order-of-magnitude argument rather than a mass bound.

[R-parity](../../../supersymmetry.md#r-parity) is

$$
R_p=(-1)^{3(B-L)+2s},
$$

where $B$ is [baryon number](../../../standard-model.md#baryon-number), $L$ is [lepton number](../../../standard-model.md#lepton-number) and $s$ is [spin angular momentum](../../../quantum-mechanics.md#spin). Standard Model particles have $R_p=+1$, while their superpartners have $R_p=-1$. The renormalizable [R-parity-violating](../../../supersymmetry.md#r-parity-violation) superpotential of the [Minimal supersymmetric Standard Model](../../../supersymmetry.md#minimal-supersymmetric-standard-model) is

$$
W_{\rm RPV}=\frac12\lambda_{ijk}L_iL_jE_k^c
+\lambda'_{ijk}L_iQ_jD_k^c
+\frac12\lambda''_{ijk}U_i^cD_j^cD_k^c
+\kappa_iL_iH_u,
$$

with $\lambda_{ijk}=-\lambda_{jik}$ and $\lambda''_{ijk}=-\lambda''_{ikj}$.

Combining $\lambda'_{i1k}L_iQ_1D_k^c$ with $\lambda''_{11k}U_1^cD_1^cD_k^c$ produces [proton decay](../../../standard-model.md#proton-decay) through exchange of a virtual right-handed down-type [squark](../../../supersymmetry.md#squark). The tree diagram has $u$ and $d$ entering the baryon-number-violating vertex, an internal $\widetilde d_{Rk}$ line, and the lepton-number-violating vertex emitting $\bar\nu_i$ and a light quark. Hadronization gives

$$
p\longrightarrow\pi^++\bar\nu_i.
$$

The invisible particle is an [antineutrino](../../../standard-model.md#antineutrino) of any family $i=1,2,3$, and electric-charge conservation requires a positively charged [pion](../../../standard-model.md#pion). The antisymmetry of $\lambda''_{11k}$ requires $k=2$ or $3$.

Integrating out a squark of mass $m_{\widetilde q}$ gives a dimension-six interaction with coefficient $C\sim\lambda'\lambda''/m_{\widetilde q}^2$. Ignoring order-one hadronic and phase-space factors,

$$
\Gamma_p\sim\frac{|\lambda'\lambda''|^2}{8\pi}
\frac{m_p^5}{m_{\widetilde q}^4}.
$$

For $m_p\sim1\ \mathrm{GeV}$ and $m_{\widetilde q}\sim10^4\ \mathrm{GeV}$, the factor before the couplings is about $10^{-18}$--$10^{-17}\ \mathrm{GeV}$. A lifetime above $10^{34}$ years is about $10^{65}\ \mathrm{GeV}^{-1}$, so $\Gamma_p\lesssim10^{-65}\ \mathrm{GeV}$ and

$$
\boxed{|\lambda'\lambda''|\lesssim10^{-24}}
$$

at order-of-magnitude accuracy. Hadronic matrix elements and flavour choices alter the numerical coefficient, not the conclusion that simultaneous baryon- and lepton-number violation is extraordinarily constrained.

The matter-parity factor $(-1)^{3(B-L)}$ is odd for every quark or lepton superfield and even for either Higgs superfield. Each term in $W_{\rm RPV}$ contains an odd number of matter superfields, so [R-parity](../../../supersymmetry.md#r-parity) forbids all four types of term. Standard MSSM Yukawa interactions contain two matter superfields and remain allowed.

Finally, the requested four-point interaction contains a squark, an antisquark, a $W$ boson and a gluon. It comes from the squark [gauge-covariant kinetic term](../../../quantum-field-theory.md#gauge-covariant-kinetic-term)

$$
(D_\mu\widetilde Q)^\dagger D^\mu\widetilde Q,
\qquad
D_\mu=\partial_\mu+ig_sG_\mu^aT^a+ig_2W_\mu^It^I+\cdots.
$$

The cross term is

$$
2g_sg_2\,\widetilde Q^\dagger T^at^I\widetilde Q\,G_\mu^aW^{I\mu},
$$

because the colour and weak generators commute. With all fields incoming, its [Feynman rule](../../../perturbative-quantum-field-theory.md#feynman-rule) is

$$
2ig_sg_2g^{\mu\nu}(T^a)_{ji}(t^I)_{BA},
$$

with the conventional $1/\sqrt2$ conversion when $W^I$ is replaced by $W^\pm$.

## 3

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

With $\epsilon_{0123}=+1$, define the [Pauli-Lubanski pseudovector](../../../special-relativity.md#pauli-lubanski-pseudovector) by

$$
W_\mu=\frac12\epsilon_{\mu\nu\rho\sigma}M^{\nu\rho}P^\sigma.
$$

For a translation $a^\mu$ and a [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) $\Lambda=\exp(\omega)$, a left-handed [Weyl spinor](../../../relativistic-quantum-field.md#weyl-spinor) transforms as

$$
\psi'_\alpha(x')=
\left[\exp\left(-\frac i2\omega_{\mu\nu}\sigma^{\mu\nu}\right)\right]_\alpha{}^\beta
\psi_\beta(x),
\qquad x'=\Lambda x+a.
$$

Equivalently, the active field at a fixed point uses $\psi'(x)=S(\Lambda)\psi(\Lambda^{-1}(x-a))$.

The [Clebsch-Gordan decomposition](../../../quantum-mechanics.md#clebsch-gordan-decomposition) is

$$
\left(\frac12,0\right)\otimes\left(\frac12,0\right)
=(1,0)\oplus(0,0).
$$

Indeed,

$$
\psi_\alpha\chi_\beta
=\psi_{(\alpha}\chi_{\beta)}
+\frac12\epsilon_{\alpha\beta}\psi^\gamma\chi_\gamma.
$$

The symmetric spinor is the $(1,0)$ representation, while its antisymmetric part is the Lorentz scalar $(0,0)$.

In the conventions used below, the nonzero brackets involving the supercharges are

$$
\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu,
\qquad
[M^{\mu\nu},Q_\alpha]=i(\sigma^{\mu\nu})_\alpha{}^\beta Q_\beta,
$$



$$
[M^{\mu\nu},\bar Q_{\dot\alpha}]
=i(\bar\sigma^{\mu\nu})_{\dot\alpha}{}^{\dot\beta}\bar Q_{\dot\beta},
\qquad
[P_\mu,Q_\alpha]=[P_\mu,\bar Q_{\dot\alpha}]=0,
$$

and $\{Q_\alpha,Q_\beta\}=\{\bar Q_{\dot\alpha},\bar Q_{\dot\beta}\}=0$. These equations, together with the [Poincare algebra](../../../special-relativity.md#poincare-algebra), are the four-dimensional $\mathcal N=1$ [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) without central charges.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Both terms in $B_\mu=W_\mu-\frac14\bar Q\bar\sigma_\mu Q$ commute with momentum. For the first,

$$
[W_\mu,P_\rho]=\frac12\epsilon_{\mu\nu\lambda\sigma}
[M^{\nu\lambda},P_\rho]P^\sigma=0,
$$

because the two resulting products of momenta are symmetric in indices contracted with the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol). For the second, $[P_\rho,Q]=[P_\rho,\bar Q]=0$. Therefore

$$
\boxed{[B_\mu,P_\rho]=0}.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Using part i and $[P_\mu,P_\rho]=0$,

$$
[C_{\mu\nu},P_\rho]
=[B_\mu P_\nu-B_\nu P_\mu,P_\rho]=0.
$$

Thus

$$
\boxed{[C_{\mu\nu},P_\rho]=0}.
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Move $Q_\alpha$ through the two odd supercharges and use $\{Q_\alpha,Q_\beta\}=0$:

$$
[\bar Q_{\dot\beta}(\bar\sigma_\mu)^{\dot\beta\beta}Q_\beta,Q_\alpha]
=-\{Q_\alpha,\bar Q_{\dot\beta}\}
(\bar\sigma_\mu)^{\dot\beta\beta}Q_\beta.
$$

Consequently,

$$
\boxed{[\bar Q\bar\sigma_\mu Q,Q_\alpha]
=-2(\sigma^\nu\bar\sigma_\mu)_\alpha{}^\beta P_\nu Q_\beta}.
$$

This unsimplified form keeps all signs transparent; changing the placement convention for the conjugate supercharge changes the displayed intermediate sign consistently with the definition of $B_\mu$.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The [Pauli-Lubanski pseudovector](../../../special-relativity.md#pauli-lubanski-pseudovector) and the spinor Lorentz transformation give

$$
[W_\mu,Q_\alpha]=i(\sigma_{\mu\nu})_\alpha{}^\beta P^\nu Q_\beta.
$$

Combining this with part iii and the [Pauli matrix](../../../algebra.md#pauli-matrices) identity $\sigma^\nu\bar\sigma_\mu=\eta^\nu{}_\mu\mathbf1+2i\sigma^\nu{}_\mu$ cancels the term containing $\sigma_{\mu\nu}P^\nu$. In these conventions,

$$
\boxed{[B_\mu,Q_\alpha]=-\frac12P_\mu Q_\alpha}.
$$

Simultaneously reversing the convention for $W_\mu$ reverses the final sign, but the proportionality to $P_\mu Q_\alpha$ is invariant and is what the next part needs.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Since momentum commutes with the supercharge, part iv gives

$$
[C_{\mu\nu},Q_\alpha]
=[B_\mu,Q_\alpha]P_\nu-[B_\nu,Q_\alpha]P_\mu
=-\frac12(P_\mu P_\nu-P_\nu P_\mu)Q_\alpha=0.
$$

Therefore

$$
\boxed{[C_{\mu\nu},Q_\alpha]=0}.
$$

Hermitian conjugation also gives $[C_{\mu\nu},\bar Q_{\dot\alpha}]=0$.

<h3 id="3/vi">vi</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#3/vi)

The antisymmetric $C_{\mu\nu}$ transforms as a [Lorentz tensor](../../../special-relativity.md#lorentz-tensor), so its complete contraction

$$
\widetilde C_2=C_{\mu\nu}C^{\mu\nu}
$$

is a [Lorentz scalar](../../../special-relativity.md#lorentz-scalar). Hence

$$
[M^{\rho\sigma},\widetilde C_2]=0.
$$

Parts ii and v give $[P_\rho,\widetilde C_2]=[Q_\alpha,\widetilde C_2]=[\bar Q_{\dot\alpha},\widetilde C_2]=0$. It therefore commutes with every generator of the [Super-Poincaré algebra](../../../supersymmetry.md#super-poincare-algebra) and is a [Casimir element](../../../semisimple-lie-algebra.md#casimir-element), called the [superspin Casimir](../../../supersymmetry.md#superspin-casimir).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
