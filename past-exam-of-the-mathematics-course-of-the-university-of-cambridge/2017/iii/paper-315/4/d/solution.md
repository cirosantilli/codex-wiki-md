<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let an isothermal non-scattering atmospheric layer of [temperature](../../../../../../temperature.md) $T_a$ lie above an optically thick continuum source with [brightness temperature](../../../../../../brightness-temperature.md) $T_b$. Assume [local thermodynamic equilibrium](../../../../../../local-thermodynamic-equilibrium.md), so the layer emits with [Planck function](../../../../../../planck-function.md) $B_\lambda(T_a)$. Its vertical [optical depth](../../../../../../optical-depth.md) is $\tau_\lambda$; a ray with direction cosine $\mu$ has slant depth $t_\lambda=\tau_\lambda/\mu$.

The [formal solution of the radiative transfer equation](../../../../../../formal-solution-of-the-radiative-transfer-equation.md) gives

$$
\boxed{I_\lambda=B_\lambda(T_b)e^{-t_\lambda}
+B_\lambda(T_a)(1-e^{-t_\lambda}).}
$$

The two terms are attenuated background and layer emission. Compare a line and nearby continuum at the same wavelength to adequate approximation, with $t_{\rm line}>t_{\rm cont}$. The [one-layer spectral contrast](../../../../../../one-layer-spectral-contrast.md) is

$$
I_{\rm line}-I_{\rm cont}
=[B_\lambda(T_a)-B_\lambda(T_b)]
[e^{-t_{\rm cont}}-e^{-t_{\rm line}}].
$$

The second bracket is positive, and $B_\lambda(T)$ increases with [temperature](../../../../../../temperature.md). Therefore a cooler upper layer produces absorption, a hotter upper layer produces emission, and an isothermal source-plus-layer produces no line contrast:

$$
\boxed{T_a<T_b:\ \text{absorption};\quad
T_a>T_b:\ \text{emission};\quad T_a=T_b:\ \text{no contrast}.}
$$

This is why higher [opacity](../../../../../../opacity.md) sampling a cooler altitude creates absorption in an outward-cooling atmosphere, whereas an [atmospheric thermal inversion](../../../../../../inversion-meteorology.md) can create emission. If both line and continuum are very optically thick in the same layer, their contrast tends to vanish even with a different deeper [temperature](../../../../../../temperature.md). Scattering, non-LTE excitation, and nonuniform layers require a more general [radiative transfer](../../../../../../radiative-transfer.md) treatment.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
