<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [flavor hypercharge](../../../../../flavor-hypercharge.md) $Y=B+S$, where $B$ is [baryon number](../../../../../baryon-number.md) and $S$ is [strangeness](../../../../../strangeness.md). The [isospin](../../../../../isospin.md) coordinate is $I_3$. The [baryon octet](../../../../../baryon-octet.md) has coordinates

$$
\begin{array}{c|rrrrrrrr}
\text{state}&p&n&\Sigma^+&\Sigma^0&\Sigma^-&\Lambda^0&\Xi^0&\Xi^-\\\hline
I_3&\tfrac12&-\tfrac12&1&0&-1&0&\tfrac12&-\tfrac12\\
Y&1&1&0&0&0&0&-1&-1
\end{array}
$$

Here the [nucleons](../../../../../nucleon.md) have $S=0$, the [Sigma baryons](../../../../../sigma-baryon.md) and [Lambda baryon](../../../../../lambda-baryon.md) have $S=-1$, and the [Xi baryons](../../../../../xi-baryon.md) have $S=-2$. The central [Sigma baryon](../../../../../sigma-baryon.md) belongs to an [isospin](../../../../../isospin.md) triplet while the central [Lambda baryon](../../../../../lambda-baryon.md) is an [isospin](../../../../../isospin.md) singlet; equal coordinates do not identify the states.

The pseudoscalar [meson octet](../../../../../meson-octet.md) is

$$
\begin{array}{c|rrrrrrrr}
\text{state}&K^+&K^0&\pi^+&\pi^0&\pi^-&\eta_8&\bar K^0&K^-\\\hline
I_3&\tfrac12&-\tfrac12&1&0&-1&0&\tfrac12&-\tfrac12\\
Y&1&1&0&0&0&0&-1&-1
\end{array}
$$

The [pions](../../../../../pion.md) have $S=0$, the upper [kaons](../../../../../kaon.md) have $S=+1$, and their lower antiparticles have $S=-1$. The two central states are the neutral [pion](../../../../../pion.md) and the [Eta octet state](../../../../../eta-octet-state.md). This is the octet basis of [flavor symmetry](../../../../../flavor-symmetry.md); the physical eta can also mix with the flavor-singlet state.

<a id="4/image-flavor-su-3-baryon-and-pseudoscalar-meson-octets-in-isospin-and-strong-hypercharge-coordinates"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-44-flavor-octets.png)

