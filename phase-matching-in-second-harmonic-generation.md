# Phase matching in second-harmonic generation

↑ **Parent:** [Second-harmonic generation](second-harmonic-generation.md)

[Phase matching](phase-matching.md) makes [wave amplitudes](wave-amplitude.md) emitted at different depths add coherently. Consider collinear [plane waves](plane-wave.md) in a uniform transparent material of length $L$, with fixed [polarization of waves](polarization-waves.md) and nonzero selected [nonlinear optical susceptibility](nonlinear-optical-susceptibility.md). Assume negligible pump depletion, negligible [absorption](absorption-electromagnetic-radiation.md), an initially absent harmonic, and a wide beam for which [diffraction](diffraction.md) is negligible. The pump's [wave amplitude](wave-amplitude.md) is then constant throughout the interaction.

The pump [electric field](electric-field-split.md) has spatial [wave phase](phase-waves.md) $k_\omega z$; its quadratic source has spatial [wave phase](phase-waves.md) $2k_\omega z$. The freely propagating harmonic has [wave number](wavenumber.md) $k_{2\omega}$. Define the [second-harmonic phase mismatch](second-harmonic-phase-mismatch.md) by

$$
\Delta k=k_{2\omega}-2k_\omega,
\qquad k_\omega=\frac{n_\omega\omega}{c},\qquad
k_{2\omega}=\frac{2n_{2\omega}\omega}{c}.
$$

For the chosen complex-field convention, the outgoing harmonic [wave amplitude](wave-amplitude.md), up to an overall constant and propagation phase, is proportional to

$$
\mathcal A(L)=\int_0^L e^{i\Delta k z}\,dz
=L e^{i\Delta kL/2}\operatorname{sinc}\!\left(\frac{\Delta kL}{2}\right),
\qquad \operatorname{sinc}x=\begin{cases}\sin x/x,&x\ne0,\\1,&x=0.\end{cases}
$$

Choosing the conjugate complex-field convention reverses the exponent's sign without changing the [wave intensity](intensity-physics.md). Taking the squared [complex modulus](complex-modulus.md) gives

$$
I_{2\omega}(L)=C I_\omega^2 L^2\operatorname{sinc}^2\!\left(\frac{\Delta kL}{2}\right),\qquad C>0.
$$

Here $C$ is fixed for the chosen modes and material; its dimensions accommodate the stated [wave intensity](intensity-physics.md) convention. The quadratic pump dependence follows because the source [wave amplitude](wave-amplitude.md) is proportional to $E_0^2$, whereas $I_\omega$ is proportional to $E_0^2$. The [sinc function](sinc-function.md) comes from summing contributions along the whole material, just as a finite aperture produces [diffraction](diffraction.md) through addition of [complex amplitudes](complex-amplitude.md).

At $\Delta k=0$, the [integral](integral-split.md) is $L$ and the harmonic [wave intensity](intensity-physics.md) grows as $L^2$. At $\Delta kL=2\pi$, all those contributions cancel. This cancellation needs no [absorption](absorption-electromagnetic-radiation.md): their [wave phases](phase-waves.md) wind through a full turn. At high conversion, the constant-pump assumption fails, so the $L^2$ law cannot continue indefinitely. Tight focusing, finite [optical pulses](optical-pulse.md), [absorption](absorption-electromagnetic-radiation.md), and transverse separation of modes also require a more complete model.

[Optical dispersion](dispersion-optics.md) generally makes $n_{2\omega}\ne n_\omega$. In a suitable [crystal](crystal.md), [birefringence](birefringence.md) allows modes with different [polarization of waves](polarization-waves.md) to experience different [refractive indices](refractive-index.md), making their selected values equal. The appropriate crystal direction and allowed [nonlinear optical susceptibility](nonlinear-optical-susceptibility.md) component must both work.[p. 19: momentum mismatch and birefringence compensation](nonlinear-optics-and-spectroscopy-by-nicolaas-bloembergen.md)

<a id="image-calculated-second-harmonic-generation-versus-second-harmonic-phase-mismatch-and-interaction-length"></a>
![](second-harmonic-phase-matching-sinc-squared.png)

**[Figure 24](#image-calculated-second-harmonic-generation-versus-second-harmonic-phase-mismatch-and-interaction-length). Calculated second-harmonic generation versus second-harmonic phase mismatch and interaction length**. [Source](second-harmonic-phase-matching-sinc-squared.py). Original uniform-medium, undepleted [plane wave](plane-wave.md) model with chosen $L_0=1\,\mathrm{mm}$. Both curves use the same pump and prefactor: $I_{2\omega}/(CI_\omega^2L_0^2)=(L/L_0)^2\operatorname{sinc}^2(\Delta kL/2)$. Doubling $L$ raises the matched peak fourfold and halves the mismatch to the first zero. The dimensionless horizontal coordinate is $\Delta kL_0/(2\pi)$; no curve is a fit to historical data.

For a worked calculation, choose $L_0=1\,\mathrm{mm}$ and $\Delta k=\pi\,\mathrm{mm^{-1}}$. At $L=L_0$, the harmonic [wave intensity](intensity-physics.md) is $4/\pi^2\simeq0.4053$ of its perfectly matched value. At $L=2L_0$ it vanishes in this model. More material can therefore reduce the output. If instead $\Delta k=0$, doubling $L$ multiplies output by four. The two curves retain that common normalization, so their different peak heights are meaningful.

**Table of contents**

- [Second-harmonic phase mismatch](second-harmonic-phase-mismatch.md)
- [Second-harmonic coherence length](second-harmonic-coherence-length.md)

## ↑ Ancestors (6)

1. [Second-harmonic generation](second-harmonic-generation.md)
2. [Nonlinear optics](nonlinear-optics.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
