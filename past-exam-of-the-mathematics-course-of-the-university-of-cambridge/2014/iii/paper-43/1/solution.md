<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [hypercharge](../../../../../hypercharge.md) normalization $Q_{\rm electric}=T^3+Y$. All matter [chiral superfields](../../../../../chiral-superfield.md) are written with left-handed [Weyl spinors](../../../../../weyl-spinor.md), so the fields denoted by a superscript $c$ contain the charge conjugates of the usual right-handed [Standard Model fermions](../../../../../standard-model-fermion.md). The [MSSM superfield representations](../../../../../mssm-superfield-representations.md) are

$$
\begin{array}{c|c|c}
\text{chiral superfield}&SU(3)_c\times SU(2)_L\times U(1)_Y&\text{multiplicity}\\\hline
Q&(\mathbf3,\mathbf2,1/6)&3\\
U^c&(\overline{\mathbf3},\mathbf1,-2/3)&3\\
D^c&(\overline{\mathbf3},\mathbf1,1/3)&3\\
L&(\mathbf1,\mathbf2,-1/2)&3\\
E^c&(\mathbf1,\mathbf1,1)&3\\
H_u&(\mathbf1,\mathbf2,1/2)&1\\
H_d&(\mathbf1,\mathbf2,-1/2)&1
\end{array}
$$

Each [fermion generation](../../../../../fermion-generation.md) contributes the first five [chiral superfields](../../../../../chiral-superfield.md). Their [complex scalar field](../../../../../complex-scalar-field.md) partners are [squarks](../../../../../squark.md) for the [quarks](../../../../../quark.md) and [sleptons](../../../../../slepton.md) for the [leptons](../../../../../lepton.md). Each [Higgs chiral doublet](../../../../../higgs-chiral-doublet.md) contains a Higgs [complex scalar field](../../../../../complex-scalar-field.md) and a [higgsino](../../../../../higgsino.md). Every [chiral superfield](../../../../../chiral-superfield.md) also has a complex [auxiliary field](../../../../../auxiliary-field.md). The [vector superfields](../../../../../vector-superfield.md) are

$$
\boxed{V_3:(\mathbf8,\mathbf1,0),\qquad V_2:(\mathbf1,\mathbf3,0),\qquad V_1:(\mathbf1,\mathbf1,0).}
$$

They contain the corresponding [gauge bosons](../../../../../gauge-boson.md), [gauginos](../../../../../gaugino.md) in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), and real [auxiliary fields](../../../../../auxiliary-field.md). A right-handed neutrino [chiral superfield](../../../../../chiral-superfield.md) is not part of the minimal field content.

A [gauge anomaly](../../../../../gauge-anomaly.md) is a quantum obstruction to a classical [gauge symmetry](../../../../../gauge-invariance.md). For [hypercharge](../../../../../hypercharge.md), triangle diagrams with left-handed [Weyl spinors](../../../../../weyl-spinor.md) can violate the Ward identity of the [gauge boson](../../../../../gauge-boson.md); an uncancelled [gauge anomaly](../../../../../gauge-anomaly.md) makes the [gauge theory](../../../../../gauge-theory.md) inconsistent. [Anomaly cancellation](../../../../../anomaly-cancellation.md) sums over every component, including colour and weak multiplicities. [Complex scalar fields](../../../../../complex-scalar-field.md) do not contribute to these chiral [gauge anomalies](../../../../../gauge-anomaly.md). For one [fermion generation](../../../../../fermion-generation.md), the cubic [hypercharge](../../../../../hypercharge.md) coefficient is

$$
\begin{aligned}
\mathcal A_{Y^3}
&=6(1/6)^3+3(-2/3)^3+3(1/3)^3+2(-1/2)^3+1^3\\
&=\frac1{36}-\frac89+\frac19-\frac14+1=\boxed{0}.
\end{aligned}
$$

