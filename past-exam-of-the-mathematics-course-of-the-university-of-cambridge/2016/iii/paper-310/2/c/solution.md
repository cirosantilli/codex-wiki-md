<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because density is a [scalar field](../../../../../../scalar-field.md), $\widetilde\rho(\widetilde x)=\rho(x)$. Write both sides as background plus perturbation and expand the background time shift:

$$
\bar\rho(\tau)+\delta\rho(\tau,\mathbf x)
=\bar\rho(\tau+T)+\widetilde{\delta\rho}(\tau+T,\mathbf x+\nabla L)
=\bar\rho(\tau)+\bar\rho'T+\widetilde{\delta\rho}(\tau,\mathbf x).
$$

The coordinate shift acting on an already first-order perturbation contributes only at second order. Thus the [density perturbation gauge transformation](../../../../../../density-perturbation-gauge-transformation.md) is

$$
\boxed{\widetilde{\delta\rho}=\delta\rho-\bar\rho'T.}
$$

The [uniform-density curvature perturbation](../../../../../../uniform-density-curvature-perturbation.md) in the paper's sign convention is

$$
\zeta=-C+\frac13\nabla^2E+\mathcal H\frac{\delta\rho}{\bar\rho'}.
$$

The derivative on $\bar\rho'$ is essential and is present in the PDF; the TeX transcription drops it. The scalar-curvature combination transforms as

$$
-\widetilde C+\frac13\nabla^2\widetilde E
=-C+\frac13\nabla^2E+\mathcal HT,
$$

while the density term changes by $-\mathcal HT$. Hence **the two time-slicing changes cancel**:

$$
\boxed{\widetilde\zeta=\zeta.}
$$

On a uniform-density slice, $\delta\rho=0$ and this variable is the signed spatial-curvature perturbation. The construction assumes $\bar\rho'\ne0$; a pure constant-density cosmological constant does not define such a time slicing.

In [Newtonian gauge in cosmology](../../../../../../newtonian-gauge.md), $E=B=0$ and $C=-\Phi$. The background [cosmological perfect-fluid continuity equation](../../../../../../cosmological-perfect-fluid-continuity-equation.md) gives $\bar\rho'=-3\mathcal H(\bar\rho+\bar P)$, so, writing $D=\bar\rho+\bar P$,

$$
\zeta=\Phi-\frac{\delta\rho}{3D}.
$$

Set the [cosmological adiabatic sound speed](../../../../../../cosmological-adiabatic-sound-speed.md) $c_a^2=\bar P'/\bar\rho'$. Then $D'=-3\mathcal H D(1+c_a^2)$. Differentiate the previous expression and insert the perturbed energy-conservation equation:

$$
\begin{aligned}
\zeta'&=\Phi'-\frac{\delta\rho'}{3D}
+\frac{\delta\rho D'}{3D^2}\\
&=\frac{\mathcal H}{D}(\delta\rho+\delta P)
+\frac{\nabla\cdot\mathbf q}{3D}
-\frac{\mathcal H}{D}(1+c_a^2)\delta\rho.
\end{aligned}
$$

Consequently the **curvature evolution equation in this sign convention** is

$$
\boxed{\zeta'=\frac{\mathcal H}{\bar\rho+\bar P}\delta P_{\rm nad}
+\frac{\nabla\cdot\mathbf q}{3(\bar\rho+\bar P)}
=\frac{\mathcal H}{\bar\rho+\bar P}\delta P_{\rm nad}
+\frac13\nabla\cdot\mathbf v.}
$$

The last equality defines the total energy-frame velocity by $\mathbf q=D\mathbf v$. For [adiabatic cosmological perturbations](../../../../../../adiabatic-initial-conditions.md), the [non-adiabatic pressure perturbation](../../../../../../non-adiabatic-pressure-perturbation.md) vanishes. On [superhorizon scales](../../../../../../superhorizon-scale.md), the stated suppression of the velocity divergence makes the remaining gradient term negligible. Thus **$\zeta$ is conserved to leading order in $k/\mathcal H$**. The positive sign of the pressure source follows from the paper's definition of $\zeta$ and must not be replaced by a formula using the opposite curvature convention.

[Superhorizon conservation of uniform-density curvature](../../../../../../superhorizon-conservation-of-uniform-density-curvature.md) lets one carry a [primordial perturbation](../../../../../../primordial-perturbation.md) from its inflationary generation through otherwise complicated eras and predict the initial conditions for later [Cosmic microwave background anisotropy](../../../../../../cosmic-microwave-background-anisotropy-split.md) and structure growth. It relies on adiabaticity: an [isocurvature perturbation](../../../../../../cosmological-entropy-perturbation.md) can source curvature evolution, so the same conclusion is not automatic in an arbitrary multifield model.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
