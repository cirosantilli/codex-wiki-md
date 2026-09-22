<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use metric $(+---)$, $\epsilon^{0123}=+1$ and relativistically normalized external spinors. The [Fermi interaction](../../../../../../fermi-interaction.md) gives

$$
\mathcal M=\frac{G_F}{\sqrt2}\,[\bar v(p_2)\gamma^\alpha(P+Q\gamma^5)u(p_1)]\,[\bar u(k_1)\gamma_\alpha(P+Q\gamma^5)v(k_2)],
$$

up to an irrelevant phase. The [fermion spin sums](../../../../../../fermion-spin-sum.md) replace $u\bar u$ and $v\bar v$ by the slashed massless momenta. Write $C=P^2+Q^2$. The [gamma matrix trace identities](../../../../../../gamma-matrix-trace-identities.md) yield

$$
T^{\alpha\beta}(a,b)=\operatorname{Tr}[\not a\gamma^\alpha(P+Q\gamma^5)\not b\gamma^\beta(P+Q\gamma^5)]=4C(a^\alpha b^\beta+a^\beta b^\alpha-g^{\alpha\beta}a\cdot b)+8iPQ\epsilon^{\alpha\beta\rho\sigma}a_\rho b_\sigma.
$$

The symmetric-antisymmetric mixed contractions vanish. The symmetric contraction is $2[(a\cdot c)(b\cdot d)+(a\cdot d)(b\cdot c)]$, while the two epsilon tensors contract to $-2[(a\cdot c)(b\cdot d)-(a\cdot d)(b\cdot c)]$. Including $G_F^2/2$ and the $1/4$ initial-spin average therefore gives

$$
\overline{|\mathcal M|^2}=4G_F^2\left[(C^2+4P^2Q^2)(p_2\cdot k_1)(p_1\cdot k_2)+(C^2-4P^2Q^2)(p_2\cdot k_2)(p_1\cdot k_1)\right].
$$

The singlet [color charge](../../../../../../color-charge.md) contractions $\delta_{ij}\delta_{kl}$ have net factor one after summing final colours and averaging initial [color charge](../../../../../../color-charge.md) states. Thus this is also the colour-averaged partonic result; no extra factor three is required.

In the [centre-of-momentum frame](../../../../../../center-of-momentum-frame.md), let $c_\theta=\cos\theta$. The [Mandelstam variables](../../../../../../mandelstam-variables.md) satisfy $t=-s(1-c_\theta)/2$ and $u=-s(1+c_\theta)/2$, giving $(p_2\cdot k_1)(p_1\cdot k_2)=s^2(1+c_\theta)^2/16$ and $(p_2\cdot k_2)(p_1\cdot k_1)=s^2(1-c_\theta)^2/16$. Hence

$$
\overline{|\mathcal M|^2}=\frac{G_F^2s^2}{2}\left[C^2(1+c_\theta^2)+8P^2Q^2c_\theta\right].
$$

The massless [invariant flux factor](../../../../../../invariant-flux-factor.md) is $2s$ and $d\Phi_2=d\Omega/(32\pi^2)$, so the [weak charged-current quark scattering](../../../../../../weak-charged-current-quark-scattering.md) cross-section is

$$
\boxed{F(s)=\frac{G_F^2s}{128\pi^2},\qquad H_1=(P^2+Q^2)^2,\qquad H_2=8P^2Q^2.}
$$

For a purely left-handed [weak charged current](../../../../../../charged-current.md), $P=1$, $Q=-1$, this reduces to $d\sigma/d\Omega=G_F^2s(1+\cos\theta)^2/(32\pi^2)$, fixing the sign of the forward term. Purely right-handed [weak charged currents](../../../../../../charged-current.md) at both vertices have the same unpolarized angular law. The factorization convention for $F,H_1,H_2$ could be rescaled by a common numerical factor; the displayed product fixes the normalization.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
