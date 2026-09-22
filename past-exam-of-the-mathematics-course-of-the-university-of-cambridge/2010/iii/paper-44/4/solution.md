<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose a Euclidean [string worldsheet](../../../../../worldsheet.md) and the usual normalization of the [Polyakov action](../../../../../polyakov-action.md). For a closed oriented worldsheet $\Sigma$, the [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md) is

$$
\boxed{\begin{aligned}
S={}&\frac1{4\pi\alpha'}\int_\Sigma d^2\sigma\sqrt g\,g^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu\\
&+\frac{i}{4\pi\alpha'}\int_\Sigma d^2\sigma\,\varepsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+\frac1{4\pi}\int_\Sigma d^2\sigma\sqrt g\,\Phi(X)R^{(2)}.
\end{aligned}}
$$

Here $\varepsilon^{12}=1$ is the alternating density, not the tensor with components $1/\sqrt g$. The imaginary coefficient in the [Kalb–Ramond field](../../../../../kalb-ramond-field.md) term is the Euclidean continuation; in Lorentzian signature this term is real. $G$ is the spacetime metric and $\Phi$ the [dilaton](../../../../../dilaton.md).

All three terms have [worldsheet diffeomorphism](../../../../../worldsheet-diffeomorphism.md) invariance, and are covariant under [spacetime](../../../../../spacetime.md) coordinate transformations when $X$, $G$, $B$ and $\Phi$ are transformed together. Under a [Weyl transformation](../../../../../weyl-transformation.md) $g_{ab}\mapsto e^{2\omega}g_{ab}$, $\sqrt g\,g^{ab}$ is invariant in two dimensions, so the metric coupling has classical [Weyl invariance](../../../../../weyl-transformation.md). The antisymmetric coupling is independent of the [worldsheet metric](../../../../../worldsheet-metric.md), so it too has classical [Weyl invariance](../../../../../weyl-transformation.md).

The curvature coupling requires care. An infinitesimal [Weyl transformation](../../../../../weyl-transformation.md) gives $\delta_\omega(\sqrt gR^{(2)})=-2\sqrt g\,\Delta_g\omega$. Integration by parts on the closed worldsheet therefore gives the [Weyl variation of a nonconstant dilaton coupling](../../../../../weyl-variation-of-a-nonconstant-dilaton-coupling.md):

$$
\delta_\omega S_\Phi=-\frac1{2\pi}\int_\Sigma\sqrt g\,\Phi(X)\Delta_g\omega=-\frac1{2\pi}\int_\Sigma\sqrt g\,\omega\Delta_g\Phi(X).
$$

**A constant dilaton coupling is topological and Weyl invariant; a general varying dilaton coupling is not separately classically Weyl invariant.** Its classical variation participates in canceling the quantum [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md), producing the improved background equations below.

To relate these background couplings to the flat-space [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md), expand $G_{\mu\nu}=\eta_{\mu\nu}+h_{\mu\nu}(X)$ and express $h$ and $B$ as superpositions of plane waves. The perturbation of the action is a sum of [integrated string vertex operators](../../../../../integrated-string-vertex-operator.md) of the form

$$
\int d^2z\,\epsilon_{\mu\nu}:\partial X^\mu\bar\partial X^\nu e^{ip\cdot X}:.
$$

This is the vertex of $\alpha_{-1}^\mu\widetilde\alpha_{-1}^\nu|p\rangle$ in the [massless first closed-string level](../../../../../massless-first-closed-string-level.md). Its [conformal weights](../../../../../conformal-weight.md) are $(1+\alpha'p^2/4,1+\alpha'p^2/4)$, so marginality gives $p^2=0$. The [primary operator](../../../../../primary-field.md) conditions give transversality, and the [string-state gauge redundancy](../../../../../string-state-gauge-redundancy.md) removes longitudinal components. The symmetric trace-free [polarization tensor](../../../../../polarization-tensor.md) is the [graviton](../../../../../graviton.md) and perturbs $G$; its antisymmetric part is the [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and perturbs $B$. The scalar physical polarization is the [dilaton](../../../../../dilaton.md). At the level of background fields its vertex involves the metric trace and the curvature improvement, so an arbitrary off-shell metric trace should not simply be identified with the physical dilaton without this distinction.

The spacetime [gauge invariance](../../../../../gauge-invariance.md) of the antisymmetric coupling is

$$
\boxed{B\longmapsto B+d\Lambda,\qquad \delta B_{\mu\nu}=\partial_\mu\Lambda_\nu-\partial_\nu\Lambda_\mu,\qquad H=dB.}
$$

Indeed its action is $S_B=i(2\pi\alpha')^{-1}\int_\Sigma X^*B$. Its variation is

$$
\delta S_B=\frac{i}{2\pi\alpha'}\int_\Sigma d(X^*\Lambda)=\frac{i}{2\pi\alpha'}\int_{\partial\Sigma}X^*\Lambda=0
$$

for a closed worldsheet, by [Stokes theorem](../../../../../stokes-theorem.md). In components this is the total derivative $\partial_a(\varepsilon^{ab}\Lambda_\nu(X)\partial_bX^\nu)$: the term containing $\partial_a\partial_bX^\nu$ vanishes by antisymmetry. Thus only the [Kalb-Ramond field strength](../../../../../kalb-ramond-field-strength.md) $H$ can enter the local spacetime equations. With boundaries, a compensating boundary gauge-field transformation is needed.

Separate the [dilaton](../../../../../dilaton.md) into a constant $\Phi_0$ and a varying part. The [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives

$$
\frac1{4\pi}\int_\Sigma\sqrt g\,R^{(2)}=\chi(\Sigma)=2-2g
$$

for a connected closed orientable genus-$g$ worldsheet. Its Euclidean path-integral weight contains

$$
\boxed{e^{-S_{\Phi_0}}=e^{-(2-2g)\Phi_0}=g_s^{2g-2},\qquad g_s=e^{\Phi_0}.}
$$

Consequently the sum over worldsheet topologies is the [string genus expansion](../../../../../string-genus-expansion.md) $\sum_{g\ge0}g_s^{2g-2}\mathcal A_g$, with each coefficient integrating over that genus's [worldsheet moduli](../../../../../worldsheet-moduli.md). Each extra handle costs $g_s^2$, which is the loop-counting factor of [string perturbation theory](../../../../../string-perturbation-theory.md). With the usual normalization of $n$ external closed-string vertices, the connected amplitude carries $g_s^{2g-2+n}$. This [dilaton Euler-characteristic weighting](../../../../../dilaton-euler-characteristic-weighting.md) is distinct from the expansion in $\alpha'$ of a fixed-worldsheet [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md).

Finally quantize that two-dimensional theory. The background fields are its couplings. The [background field expansion of a string sigma model](../../../../../background-field-expansion-of-a-string-sigma-model.md), $X=x+\xi$ in target-space [normal coordinates](../../../../../normal-coordinates.md), contains curvature vertices quadratic in the fluctuation $\xi$. Contracting their two fluctuation indices produces the [Ricci tensor](../../../../../ricci-tensor.md) multiplying $\partial x^\mu\bar\partial x^\nu$. Logarithmic short-distance contractions renormalize $G$, $B$, and $\Phi$, giving functional [sigma-model beta functions](../../../../../sigma-model-beta-function.md). Gauge independence requires vanishing of the [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md), including the classical improvement from the varying [dilaton](../../../../../dilaton.md), not merely an arbitrary choice of renormalization scale.

For clarity, in conventional leading-order normalization the improved coefficients are

$$
\begin{aligned}
\overline\beta^G_{\mu\nu}&=\alpha'\left(R_{\mu\nu}-\frac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}+2\nabla_\mu\nabla_\nu\Phi\right)+O(\alpha'^2),\\
\overline\beta^B_{\mu\nu}&=\alpha'\left(-\frac12\nabla^\rho H_{\rho\mu\nu}+\nabla^\rho\Phi\,H_{\rho\mu\nu}\right)+O(\alpha'^2),\\
\overline\beta^\Phi&=\frac{D-26}{6}+\alpha'\left((\nabla\Phi)^2-\frac12\nabla^2\Phi-\frac1{24}H^2\right)+O(\alpha'^2).
\end{aligned}
$$

Here $H^2=H_{\mu\nu\rho}H^{\mu\nu\rho}$. The constant term in the [dilaton](../../../../../dilaton.md) coefficient is the matter-plus-ghost [central charge](../../../../../central-charge.md) deficit. At $D=26$, setting these coefficients to zero gives the leading spacetime field equations

$$
\boxed{\begin{aligned}
R_{\mu\nu}-\frac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}+2\nabla_\mu\nabla_\nu\Phi&=0,\\
\nabla^\rho(e^{-2\Phi}H_{\rho\mu\nu})&=0,\\
R+4\nabla^2\Phi-4(\nabla\Phi)^2-\frac1{12}H^2&=0.
\end{aligned}}
$$

For the last equation, take the trace of the first, $R-H^2/4+2\nabla^2\Phi=0$, and combine it with $\overline\beta^\Phi=0$; this verifies the coefficients and signs. These are equivalently the equations from the leading [string-frame massless effective action](../../../../../string-frame-massless-effective-action.md)

$$
S_{\rm eff}\propto\int d^{26}x\sqrt{-G}\,e^{-2\Phi}\left(R+4(\nabla\Phi)^2-\frac1{12}H^2\right).
$$

Higher worldsheet orders give higher-derivative $\alpha'$ corrections, whereas additional handles give string-loop corrections controlled by $g_s$. Thus quantum consistency of a two-dimensional [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md) determines the dynamics of its spacetime background fields. These leading coefficient conventions agree with [the primary string-theory lectures' background-field calculation](https://arxiv.org/html/0908.0333v3).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
