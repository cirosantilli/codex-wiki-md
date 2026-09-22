<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an oriented Euclidean [string worldsheet](../../../../../worldsheet.md) with metric $h_{ab}$, use the [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md) action

$$
S_E=\frac1{4\pi\alpha'}\int d^2\sigma\,
\left[\sqrt h\,h^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+i\epsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+\alpha'\sqrt h\,\Phi(X)R^{(2)}(h)\right].
$$

Here $\epsilon^{ab}$ is an antisymmetric density with $\epsilon^{12}=1$. The factor $i$ in the Euclidean [Kalb–Ramond field](../../../../../kalb-ramond-field.md) term follows from continuing the real Lorentzian two-form coupling; reversing orientation or the convention for $B$ reverses its sign. The conventional positive Euclidean [dilaton](../../../../../dilaton.md) coupling is being used. With [worldsheet](../../../../../worldsheet.md) boundaries its curvature coupling also needs $\int_{\partial\Sigma}\Phi k\,ds/(2\pi)$, where $k$ is the boundary geodesic curvature, to have the proper topological normalization for constant $\Phi$.

All three terms are invariant under [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md). Target-coordinate changes act on $X,G,B,\Phi$ by their ordinary scalar and tensor transformation rules, making the target description covariant as well. For the two-form there is also the target [gauge symmetry](../../../../../gauge-invariance.md) $B\mapsto B+d\Lambda$. Its change in the closed-worldsheet action is an integral of an exact two-form and hence zero. With boundaries it is instead $i\int_{\partial\Sigma}X^*\Lambda/(2\pi\alpha')$; an endpoint [gauge field](../../../../../gauge-field.md) with $\delta A=-\Lambda/(2\pi\alpha')$ cancels it.

Under a local [Weyl transformation](../../../../../weyl-transformation.md) $h_{ab}\mapsto e^{2\omega}h_{ab}$, the metric term is invariant because the two-dimensional factors $\sqrt h$ and $h^{ab}$ cancel. The $B$ term is independent of $h$ and is separately invariant. The curvature transforms as

$$
\sqrt hR^{(2)}\longmapsto\sqrt h(R^{(2)}-2\nabla_h^2\omega).
$$

On a closed surface the [dilaton](../../../../../dilaton.md) variation is consequently

$$
\delta_\omega S_\Phi=-\frac1{2\pi}\int\sqrt h\,\Phi(X)\nabla_h^2\omega
=-\frac1{2\pi}\int\sqrt h\,\omega\nabla_h^2\Phi(X).
$$

Thus a general nonconstant [dilaton](../../../../../dilaton.md) term is not separately invariant under [Weyl transformations](../../../../../weyl-transformation.md). Its variation is the [Weyl variation of a nonconstant dilaton coupling](../../../../../weyl-variation-of-a-nonconstant-dilaton-coupling.md); it vanishes for constant $\Phi$ after the boundary completion where necessary.

For $\Phi=\Phi_0$, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives $S_\Phi=\Phi_0\chi(\Sigma)$. In the [Euclidean path integral](../../../../../euclidean-path-integral.md) the resulting weight is

$$
\boxed{e^{-S_\Phi}=g_s^{-\chi(\Sigma)},\qquad g_s=e^{\Phi_0}.}
$$

For a connected orientable genus-$g$ surface with $b$ boundaries, $\chi=2-2g-b$, so the weight is $g_s^{2g+b-2}$. A closed-string handle therefore adds two powers of [string coupling](../../../../../string-coupling.md). External vertex normalizations add their own coupling factors; they are distinct from this [dilaton Euler-characteristic weighting](../../../../../dilaton-euler-characteristic-weighting.md). The constant [dilaton](../../../../../dilaton.md) controls the [string genus expansion](../../../../../string-genus-expansion.md), rather than adding a force to the classical embedding equation.

Quantization treats the target fields as position-dependent couplings of a two-dimensional interacting [quantum field theory](../../../../../quantum-field-theory-split.md). Expanding $X$ around a background embedding gives fluctuation vertices involving target curvature and [derivatives](../../../../../derivative.md) of $B$ and $\Phi$. Short-distance contractions require local [counterterms](../../../../../counterterm.md), so the target fields become renormalized couplings. In particular a curvature vertex contracted once yields a [Ricci tensor](../../../../../ricci-tensor.md) [counterterm](../../../../../counterterm.md) proportional to $\alpha'R_{\mu\nu}$. Each additional sigma-model loop brings another power of $\alpha'$ and more target [derivatives](../../../../../derivative.md). The expansion is useful when the target variation scale is large compared with $\sqrt{\alpha'}$; it is not the separate expansion in powers of $g_s$.

After [gauge fixing](../../../../../gauge-fixing.md), a [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md) would make amplitudes depend on the discarded local conformal factor. Quantum consistency therefore requires the trace anomaly to vanish, including the reparameterization [worldsheet ghost field](../../../../../worldsheet-ghost-field.md) contribution. In a conventional [renormalization scheme](../../../../../renormalization-scheme.md) the resulting [bosonic sigma-model Weyl anomaly coefficients](../../../../../bosonic-sigma-model-weyl-anomaly-coefficients.md) start as

$$
\begin{aligned}
\overline\beta^G_{\mu\nu}
&=\alpha'\left[R_{\mu\nu}-\frac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}
+2\nabla_\mu\nabla_\nu\Phi\right]+O(\alpha'^2),\\
\overline\beta^B_{\mu\nu}
&=\alpha'\left[-\frac12\nabla^\rho H_{\rho\mu\nu}
+(\nabla^\rho\Phi)H_{\rho\mu\nu}\right]+O(\alpha'^2),\\
\overline\beta^\Phi
&=\frac{d-26}{6}
+\alpha'\left[(\nabla\Phi)^2-\frac12\nabla^2\Phi-\frac1{24}H_{\mu\nu\rho}H^{\mu\nu\rho}\right]
+O(\alpha'^2),\qquad H=dB.
\end{aligned}
$$

The barred quantities include the [dilaton](../../../../../dilaton.md) [stress-energy tensor improvement](../../../../../stress-energy-tensor-improvement.md); ordinary coupling [sigma-model beta functions](../../../../../sigma-model-beta-function.md) can differ by field redefinitions or target diffeomorphisms. Setting these coefficients to zero gives differential equations for the background fields order by order, including the metric gravitational equation and the antisymmetric-field equation. These conventions for the leading coefficients are described in [the background-field lecture notes](https://davidtong.org/pdfs/teaching/string-theory/string7.pdf). Higher orders supply higher-curvature and higher-derivative corrections. This explains how spacetime dynamics follows from quantum gauge consistency of the [worldsheet](../../../../../worldsheet.md), not from asking only for a classical stationary [worldsheet](../../../../../worldsheet.md) in an arbitrarily chosen background.

The apparently noninvariant [dilaton](../../../../../dilaton.md) term is essential outside the critical dimension because its [stress-energy tensor improvement](../../../../../stress-energy-tensor-improvement.md) can cancel the quantum [central charge](../../../../../central-charge.md) mismatch. A flat constant-dilaton background has matter [central charge](../../../../../central-charge.md) $d$ and [worldsheet ghost field](../../../../../worldsheet-ghost-field.md) [central charge](../../../../../central-charge.md) $-26$. If $d\ne26$, changing the constant value of $\Phi$ only changes $g_s$ and cannot cure that mismatch.

A concrete solution is the [linear dilaton conformal field theory](../../../../../linear-dilaton-conformal-field-theory.md) with $G=\eta$, $B=0$, and $\Phi=\Phi_0+V_\mu X^\mu$. Its metric and antisymmetric-field anomaly coefficients vanish, while the scalar condition is

$$
\boxed{V^2=\frac{26-d}{6\alpha'}.}
$$

One can also see this cancellation directly from the improved [holomorphic stress-energy tensor](../../../../../holomorphic-stress-energy-tensor.md). With the positive Euclidean curvature convention above,

$$
T(z)=-\frac1{\alpha'}:\partial X\cdot\partial X:
+V\cdot\partial^2X.
$$

The free-field contraction is $X^\mu(z)X^\nu(w)\sim-\alpha'\eta^{\mu\nu}\log(z-w)/2$. Differentiating it twice at each point gives a fourth-order pole $3\alpha'V^2/(z-w)^4$ from the improvement. Since the fourth-order stress-tensor pole is $c/2$, the matter [central charge](../../../../../central-charge.md) becomes $c=d+6\alpha'V^2=26$. The [worldsheet ghost field](../../../../../worldsheet-ghost-field.md) contribution then cancels it. This is why a classical Weyl variation need not mean inconsistency: it can cancel the quantum variation of the other terms. For $d<26$ the required gradient is spacelike; for $d>26$ it is timelike in the Lorentzian target theory. Such backgrounds are not flat constant-dilaton Minkowski vacua with full target Lorentz symmetry, nor does a [central charge](../../../../../central-charge.md) cancellation by itself prove stability or [unitarity](../../../../../unitary-operator.md) of every noncritical background. If the conformal factor is instead retained dynamically, its [Liouville field theory](../../../../../liouville-field-theory.md) supplies the corresponding noncritical description.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
