<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Flavour issue in the printed effective interaction.** The displayed charged-current factor uses an [Electron](../../../../../../electron.md) field even for the muon-[neutrino](../../../../../../neutrino.md) term. Taken literally, this introduces an extra $\nu_\mu e$ charged-current interaction, contradicting the Standard Model diagrams in part (a). In the Standard Model that factor uses the charged lepton of the same flavour; for [Electron](../../../../../../electron.md) scattering the charged-current contribution is therefore present only for $\nu_e$. The [weak flavour selection in neutrino-electron scattering](../../../../../../weak-flavour-selection-in-neutrino-electron-scattering.md) fixes the physically consistent assignment used below. The literal printed consequence is given afterwards, so the discrepancy is explicit.

At leading order in the [Electron](../../../../../../electron.md) mass and in the four-fermion regime, define $\Gamma_L^\alpha=\gamma^\alpha(1-\gamma^5)$. The [weak neutral current](../../../../../../neutral-current.md) yields the [scattering amplitude](../../../../../../scattering-amplitude.md)

$$
\boxed{\mathcal M_\mu=-\frac{G_F}{\sqrt2}
[\bar u_\nu(k')\Gamma_L^\alpha u_\nu(k)]
[\bar u_e(p')\gamma_\alpha(c_V-c_A\gamma^5)u_e(p)].}
$$

An overall amplitude phase has no observable effect. The [Fermi interaction](../../../../../../fermi-interaction.md) is valid when the exchanged invariants are small compared with the squared weak-boson masses.

Average over the two initial [Electron](../../../../../../electron.md) spin states, and sum over final spins. There is no averaging over a sterile right-handed incoming [neutrino](../../../../../../neutrino.md). Using the [fermion spin sum](../../../../../../fermion-spin-sum.md), the averaged square is

$$
\overline{|\mathcal M_\mu|^2}=\frac{G_F^2}{4}
\operatorname{Tr}[\not k'\Gamma_L^\alpha\not k\Gamma_L^\beta]\,
\operatorname{Tr}[\not p'\gamma_\alpha(c_V-c_A\gamma^5)
\not p\gamma_\beta(c_V-c_A\gamma^5)].
$$

To display the trace contraction, define

$$
S^{\alpha\beta}(a,b)=a^\alpha b^\beta+a^\beta b^\alpha-g^{\alpha\beta}(a\cdot b),
\qquad E^{\alpha\beta}(a,b)=\epsilon^{\alpha\beta\rho\sigma}a_\rho b_\sigma.
$$

The supplied [gamma matrix trace identities](../../../../../../gamma-matrix-trace-identities.md) give the two tensors $8(S(k',k)+iE(k',k))$ and $4[(c_V^2+c_A^2)S(p',p)+2ic_Vc_AE(p',p)]$. Symmetric-antisymmetric mixed contractions vanish. Set $X=(k'\cdot p')(k\cdot p)$ and $Y=(k'\cdot p)(k\cdot p')$. The remaining contractions are $S(k',k)S(p',p)=2(X+Y)$ and $E(k',k)E(p',p)=-2(X-Y)$, using the stated negative epsilon-contraction sign. Their sum gives

$$
\overline{|\mathcal M_\mu|^2}
=16G_F^2\left[
(c_V+c_A)^2(k\cdot p)(k'\cdot p')
+(c_V-c_A)^2(k\cdot p')(k'\cdot p)\right].
$$

The massless [Mandelstam variables](../../../../../../mandelstam-variables.md) satisfy $s+t+u=0$, and the two products are $s^2/4$ and $u^2/4$, respectively. Therefore

$$
\boxed{\overline{|\mathcal M_\mu|^2}
=4G_F^2\bigl[(c_V+c_A)^2s^2+(c_V-c_A)^2u^2\bigr].}
$$

In the centre-of-momentum frame, momentum conservation gives $E=\sqrt s/2$. If $z=\cos\theta$ is the angle cosine between $p$ and $p'$, then $u=-s(1+z)/2$. The massless [two-body Lorentz-invariant phase space](../../../../../../two-body-lorentz-invariant-phase-space.md) is $d\rho_2=d\Omega/(32\pi^2)$, while the flux is $2s$. Thus

$$
\frac{d\sigma}{dz}=\frac{\overline{|\mathcal M|^2}}{32\pi s}
=\frac{G_F^2s}{8\pi}
\left[(c_V+c_A)^2+\frac14(c_V-c_A)^2(1+z)^2\right].
$$

Integrate $\int_{-1}^1dz=2$ and $\int_{-1}^1(1+z)^2dz=8/3$:

$$
\boxed{\sigma_\mu=\frac{G_F^2s}{4\pi}
\left[(c_V+c_A)^2+\frac13(c_V-c_A)^2\right]
=\frac{G_F^2s}{3\pi}(c_V^2+c_Vc_A+c_A^2).}
$$

Consequently the intended coefficients are

$$
\boxed{F(s)=\frac{s}{3\pi},\qquad A=1,\qquad B=1,\qquad C=0.}
$$

This is the [massless neutrino-electron contact cross-section](../../../../../../massless-neutrino-electron-contact-cross-section.md).

For completeness, the literal printed muon-[neutrino](../../../../../../neutrino.md) charged-current term would instead shift both couplings by one, exactly as in part (c):

$$
\sigma_{\mu,\mathrm{literal}}
=\frac{G_F^2s}{3\pi}
[c_V^2+c_Vc_A+c_A^2+3(c_V+c_A)+3].
$$

For arbitrary real $c_V,c_A$, its linear terms cannot be represented by the requested quadratic form with coupling-independent constants. **The Standard Model result and the literal printed interaction are not the same problem.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