The other coefficients involving a [hypercharge](../../../../../hypercharge.md) [gauge boson](../../../../../gauge-boson.md) vanish too. With the fundamental index $T(\mathbf N)=1/2$,

$$
\begin{aligned}
\mathcal A_{SU(3)^2Y}&=2(1/2)(1/6)+(1/2)(-2/3)+(1/2)(1/3)=0,\\
\mathcal A_{SU(2)^2Y}&=3(1/2)(1/6)+(1/2)(-1/2)=0,\\
\mathcal A_{\mathrm{grav}^2Y}&=6(1/6)+3(-2/3)+3(1/3)+2(-1/2)+1=0.
\end{aligned}
$$

The last line is the [mixed gauge-gravitational anomaly](../../../../../mixed-gauge-gravitational-anomaly.md). Coefficients with one non-Abelian generator and two [hypercharge](../../../../../hypercharge.md) generators vanish by tracelessness. For completeness, the purely colour cubic [gauge anomaly](../../../../../gauge-anomaly.md) cancels between the two fundamental quark components and the two antifundamentals; the weak group has no perturbative cubic [gauge anomaly](../../../../../gauge-anomaly.md). Its four left-handed doublets per [fermion generation](../../../../../fermion-generation.md) also avoid the [Witten SU(2) anomaly](../../../../../witten-su-2-anomaly.md). Thus **each family is separately anomaly-free**, not merely their sum.

The [gauginos](../../../../../gaugino.md) do not spoil this result: their [hypercharge](../../../../../hypercharge.md) is zero and their [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) is real. One extra [Higgs chiral doublet](../../../../../higgs-chiral-doublet.md) is different because its [higgsino](../../../../../higgsino.md) is chiral. For $H_u$, its contributions are

$$
\mathcal A_{Y^3}=2(1/2)^3=1/4,\qquad
\mathcal A_{SU(2)^2Y}=(1/2)(1/2)=1/4,\qquad
\mathcal A_{\mathrm{grav}^2Y}=2(1/2)=1.
$$

They have no compensating contribution from the Higgs [complex scalar field](../../../../../complex-scalar-field.md). The [higgsino](../../../../../higgsino.md) in $H_d$ supplies precisely the negative of each coefficient. **Opposite-hypercharge Higgs chiral doublets restore anomaly cancellation.** The same pair restores an even number of weak fermion doublets, so the [Witten SU(2) anomaly](../../../../../witten-su-2-anomaly.md) provides an additional check of the [higgsino anomaly cancellation](../../../../../higgsino-anomaly-cancellation.md).

The independent reason is the [holomorphic need for two Higgs chiral doublets](../../../../../holomorphic-need-for-two-higgs-chiral-doublets.md). A [superpotential](../../../../../superpotential.md) is a [holomorphic function](../../../../../holomorphic-function.md) of [chiral superfields](../../../../../chiral-superfield.md), so it cannot use a conjugate Higgs [superfield](../../../../../superfield.md) to generate the missing [Yukawa couplings](../../../../../yukawa-interaction.md). The ordinary [Standard Model](../../../../../standard-model-split.md) can use a Higgs scalar and its conjugate, but the [MSSM](../../../../../minimal-supersymmetric-standard-model.md) needs distinct [chiral superfields](../../../../../chiral-superfield.md) of both [hypercharges](../../../../../hypercharge.md). For example,

$$
W_{\rm Yukawa}=y_u^{ij}U_i^c Q_j\mathbin{\cdot}H_u-y_d^{ij}D_i^c Q_j\mathbin{\cdot}H_d-y_e^{ij}E_i^c L_j\mathbin{\cdot}H_d,
$$

where the dot contracts weak indices with the antisymmetric tensor. All three terms are gauge-invariant [holomorphic functions](../../../../../holomorphic-function.md). **$H_u$ supplies up-type masses, while $H_d$ supplies down-type and charged-lepton masses.** Replacing either by the conjugate of the other would violate the [holomorphic closure of chiral superfields](../../../../../holomorphic-closure-of-chiral-superfields.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
