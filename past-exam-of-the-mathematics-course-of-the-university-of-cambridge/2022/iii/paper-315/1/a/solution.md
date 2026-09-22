<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the plane-parallel [radiative transfer equation](../../../../../../radiative-transfer-equation.md)

$$
\mu\frac{dI_\nu}{d\tau_\nu}=I_\nu-S_\nu,
$$

angular integration gives the zeroth [radiation-field moment](../../../../../../radiation-field-moment.md) equation

$$
\frac{dH_\nu}{d\tau_\nu}=J_\nu-S_\nu.
$$

The net radiative heating per unit volume is therefore

$$
4\pi\int_0^\infty\alpha_\nu(J_\nu-S_\nu)\,d\nu.
$$

[Radiative equilibrium](../../../../../../radiative-equilibrium.md) requires it to vanish, equivalently that the frequency-integrated [radiative flux](../../../../../../radiative-flux.md) be independent of depth:

$$
\boxed{\int_0^\infty\alpha_\nu(J_\nu-S_\nu)\,d\nu=0}.
$$

In [local thermodynamic equilibrium](../../../../../../local-thermodynamic-equilibrium.md) with [coherent isotropic scattering](../../../../../../coherent-isotropic-scattering.md),

$$
S_\nu=(1-\omega_\nu)B_\nu(T)+\omega_\nu J_\nu,
$$

where $\omega_\nu$ is the [single-scattering albedo](../../../../../../single-scattering-albedo.md). Since $\alpha_\nu(1-\omega_\nu)=\alpha_{\nu,\rm abs}$, the condition becomes

$$
\boxed{\int_0^\infty\alpha_{\nu,\rm abs}
[J_\nu-B_\nu(T)]\,d\nu=0}.
$$

Conservative scattering redistributes directions but contributes no net material heating.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
