<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A viscoelastic material stores part of the deformation [energy](../../../../../energy-split.md) and dissipates part of it. In [linear viscoelasticity](../../../../../linear-viscoelasticity.md), a small imposed shear [strain](../../../../../strain.md) produces a [stress](../../../../../stress.md) determined by its history, $\tau(t)=\int_{-\infty}^tG(t-t')\dot\gamma(t')\,dt'$. A shear step probes [stress relaxation](../../../../../stress-relaxation.md); a [stress](../../../../../stress.md) step probes [creep compliance](../../../../../creep-compliance.md). A purely elastic solid has persistent [stress](../../../../../stress.md) after a held [strain](../../../../../strain.md), while a [Newtonian fluid](../../../../../newtonian-fluid.md) relaxes that [stress](../../../../../stress.md) and creeps continuously under constant [stress](../../../../../stress.md).

For a [Maxwell model](../../../../../linear-maxwell-fluid.md), a [spring](../../../../../spring.md) of [shear modulus](../../../../../shear-modulus.md) $G_0$ and a [dashpot](../../../../../dashpot.md) of [viscosity](../../../../../dynamic-viscosity-split.md) $\eta$ are in series:

$$
\dot\gamma=\frac{\dot\tau}{G_0}+\frac\tau\eta,\qquad
G(t)=G_0e^{-t/\tau_M},\qquad \tau_M=\eta/G_0.
$$

For the convention $\gamma\propto e^{i\omega t}$,

$$
\boxed{G'=G_0\frac{(\omega\tau_M)^2}{1+(\omega\tau_M)^2},\qquad
G''=G_0\frac{\omega\tau_M}{1+(\omega\tau_M)^2}.}
$$

The [storage modulus](../../../../../storage-modulus.md) dominates at short times or high frequencies; the [loss modulus](../../../../../loss-modulus.md) dominates at long times or low frequencies. The [energy](../../../../../energy-split.md) dissipated per cycle per [volume](../../../../../volume.md) is $\pi G''\gamma_0^2$. A [Kelvin-Voigt model](../../../../../kelvin-voigt-model.md) places [spring](../../../../../spring.md) and [dashpot](../../../../../dashpot.md) in parallel and instead gives bounded creep $J(t)=(1-e^{-G_0t/\eta})/G_0$: a simple illustration of a viscoelastic solid. Real materials can require a spectrum of relaxation times rather than one element.

A small-amplitude oscillatory [rheometer](../../../../../rheometer.md) measures [stress](../../../../../stress.md) amplitude and phase relative to imposed [strain](../../../../../strain.md), giving $G'=|\tau_0/\gamma_0|\cos\delta$ and $G''=|\tau_0/\gamma_0|\sin\delta$. First sweep [strain](../../../../../strain.md) amplitude to identify the linear range; control [temperature](../../../../../temperature-split.md), sample ageing, [wall slip](../../../../../wall-slip.md) and instrument inertia. Frequency-dependent phase lag alone is insufficient if these apparatus effects are unresolved.

<a id="2/a/image-original-normalized-maxwell-relaxation-and-frequency-response"></a>
![](../../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2013/paper-1-viscoelastic-response.png)

**[Figure 1](#2/a/image-original-normalized-maxwell-relaxation-and-frequency-response). Original normalized Maxwell relaxation and frequency response**.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
