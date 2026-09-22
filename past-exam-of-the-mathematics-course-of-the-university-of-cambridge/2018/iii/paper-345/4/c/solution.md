<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Exner equation](../../../../../../exner-equation.md) is solid-volume [mass conservation](../../../../../../mass-conservation.md): a downstream increase in [sediment transport](../../../../../../sediment-transport.md) flux removes material and lowers the bed. The factor $\phi_b$ converts bed-height change into solid-volume change. The [saturation length](../../../../../../saturation-length.md) equation models downstream adjustment of actual [sediment transport](../../../../../../sediment-transport.md) to the [equilibrium sediment flux](../../../../../../equilibrium-sediment-flux.md). Grain acceleration and entrainment/deposition need a finite distance, so $q$ lags $q_{\mathrm{sat}}$. The last relation is an empirical transport law above the [sediment entrainment threshold](../../../../../../sediment-entrainment-threshold.md), with $\chi>0$ and normally $\gamma>0$; below threshold it must be interpreted with a [positive part](../../../../../../positive-part-of-a-real-valued-function.md) rather than raising negative excess stress to an arbitrary power. It is a constitutive closure, not a consequence of [mass conservation](../../../../../../mass-conservation.md).

Take the physical parameters $L_{\mathrm{sat}}>0$, $\phi_b>0$, $\chi>0$ and $\gamma>0$. Linearize about a horizontal, uniformly transporting bed with $\Delta=\tau_0-\tau_{\mathrm{th},0}>0$ and $q_0=\phi_b\chi\Delta^\gamma$. Set $\lambda=\sigma-ikc$ and use the real parts of

$$
\eta=\hat\eta e^{\lambda t+ikx},\qquad
q=q_0+\hat q e^{\lambda t+ikx},\qquad
q_{\mathrm{sat}}=q_0+\hat q_{\mathrm{sat}}e^{\lambda t+ikx},\qquad
\tau=\tau_0+\hat\tau e^{\lambda t+ikx}.
$$

The locally planar approximation uses the small instantaneous bed slope to compute the [inclined-bed sediment threshold](../../../../../../inclined-bed-sediment-threshold.md). Since $\alpha=\eta_x+O(\eta_x^3)$,

$$
\boxed{\hat\tau_{\mathrm{th}}=\frac{ik\tau_{\mathrm{th},0}}{\mu_s}\hat\eta}.
$$

A sinusoidal disturbance has both uphill and downhill slopes: the printed $0<\alpha\ll1$ describes the uphill derivation, and its first-order continuation applies to both signs. The zero-slope reference is the one implicit in the printed decomposition with constant term $\tau_{\mathrm{th},0}$; a finite mean inclined bed would require a shifted base threshold.

Define $C=\chi\gamma\Delta^{\gamma-1}$. The linearized transport equations are

$$
\boxed{\phi_b\lambda\hat\eta=-ik\hat q,\qquad
(1+ikL_{\mathrm{sat}})\hat q=\hat q_{\mathrm{sat}},\qquad
\hat q_{\mathrm{sat}}=\phi_bC\left(\hat\tau-\frac{ik\tau_{\mathrm{th},0}}{\mu_s}\hat\eta\right)}.
$$

The [linearization](../../../../../../linearization.md) requires $|\eta_x|\ll1$ and $|\hat\tau-\hat\tau_{\mathrm{th}}|\ll\Delta$.

**A fluid-dynamical shear-response closure is missing from the printed question.** The three sediment equations and local slope correction do not determine $\hat\tau$ from $\hat\eta$. Write the general [bed shear response](../../../../../../bed-shear-response.md) as $\hat\tau=\mathcal T(k)\hat\eta$. A frequently used scale-invariant closure for $k>0$ is

$$
\boxed{\mathcal T(k)=\tau_0k(A+iB)}.
$$

Here $A$ is the component in phase with bed height and $B$ represents an upstream phase lead in bed [shear stress](../../../../../../shear-stress.md). They require an independent flow model and can depend on $k$. Introducing them explicitly makes the [linear stability analysis](../../../../../../linear-stability.md) complete conditional on a specified flow response; it does not turn them into data supplied by the question. An example of this hydrodynamic closure is given in [Fourrière, Claudin and Andreotti's bedform-instability analysis](https://arxiv.org/abs/0805.3417).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
