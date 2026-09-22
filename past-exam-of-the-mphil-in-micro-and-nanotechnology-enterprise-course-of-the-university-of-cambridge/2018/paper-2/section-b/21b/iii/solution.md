<h1 id="section-b/21b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [Kelvin-Voigt model](../../../../../../kelvin-voigt-model.md) element places a [spring](../../../../../../spring.md) and [dashpot](../../../../../../dashpot.md) in parallel, giving

$$
\sigma=G\gamma+\eta\dot\gamma.
$$

Under a [stress](../../../../../../stress.md) step from a relaxed state,

$$
\boxed{\gamma(t)=\frac{\sigma_0}{G}(1-e^{-t/\tau}),\qquad\tau=\eta/G,\quad t>0.}
$$

It captures delayed but bounded [material creep](../../../../../../creep-deformation.md) and eventual [strain](../../../../../../strain.md) recovery after unloading, rather than steady terminal flow.

For an ideal [strain](../../../../../../strain.md) step,

$$
\sigma(t)=G\gamma_0H(t)+\eta\gamma_0\delta(t).
$$

After the loading impulse, the [stress](../../../../../../stress.md) remains $G\gamma_0$. **The model does not produce a gradual stress-relaxation tail at held [strain](../../../../../../strain.md).** A real finite-rate ramp replaces the impulse by a finite [dashpot](../../../../../../dashpot.md) [stress](../../../../../../stress.md) during loading, but the subsequent held-strain [stress](../../../../../../stress.md) is still constant. Thus this model describes [material creep](../../../../../../creep-deformation.md) retardation but not a solid's genuine time-dependent relaxation toward another finite modulus.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [21B](../../21b.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
