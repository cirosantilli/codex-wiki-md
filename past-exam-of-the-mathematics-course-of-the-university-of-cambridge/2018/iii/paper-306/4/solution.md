<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [closed string](../../../../../closed-string.md) already contains the particle required for [quantum gravity](../../../../../quantum-gravity.md). For [bosonic string theory](../../../../../bosonic-string-theory.md) in its [critical dimension of string theory](../../../../../critical-dimension-of-string-theory.md), the [mass-shell condition](../../../../../string-mass-shell-condition.md) and [closed-string level matching](../../../../../closed-string-level-matching.md) are

$$
M^2=\frac4{\alpha'}(N-1),\qquad N=\widetilde N,
\qquad \alpha'=\frac1{2\pi T}.
$$

At $N=\widetilde N=1$, the states $\epsilon_{mn}\alpha_{-1}^m\widetilde\alpha_{-1}^n|0;k\rangle$ are massless. After imposing the [Virasoro constraints](../../../../../virasoro-constraint.md) and quotienting [null string states](../../../../../null-string-state.md), the transverse [polarization tensor](../../../../../polarization-tensor.md) decomposes into symmetric trace-free, antisymmetric and scalar pieces under $SO(D-2)$. They describe a [graviton](../../../../../graviton.md), the [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and the [dilaton](../../../../../dilaton.md). In particular, **the symmetric trace-free sector is a massless spin-two [graviton](../../../../../graviton.md)**. Its number of [degrees of freedom](../../../../../degree-of-freedom.md) is $D(D-3)/2$.

The [state–operator correspondence](../../../../../state-operator-correspondence.md) associates each [physical string state](../../../../../physical-string-state.md) with a [string vertex operator](../../../../../string-vertex-operator.md). For example, the matter part of a [massless closed-string vertex operator](../../../../../massless-closed-string-vertex-operator.md) is

$$
V_{\epsilon,k}(z,\bar z)=\epsilon_{mn}:\partial X^m\bar\partial X^n e^{ik\cdot X}:,
\qquad k^2=0,\qquad k^m\epsilon_{mn}=k^n\epsilon_{mn}=0.
$$

Its [conformal weights](../../../../../conformal-weight.md) are $(1,1)$, so its integrated form $\int d^2z\,V_{\epsilon,k}$ is invariant under changes of [string worldsheet](../../../../../worldsheet.md) coordinates. At fixed insertion positions it is accompanied by $c\bar c$ from the [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md). Physical vertices represent [BRST cohomology](../../../../../brst-cohomology.md) classes; longitudinal changes of the [polarization tensor](../../../../../polarization-tensor.md) are [BRST-exact operators](../../../../../brst-exact-operator.md) and decouple from physical [scattering amplitudes](../../../../../scattering-amplitude.md). For the [graviton](../../../../../graviton.md), this [string-state gauge redundancy](../../../../../string-state-gauge-redundancy.md) becomes the linearized target-space [diffeomorphism](../../../../../diffeomorphism.md) $h_{mn}\mapsto h_{mn}+\partial_m\xi_n+\partial_n\xi_m$.

The [Polyakov path integral](../../../../../polyakov-path-integral.md) computes a [closed-string scattering amplitude](../../../../../closed-string-scattering-amplitude.md) by inserting the external [string vertex operators](../../../../../string-vertex-operator.md), integrating their unfixed positions and the inequivalent [worldsheet moduli](../../../../../worldsheet-moduli.md), and including the [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md). On a [Riemann sphere](../../../../../riemann-sphere.md) three positions are fixed by the residual conformal group. For example, contractions of [tachyon vertex operators](../../../../../tachyon-vertex-operator.md) produce the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md), whose position integral gives the [Virasoro–Shapiro amplitude](../../../../../virasoro-shapiro-amplitude.md).

The [string dual resonance](../../../../../string-dual-resonance.md) property means that one [crossing-symmetric scattering amplitude](../../../../../crossing-symmetry.md) has equivalent expansions in the different channels: its poles exhibit intermediate string states in each channel, rather than separate channel contributions being added again. The [scattering-amplitude factorization](../../../../../scattering-amplitude-factorization.md) at a [pole](../../../../../pole.md) identifies the intermediate particle and its couplings. Set $8\pi T=1$, so $\alpha'=4$ and the closed-string [tachyon](../../../../../tachyon.md) has $M^2=-1$. For four such external states the [Mandelstam variables](../../../../../mandelstam-variables.md) obey $s+t+u=-4$. The [Virasoro–Shapiro amplitude](../../../../../virasoro-shapiro-amplitude.md) has generic $s$-channel [poles](../../../../../pole.md) at $s=-1,0,1,\ldots$, exactly the [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md) in these units.

The massless [pole](../../../../../pole.md) gives an especially direct check. With overall normalization $C$ and $u=-4-s-t$, the [Gamma function recurrence](../../../../../gamma-function-recurrence.md) gives

$$
\lim_{s\to0}sA(s,t)
=C\frac{\Gamma(-1-t)\Gamma(3+t)}{\Gamma(-2-t)\Gamma(2+t)}
=-C(t+2)^2.
$$

Thus

$$
\boxed{A(s,t)=-\frac{C(t+2)^2}{s}+O(1)\qquad(s\to0).}
$$

The quadratic [residue](../../../../../residue.md) in $t$ contains a spin-two exchange. A scalar exchange alone could not give this angular dependence. Combined with the known massless spectrum and [scattering-amplitude factorization](../../../../../scattering-amplitude-factorization.md), it identifies exchange of the [graviton](../../../../../graviton.md), with possible scalar contributions from the [dilaton](../../../../../dilaton.md); the antisymmetric [Kalb–Ramond field](../../../../../kalb-ramond-field.md) does not couple to two identical scalar [tachyons](../../../../../tachyon.md) here. Consequently the [graviton](../../../../../graviton.md) participates in interactions, rather than being an isolated free state.

Decoupling longitudinal [graviton](../../../../../graviton.md) polarizations forces a universal coupling to the conserved [stress-energy tensor](../../../../../stress-energy-tensor.md). Consistency of this massless spin-two [gauge invariance](../../../../../gauge-invariance.md) extends the linearized coupling to the nonlinear dynamics of [general relativity](../../../../../general-relativity-split.md). At distances large compared with $\sqrt{\alpha'}$, the gravitational sector of the effective [action](../../../../../action.md) begins with the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md), alongside [dilaton](../../../../../dilaton.md) and [Kalb–Ramond field](../../../../../kalb-ramond-field.md) terms and higher-derivative string corrections. The infinite tower of string states supplies the short-distance completion of this [quantum gravity](../../../../../quantum-gravity.md) expansion.

Interactions are organized by [string worldsheet](../../../../../worldsheet.md) topology. A constant [dilaton](../../../../../dilaton.md) gives the [string coupling](../../../../../string-coupling.md) $g_s=e^{\Phi_0}$, and a connected oriented surface of [genus](../../../../../genus-of-a-surface.md) $g$ has [Euler characteristic](../../../../../euler-characteristic.md) $\chi=2-2g$. Its weight is $g_s^{-\chi}$; with $n$ normalized external vertices,

$$
\boxed{\mathcal A_n=\sum_{g=0}^{\infty}g_s^{2g-2+n}\mathcal A_{g,n}.}
$$

The [sphere](../../../../../sphere.md) is tree order, the [torus](../../../../../torus.md) is one loop, and each additional handle adds a factor $g_s^2$. Each coefficient is an integral over [worldsheet moduli](../../../../../worldsheet-moduli.md), so this is [string perturbation theory](../../../../../string-perturbation-theory.md) in $g_s$, with an independent low-energy expansion in $\alpha'$.

For the one-loop vacuum contribution, [torus modular invariance](../../../../../torus-modular-invariance.md) identifies $\tau$ with $(a\tau+b)/(c\tau+d)$, $ad-bc=1$. Integration is over the [standard fundamental domain of the modular group](../../../../../standard-fundamental-domain-of-the-modular-group.md),

$$
\mathcal F=\{\tau=\tau_1+i\tau_2:\ |\tau_1|\leq\tfrac12,\ |\tau|\geq1,\ \tau_2>0\},
\qquad \tau_2\geq\frac{\sqrt3}{2}.
$$

The potential short-proper-time region $\tau_2\to0$, responsible for a point-particle [ultraviolet divergence](../../../../../ultraviolet-divergence.md), is absent. It would count metrics already represented elsewhere in $\mathcal F$. [Torus modular invariance](../../../../../torus-modular-invariance.md) is therefore the geometric reason for one-loop ultraviolet finiteness. More explicitly, in $D=26$ the vacuum integrand is proportional to $d^2\tau\,\tau_2^{-14}|\eta(\tau)|^{-48}$, with $\eta$ the [Dedekind eta function](../../../../../dedekind-eta-function.md); the complete expression is invariant under the [modular group](../../../../../modular-group.md).

**Ultraviolet finiteness does not make the bosonic one-loop vacuum energy finite.** The remaining long-tube region $\tau_2\to\infty$ is an [infrared divergence](../../../../../infrared-divergence.md) from the [tachyon](../../../../../tachyon.md): $|\eta(\tau)|^{-48}\sim e^{4\pi\tau_2}$. It signals instability of the bosonic vacuum. Tachyon-free consistent backgrounds remove this particular obstruction, though other infrared effects must still be treated. The ultraviolet improvement comes from the extended string and the complete spectrum together with the worldsheet gauge identifications; the [genus](../../../../../genus-of-a-surface.md) expansion remains a perturbative description of [quantum gravity](../../../../../quantum-gravity.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
