<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a plane-parallel atmosphere with optical depth increasing downward, the [radiative transfer equation](../../../../../../radiative-transfer-equation.md) is

$$
\mu\frac{dI_\nu}{d\tau_\nu}=I_\nu-S_\nu.
$$

Integrating over solid angle gives the first [radiation-field moment](../../../../../../radiation-field-moment.md)

$$
\frac{dF_\nu}{d\tau_\nu}=4\pi(J_\nu-S_\nu).
$$

In [radiative equilibrium](../../../../../../radiative-equilibrium.md), matter has no net local radiative heating, so the opacity-weighted frequency integral of $J_\nu-S_\nu$ vanishes. After converting each optical-depth derivative to physical depth and integrating over frequency,

$$
\boxed{\frac{dF}{dz}=0}.
$$

Thus the bolometric internal flux is constant with depth, as stated by [constant flux in a plane-parallel radiative-equilibrium atmosphere](../../../../../../constant-flux-in-a-plane-parallel-radiative-equilibrium-atmosphere.md).

In local thermal equilibrium $S_\nu=B_\nu(T)$. Define the planet's [internal effective temperature of a planet](../../../../../../internal-effective-temperature-of-a-planet.md) by the constant outward flux. The standard [Planck law](../../../../../../planck-s-law.md) integral gives

$$
\boxed{F_{\rm int}=\pi\int_0^\infty B_\nu(T_{\rm eff})\,d\nu
=\sigma T_{\rm eff}^4}.
$$

The corresponding intrinsic luminosity is $L_{\rm int}=4\pi R_p^2\sigma T_{\rm eff}^4$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
