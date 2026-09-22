<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume [local thermodynamic equilibrium](../../../../../../local-thermodynamic-equilibrium.md), negligible scattering of thermal radiation, and a plane-parallel atmosphere. With inward [optical depth](../../../../../../optical-depth.md) $\tau_\lambda$ and outward ray cosine $\mu$, the [radiative transfer equation](../../../../../../radiative-transfer-equation.md) is

$$
\mu\frac{dI_\lambda}{d\tau_\lambda}=I_\lambda-B_\lambda[T(\tau_\lambda)].
$$

For a deep atmosphere, its [formal solution of the radiative transfer equation](../../../../../../formal-solution-of-the-radiative-transfer-equation.md) is

$$
I_\lambda(0,\mu)=\int_0^\infty B_\lambda[T(t)]e^{-t/\mu}\frac{dt}{\mu}.
$$

The weighting samples $\tau_\lambda$ of order unity. The [Eddington-Barbier relation](../../../../../../eddington-barbier-relation.md) makes this precise when the source function is nearly linear: $I_\lambda(0,\mu)\simeq B_\lambda[T(\tau_\lambda=\mu)]$.

A molecular band with greater [opacity](../../../../../../opacity.md) reaches unit [optical depth](../../../../../../optical-depth.md) higher than the nearby continuum. If [temperature](../../../../../../temperature.md) decreases upward, that band samples cooler gas and appears in absorption. If an [atmospheric thermal inversion](../../../../../../inversion-meteorology.md) makes the upper gas hotter, the band appears in emission. If both depths have the same [temperature](../../../../../../temperature.md), an opaque isothermal atmosphere has

$$
\boxed{I_\lambda=B_\lambda(T),}
$$

and no opacity-dependent features. This last conclusion assumes all wavelengths are opaque or the lower boundary emits the same [Planck function](../../../../../../planck-function.md); an optically thin isothermal layer over a different background need not be featureless.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
