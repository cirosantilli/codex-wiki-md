<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

With the convention in the question, the constant [velocity-anisotropy parameter](../../../../../velocity-anisotropy-parameter.md) is $\beta=1-\sigma_t^2/\sigma_r^2$. Since $V_c^2=r\,d\Phi/dr$, the [Spherical Jeans equation](../../../../../spherical-jeans-equation.md) becomes

$$
\frac{d(\nu\sigma_r^2)}{dr}
+\frac{2\beta}{r}\nu\sigma_r^2
=-\frac{\nu V_c^2}{r}.
$$

For $\nu=\nu_0r^{-\alpha}$ and $V_c^2=V_0^2r^{2\gamma}$, its general [integrating factor](../../../../../integrating-factor.md) solution is

$$
\boxed{\sigma_r^2(r)=
\frac{V_c^2(r)}{\alpha-2\beta-2\gamma}
+Cr^{\alpha-2\beta}.}
$$

The homogeneous term represents a boundary pressure. For an extended scale-free system the physical boundary condition normally removes it, leaving

$$
\boxed{\sigma_r^2=\frac{V_c^2}{\alpha-2\beta-2\gamma}.}
$$

Positivity requires $\alpha-2\beta-2\gamma>0$. A complete physical model must also have a nonnegative [galactic distribution function](../../../../../galactic-distribution-function.md) and sensible inner and outer boundary behaviour; for example, strong radial anisotropy is restricted by density-slope--anisotropy inequalities.

Observationally, the tracer density can be estimated from star counts only after correcting distances, extinction, survey selection, and incompleteness. Spectroscopy supplies mainly line-of-sight velocities; proper motions add transverse information but become less precise for distant halo stars. The equation shows the [mass--anisotropy--density degeneracy](../../../../../mass-anisotropy-density-degeneracy.md) directly: the same measured $\sigma_r$ can result from a larger $V_c$, a steeper tracer slope $\alpha$, or a different $\beta$. Even globally constant power laws therefore do not determine the galactic mass profile unless some of these quantities are independently constrained.

If $\alpha$, $\beta$, or $\gamma$ changes near a break radius, the solution at one radius also depends on the outer boundary integral. A break in observed dispersion may be attributed to a mass-profile feature, a tracer-density break, or a change in orbital anisotropy. Separate tracer populations, full three-dimensional velocities, higher velocity moments, and measurements over a wide radial range help break this degeneracy.

More flexible alternatives model a nonnegative solution of the [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) itself. An [action-based galactic distribution function](../../../../../action-based-galactic-distribution-function.md) gives an analytic or parametrized $f(\mathbf J)$; a [Schwarzschild orbit-superposition model](../../../../../schwarzschild-orbit-superposition-model.md) assigns nonnegative weights to an orbit library; and a [made-to-measure stellar-dynamical model](../../../../../made-to-measure-stellar-dynamical-model.md) adjusts particle weights to reproduce observations. These methods retain more phase-space information than Jeans moments, although their flexibility introduces model choices and regularization.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
