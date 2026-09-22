<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take an oriented [closed string](../../../../../closed-string.md) in flat, critical [bosonic string theory](../../../../../bosonic-string-theory.md), with $\alpha'=1/(2\pi T)$ and a mostly-plus target [Minkowski metric](../../../../../minkowski-metric.md). After continuation of the [worldsheet](../../../../../worldsheet.md) to Euclidean signature, the [Polyakov path integral](../../../../../polyakov-path-integral.md) sums over embeddings $X$ and [worldsheet metrics](../../../../../worldsheet-metric.md), divided by [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../weyl-transformation.md). In a flat target its kinetic [action](../../../../../action.md) is

$$
S_E=\frac1{4\pi\alpha'}\int_\Sigma d^2z\,\sqrt g\,g^{ab}
\partial_aX^m\partial_bX_m.
$$

Target-time continuation or analytic continuation of external momenta defines the Lorentzian scattering amplitude; a naive real Euclidean Gaussian for timelike $X^0$ would not be convergent.

An external [tachyon](../../../../../tachyon.md) is represented by the [tachyon vertex operator](../../../../../tachyon-vertex-operator.md) $V_p(z,\bar z)=:\!e^{ip\cdot X}\!:$, with [conformal weights](../../../../../conformal-weight.md) $h=\bar h=\alpha'p^2/4$. The physical integrated vertex has $(h,\bar h)=(1,1)$, so $p^2=4/\alpha'$. Schematically its tree amplitude is

$$
\mathcal A_N\ \propto\ \int\frac{\mathcal DX\,\mathcal Dg}
{\operatorname{Vol}(\mathrm{Diff}\times\mathrm{Weyl})}
\,e^{-S_E}\prod_{a=1}^N\int_\Sigma d^2z_a\,\sqrt g\,V_{p_a}(z_a,\bar z_a).
$$

The [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) from [conformal gauge](../../../../../conformal-gauge.md) is represented by the [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md). At tree level the [worldsheet](../../../../../worldsheet.md) is a [Riemann sphere](../../../../../riemann-sphere.md), whose unpunctured [complex structure](../../../../../complex-structure.md) has no moduli. Its residual conformal automorphisms are the [Möbius transformations](../../../../../mobius-transformation.md), $PSL(2,\mathbb C)$. Fix three insertion points, accompanying their unintegrated vertices by the required $c\widetilde c$ ghost factors. The remaining $N-3$ complex insertion positions are integrated over the sphere; equivalently one integrates all positions and divides by the residual conformal group.

The embedding fields are free, with

$$
\langle X^m(z)X^n(w)\rangle
=-\frac{\alpha'}2\eta^{mn}\log|z-w|^2.
$$

Their zero-mode integral gives [momentum conservation](../../../../../momentum-conservation.md), and their nonzero-mode [Gaussian integral](../../../../../gaussian-integral.md) gives the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md)

$$
(2\pi)^D\delta^D\!\left(\sum_a p_a\right)
\prod_{a<b}|z_a-z_b|^{\alpha'p_a\cdot p_b}.
$$

This explains the [sphere tachyon position integral](../../../../../sphere-tachyon-position-integral.md) without needing its evaluation. For four [tachyons](../../../../../tachyon.md) the resulting [Virasoro–Shapiro amplitude](../../../../../virasoro-shapiro-amplitude.md) displays the exchanged string spectrum directly.

Use all-incoming external momenta and introduce $u=-(p_1+p_4)^2/(8\pi T)$ alongside the two printed dimensionless [Mandelstam variables](../../../../../mandelstam-variables.md). Since $p_a^2=8\pi T$ and $\sum_a p_a=0$, one obtains $s+t+u=-4$. The physical center-of-mass energy squared in the $s$ channel is $s_{\mathrm{phys}}=8\pi T s=4s/\alpha'$. The $t$ channel measures the analogous crossed [momentum](../../../../../momentum.md) transfer, with sign determined by the mostly-plus convention. Rewriting the Gamma factors in a symmetric form gives

$$
A(s,t)=\prod_{x=s,t,u}\frac{\Gamma(-1-x)}{\Gamma(2+x)}.
$$

The [Gamma function](../../../../../gamma-function.md) [poles](../../../../../pole.md) imply, at generic fixed values of the other invariant,

$$
\boxed{s=n-1\quad\hbox{or}\quad t=n-1,\qquad n=0,1,2,\ldots.}
$$

The denominator Gamma factors can remove [residues](../../../../../residue.md) at special intersecting channel kinematics; the statement concerns a generic single-channel limit. An $s$-channel [pole](../../../../../pole.md) occurs when the intermediate [momentum](../../../../../momentum.md) $p_1+p_2$ satisfies the [mass-shell condition](../../../../../string-mass-shell-condition.md) for a closed-string state:

$$
M_n^2=8\pi T(n-1).
$$

The [pole](../../../../../pole.md) at $s=-1$ exchanges the ground-state [tachyon](../../../../../tachyon.md), the [pole](../../../../../pole.md) at $s=0$ exchanges massless states, and the positive integer [poles](../../../../../pole.md) exchange the infinite massive tower. The $t$-channel interpretation is the crossed version. Factorization means that each [residue](../../../../../residue.md) is a sum of products of couplings to intermediate physical states that couple to the chosen external particles. It need not expose every representation at that mass.

For example, the [Gamma function recurrence](../../../../../gamma-function-recurrence.md) and [Gamma function residue at a nonpositive integer](../../../../../gamma-function-residue-at-a-nonpositive-integer.md) give the dimensionless [Virasoro–Shapiro amplitude pole residue](../../../../../virasoro-shapiro-amplitude-pole-residue.md)

$$
\operatorname*{Res}_{s=n-1}A(s,t)
=-\frac{[(t+2)_n]^2}{(n!)^2},\qquad
(t+2)_n=\prod_{j=0}^{n-1}(t+2+j).
$$

The [residue](../../../../../residue.md) polynomial has degree $2n$, consistent with maximum spin $2n$ in the exchanged level. The amplitude also has the corresponding $u$-channel [poles](../../../../../pole.md) by [crossing symmetry](../../../../../crossing-symmetry.md).

The massless fields can be treated as target backgrounds rather than separate asymptotic insertions. Write the target metric as $G_{mn}=\eta_{mn}+h_{mn}$, introduce a [Kalb–Ramond field](../../../../../kalb-ramond-field.md) $B_{mn}$, and a [dilaton](../../../../../dilaton.md) $\Phi$. In conventional Euclidean signs their [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md) [action](../../../../../action.md) is

$$
S_E[X;G,B,\Phi]=\frac1{4\pi\alpha'}\int d^2z\left[
\sqrt g\,g^{ab}G_{mn}(X)\partial_aX^m\partial_bX^n
+i\epsilon^{ab}B_{mn}(X)\partial_aX^m\partial_bX^n\right]
+\frac1{4\pi}\int d^2z\,\sqrt g\,\Phi(X)R^{(2)}.
$$

Here $\epsilon^{ab}$ is the antisymmetric tensor density. The three backgrounds correspond to the [graviton](../../../../../graviton.md), antisymmetric tensor and scalar states at closed-string level one. Expanding the vacuum functional in $h,B,\Phi$, then Fourier expanding the backgrounds, produces exactly their integrated [string vertex operators](../../../../../string-vertex-operator.md). Its [functional derivatives](../../../../../functional-derivative.md) therefore generate the amplitudes with massless external strings. The connected vacuum functional organizes connected amplitudes; the spacetime effective [action](../../../../../action.md) organizes the corresponding vertices after treating massless propagation consistently.

At momenta small compared with $1/\sqrt{\alpha'}$, massive string propagators can be expanded in powers of momenta over their masses. The analytic part of the amplitudes consequently determines local higher-derivative interactions, ordered by powers of $\alpha'$. Massless exchange [poles](../../../../../pole.md) are retained through propagation of the massless fields, rather than expanded into local contact terms. Up to field redefinitions, the leading massless-sector [action](../../../../../action.md) in the [string-frame metric](../../../../../string-frame-metric.md) is

$$
\boxed{S_{\mathrm{eff}}^{\mathrm{tree}}
=\frac1{2\kappa_0^2}\int d^Dx\,\sqrt{-G}\,e^{-2\Phi}
\left[R+4(\nabla\Phi)^2-\frac1{12}H_{mnp}H^{mnp}+O(\alpha')\right],\qquad H=dB.}
$$

The terms denoted $O(\alpha')$ contain additional derivatives, including curvature-squared terms in the bosonic theory. The expansion concerns the massless sector around the perturbative bosonic background; the [tachyon](../../../../../tachyon.md) instability remains and is not cured by omitting its field from this displayed [action](../../../../../action.md). Thus this is a formal perturbative effective description, not a claim of a stable bosonic vacuum.

Finally split the [dilaton](../../../../../dilaton.md) into a constant and its variation, $\Phi=\Phi_0+\phi$. By the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md), its [dilaton Euler-characteristic weighting](../../../../../dilaton-euler-characteristic-weighting.md) on a connected closed oriented surface follows from

$$
S_{\Phi_0}=\frac{\Phi_0}{4\pi}\int_\Sigma\sqrt g\,R^{(2)}
=\Phi_0\chi(\Sigma)=\Phi_0(2-2g).
$$

Define the [string coupling](../../../../../string-coupling.md) by **$g_s=e^{\Phi_0}$**. A genus-$g$ path integral is weighted by

$$
\boxed{e^{-S_{\Phi_0}}=g_s^{2g-2}.}
$$

The sphere carries $g_s^{-2}$, the torus carries $g_s^0$, and each extra handle adds $g_s^2$. At higher genus one integrates over complex-structure moduli as well as insertion points, with the associated antighost insertions supplying the correct moduli measure. With canonically normalized external vertices an $N$-point genus-$g$ amplitude scales as $g_s^{2g-2+N}$.

Summing connected [worldsheets](../../../../../worldsheet.md) of every [genus of a surface](../../../../../genus-of-a-surface.md) yields the [string-loop effective action expansion](../../../../../string-loop-effective-action-expansion.md)

$$
\boxed{S_{\mathrm{eff}}=
\sum_{g=0}^{\infty}g_s^{2g-2}\,S_g[G,B,\phi;\alpha'].}
$$

Each coefficient has its own low-energy $\alpha'$ expansion. The two parameters have different roles: $\alpha'$ resolves finite string size through higher derivatives, while $g_s^2$ counts additional string loops.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
