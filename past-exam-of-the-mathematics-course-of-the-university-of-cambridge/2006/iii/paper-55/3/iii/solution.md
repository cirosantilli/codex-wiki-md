<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $A=\bar\rho+\bar P$, and assume $A\ne0$ so that the density-defined curvature is meaningful. Under the [cosmological gauge transformation](../../../../../../gauge-transformation-in-cosmological-perturbation-theory.md) in part ii,

$$
\widetilde\Psi=\Psi+\bar NH T,\qquad
\delta\widetilde\rho=\delta\rho+3\bar NH A T.
$$

Therefore the two time-shift terms cancel:

$$
\boxed{\widetilde\zeta=\widetilde\Psi-\frac{\delta\widetilde\rho}{3A}
=\Psi-\frac{\delta\rho}{3A}=\zeta.}
$$

This is the [uniform-density curvature perturbation](../../../../../../uniform-density-curvature-perturbation.md) with the paper's overall sign. On a uniform-density slice it is the spatial curvature potential $\Psi$. Its opposite overall sign is also a common convention, so the sign must be kept consistent rather than imported from another metric convention.

To establish time conservation, write $D_t=\bar N^{-1}\partial_t$ and $c_a^2=\dot{\bar P}/\dot{\bar\rho}$. Background [stress-energy conservation](../../../../../../stress-energy-conservation.md) implies

$$
D_tA=-3H(1+c_a^2)A.
$$

For constant $w$ in the given barotropic [equation of state](../../../../../../equation-of-state.md), $c_a^2=w$. Differentiate $\zeta=\Psi-\delta\rho/(3A)$:

$$
D_t\zeta=D_t\Psi-\frac{D_t\delta\rho}{3A}
+\frac{\delta\rho}{3A^2}D_tA.
$$

Insert both perturbed evolution equations from the hint, keeping the spatial Laplacian $\Delta=\nabla^2/a^2$:

$$
\begin{aligned}
D_t\zeta
&=-H\Phi+\frac\kappa3+\frac{\Delta\chi}{3}
+\frac{H(\delta\rho+\delta P)}A-\frac\kappa3+H\Phi
+\frac{\Delta u}{3A}-\frac{H(1+c_a^2)\delta\rho}A\\
&=\frac{H}{A}(\delta P-c_a^2\delta\rho)
+\frac13\Delta\left(\chi+\frac uA\right).
\end{aligned}
$$

Thus the lapse perturbation $\Phi$ and the trace perturbation $\kappa$ cancel exactly. The remaining pressure term is the [non-adiabatic pressure perturbation](../../../../../../non-adiabatic-pressure-perturbation.md) $\delta P_{\rm nad}=\delta P-c_a^2\delta\rho$. In the assumed barotropic fluid, the perturbed [equation of state](../../../../../../equation-of-state.md) gives $\delta P=w\delta\rho$ and $c_a^2=w$, so it vanishes. For a [Fourier mode](../../../../../../fourier-mode.md),

$$
\boxed{\frac{\dot\zeta}{\bar N}=-\frac{k^2}{3a^2}\left(\chi+\frac uA\right).}
$$

For regular long-wavelength perturbations, the velocity and shear potentials in this combination do not grow as $k^{-2}$, so the right-hand side is gradient-suppressed when $k\ll aH$. Therefore **$\zeta$ is conserved to leading superhorizon order**, which is the [superhorizon conservation of uniform-density curvature](../../../../../../superhorizon-conservation-of-uniform-density-curvature.md) requested.

The statement is not exact for arbitrary finite $k$: the displayed gradient term gives its correction. It also requires [adiabatic cosmological perturbations](../../../../../../adiabatic-initial-conditions.md); entropy perturbations in a multicomponent system or a nonbarotropic fluid can give $\delta P_{\rm nad}\ne0$ and evolve $\zeta$ even at zero gradient order. At exact $w=-1$, $A=0$ and the question's variable is undefined, rather than a well-defined conserved density-slicing perturbation.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