**[Figure 2](#4/image-flavor-su-3-baryon-and-pseudoscalar-meson-octets-in-isospin-and-strong-hypercharge-coordinates). Flavor SU(3) baryon and pseudoscalar meson octets in isospin and strong hypercharge coordinates**.

For the [flavor SU(3) Cartan generators](../../../../../flavor-su-3-cartan-generators.md), choose the Hermitian physics convention and the [inner product](../../../../../inner-product.md) $\langle A,B\rangle=\operatorname{tr}(AB)$. Then an orthonormal diagonal basis is

$$
\boxed{h_1=\frac1{\sqrt2}\operatorname{diag}(1,-1,0),\qquad h_2=\frac1{\sqrt6}\operatorname{diag}(1,1,-2),\qquad\operatorname{tr}(h_ih_j)=\delta_{ij}.}
$$

Strictly, $ih_1,ih_2$ are elements of the anti-Hermitian [SU(3) Lie algebra](../../../../../su-3-lie-algebra.md); $h_1,h_2$ are the corresponding Hermitian observables. In the quark basis $(u,d,s)$, the up and down [quarks](../../../../../quark.md) form an [isospin](../../../../../isospin.md) doublet and the strange [quark](../../../../../quark.md) is a singlet. Their $I_3$ values are $(1/2,-1/2,0)$. Each [quark](../../../../../quark.md) has [baryon number](../../../../../baryon-number.md) $1/3$, and their [strangeness](../../../../../strangeness.md) values are $(0,0,-1)$. It follows that

$$
\boxed{I_3=\frac{h_1}{\sqrt2},\qquad Y=\sqrt{\frac23}\,h_2=\operatorname{diag}\left(\frac13,\frac13,-\frac23\right).}
$$

These [flavor hypercharge](../../../../../flavor-hypercharge.md) conventions differ from the [electroweak hypercharge](../../../../../hypercharge.md) convention. If instead the inner product is $2\operatorname{tr}(AB)$, the orthonormal basis is $t_3=h_1/\sqrt2$, $t_8=h_2/\sqrt2$, and the same operators are $I_3=t_3$, $Y=2t_8/\sqrt3$.

In the ordinary [quark model](../../../../../quark-model.md), the [proton](../../../../../proton.md) has valence content $uud$ and charge $+1$, while the [neutron](../../../../../neutron.md) has content $udd$ and charge zero. Additivity of [electric charge](../../../../../electric-charge.md) gives $2q_u+q_d=1$ and $q_u+2q_d=0$, hence $q_u=2/3$, $q_d=-1/3$. The [Sigma baryon](../../../../../sigma-baryon.md) $\Sigma^-$ has content $dds$ and charge $-1$, giving $2q_d+q_s=-1$. Thus the [quark](../../../../../quark.md) triplet's [electric charges](../../../../../electric-charge.md), in units of the positive elementary charge, are

$$
\boxed{(q_u,q_d,q_s)=\left(\frac23,-\frac13,-\frac13\right).}
$$

The [Gell-Mann--Nishijima formula](../../../../../gell-mann-nishijima-formula.md) is consequently

$$
\boxed{Q=I_3+\frac Y2=\frac{h_1}{\sqrt2}+\frac{h_2}{\sqrt6}=\operatorname{diag}\left(\frac23,-\frac13,-\frac13\right).}
$$

It also reproduces every [baryon octet](../../../../../baryon-octet.md) charge from the first diagram. On [antiquarks](../../../../../antiquark.md) the additive quantum numbers reverse sign, and combining a [quark](../../../../../quark.md) with an [antiquark](../../../../../antiquark.md) reproduces the [meson octet](../../../../../meson-octet.md) charges.

Because the down and strange [quarks](../../../../../quark.md) have identical [electric charge](../../../../../electric-charge.md), $Q$ commutes with the [U-spin](../../../../../u-spin.md) generators

$$
U_1=\frac{E_{23}+E_{32}}2,\qquad U_2=\frac{E_{23}-E_{32}}{2i},\qquad U_3=\frac12\operatorname{diag}(0,1,-1).
$$

They satisfy $[U_a,U_b]=i\epsilon_{abc}U_c$; equivalently the anti-Hermitian matrices $iU_a$ span an $\mathfrak{su}(2)$ subalgebra. The entries on the $d,s$ block of $Q$ are equal, so **$[Q,U_a]=0$ for all three [U-spin](../../../../../u-spin.md) generators**. The [electric charge](../../../../../electric-charge.md) is therefore constant within each irreducible [U-spin](../../../../../u-spin.md) multiplet. For example, [U-spin](../../../../../u-spin.md) relates $\pi^+$ and $K^+$, and relates $p$ and $\Sigma^+$, without changing their charge. It does not imply exact mass degeneracy: unequal down- and strange-quark masses break [U-spin](../../../../../u-spin.md).

For [pion-nucleon octet channels](../../../../../pion-nucleon-octet-channels.md), assume the collision is governed by the [strong interaction](../../../../../strong-interaction.md). The initial [baryon number](../../../../../baryon-number.md) is one and [strangeness](../../../../../strangeness.md) is zero, so an outgoing [meson](../../../../../meson.md)-[baryon](../../../../../baryon.md) pair must preserve $B=1$, $S=0$, and [electric charge](../../../../../electric-charge.md). Thus its total [flavor hypercharge](../../../../../flavor-hypercharge.md) is $Y=1$. The allowed types are

$$
\boxed{\pi N,\qquad\eta_8N,\qquad K\Lambda,\qquad K\Sigma.}
$$

A [kaon](../../../../../kaon.md) of $S=+1$ can accompany a [Lambda baryon](../../../../../lambda-baryon.md) or [Sigma baryon](../../../../../sigma-baryon.md) of $S=-1$. An antikaon cannot balance the nonpositive [strangeness](../../../../../strangeness.md) of an octet [baryon](../../../../../baryon.md). A [Xi baryon](../../../../../xi-baryon.md) would require a meson of $S=+2$, which the [meson octet](../../../../../meson-octet.md) does not contain.

Resolving these types by [electric charge](../../../../../electric-charge.md) gives all possible pairs:

$$
\begin{array}{c|l|l}
Q&\text{incoming}&\text{outgoing pairs allowed by additive charges}\\\hline
2&\pi^+p&\pi^+p,\ K^+\Sigma^+\\
1&\pi^0p,\ \pi^+n&\pi^+n,\ \pi^0p,\ \eta_8p,\ K^+\Lambda^0,\ K^+\Sigma^0,\ K^0\Sigma^+\\
0&\pi^-p,\ \pi^0n&\pi^-p,\ \pi^0n,\ \eta_8n,\ K^0\Lambda^0,\ K^+\Sigma^-,\ K^0\Sigma^0\\
-1&\pi^-n&\pi^-n,\ K^0\Sigma^-
\end{array}
$$

In the [isospin](../../../../../isospin.md)-symmetric approximation, total [isospin](../../../../../isospin.md) is conserved as well: the incoming $1\otimes\tfrac12$ contains $I=\tfrac12,\tfrac32$. The $\pi N$ and $K\Sigma$ channels contain both values, while $\eta_8N$ and $K\Lambda$ contain only $I=\tfrac12$. The extreme-charge initial states are pure $I=\tfrac32$, consistently excluding $\eta_8N$ and $K\Lambda$. [Clebsch-Gordan coefficients](../../../../../clebsch-gordan-coefficients.md) relate amplitudes in different charge channels; the table establishes permission, not equal probabilities. Electromagnetism and unequal up- and down-quark masses introduce small violations of [isospin](../../../../../isospin.md) symmetry.

Finally, [energy](../../../../../energy.md) and [momentum conservation](../../../../../momentum-conservation.md) require $\sqrt{s}\geq m_M+m_B$ for a particular pair, where $s$ is the squared total [four-momentum](../../../../../four-momentum.md). Only channels above their own threshold can occur. Total [angular momentum](../../../../../angular-momentum.md) and [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md) constrain the [partial waves](../../../../../partial-wave.md) of the [meson-baryon scattering](../../../../../meson-baryon-scattering.md): a pseudoscalar [meson](../../../../../meson.md) and a positive-parity spin-one-half [baryon](../../../../../baryon.md) have pair parity $-(-1)^L$ and total [angular momentum](../../../../../angular-momentum.md) $J=L\pm\tfrac12$ (only $J=\tfrac12$ for $L=0$). Initial and final [partial waves](../../../../../partial-wave.md) must have matching $J$ and parity. Sufficient energy can open a channel, but cannot remove the [electric charge conservation](../../../../../charge-conservation.md), [baryon number](../../../../../baryon-number.md), or [strangeness](../../../../../strangeness.md) constraints.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
