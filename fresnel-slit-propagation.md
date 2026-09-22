# Fresnel slit propagation

↑ **Parent:** [Fresnel diffraction](fresnel-diffraction.md)

Consider a uniform [plane wave](plane-wave.md) of unit [complex amplitude](complex-amplitude.md) transmitted by an ideal [optical slit](optical-slit.md) of full width $D$. Treat the field as invariant along the [optical slit](optical-slit.md) height: this is [one-dimensional transverse Fresnel propagation](one-dimensional-transverse-fresnel-propagation.md), so the prefactor is $1/\sqrt{i\lambda z}$, rather than the two-dimensional prefactor $1/(i\lambda z)$. Removing the carrier $e^{ikz}$ gives

$$
u(x,z)=\frac{e^{-i\pi/4}}{\sqrt{\lambda z}}\int_{-D/2}^{D/2}\exp\!\left[\frac{i\pi(x-\xi)^2}{\lambda z}\right]d\xi,\qquad\frac{I(x,z)}{I_{\rm inc}}=|u(x,z)|^2.
$$

Here $I_{\rm inc}$ is incident [irradiance](irradiance.md). This infinitely long slit model describes a transverse cut away from the ends of a sufficiently long physical slit; its finite conserved quantity is transmitted [power](power.md) per unit [optical slit](optical-slit.md) height.

Put $t=\xi/D$ and $q=xD/(\lambda z)$. Substitution reduces the [integral](integral-split.md) to

$$
A(q,N_D)=\int_{-1/2}^{1/2}e^{i\pi N_Dt^2-2\pi iqt}dt,\qquad\frac{I(x,z)}{I_{\rm inc}}=N_D|A(q,N_D)|^2.
$$

This form separates the pattern's shape from its physical scale. Reflection $t\mapsto-t$ proves $A(-q,N_D)=A(q,N_D)$, so the [light intensity](light-intensity.md) is an [even function](even-function.md) of $x$. At $N_D=0$, direct integration gives $A(q,0)=\sin(\pi q)/(\pi q)$, with [limit](limit-of-a-function.md) one at $q=0$. Hence the [Fraunhofer diffraction](fraunhofer-diffraction.md) comparison is the squared [sinc function](sinc-function.md). In this paragraph the unnormalized [sinc function](sinc-function.md) takes argument $\pi q$.

For an original example, choose [wavelength](wavelength.md) $\lambda=633\,\mathrm{nm}$ and full width $D=0.400\,\mathrm{mm}$. At $z=0.0200\,\mathrm m$, $N_D\simeq12.6382$, $N_a\simeq3.15956$ and the edge-to-centre [wave phase](phase-waves.md) change is $9.92604$ [radians](radian.md). At $z=2.00\,\mathrm m$, $N_D\simeq0.126382$, $N_a\simeq0.0315956$ and that [wave phase](phase-waves.md) change is only $0.0992604$ [radians](radian.md). Even the nearer screen is fifty slit widths away; that geometric comparison alone misses its strong [Fresnel diffraction](fresnel-diffraction.md).

<a id="image-original-calculated-fresnel-diffraction-profiles-of-a-0-400-mm-slit-at-633-nm-compared-with-the-fraunhofer-diffraction-shape"></a>
![](fresnel-slit-near-far-profiles.png)

**[Figure 2](#image-original-calculated-fresnel-diffraction-profiles-of-a-0-400-mm-slit-at-633-nm-compared-with-the-fraunhofer-diffraction-shape). Original calculated Fresnel diffraction profiles of a 0.400 mm slit at 633 nm, compared with the Fraunhofer diffraction shape**.

These are numerical predictions from the displayed scalar [integral](integral-split.md), using the [composite trapezoidal rule](composite-trapezoidal-rule.md), rather than measured profiles. Each curve is divided by its own peak [light intensity](light-intensity.md); the two horizontal scales differ. At 2 cm the computed central [irradiance](irradiance.md) is about $1.14812I_{\rm inc}$, with brighter off-axis maxima. At 2 m it is about $0.126272I_{\rm inc}$ and is the peak. The dashed [Fraunhofer diffraction](fraunhofer-diffraction.md) curve has its own central normalization; its first zeros are at $x=\pm\lambda z/D=\pm3.165\,\mathrm{mm}$. The finite-distance [Fresnel diffraction](fresnel-diffraction.md) curve remains slightly nonzero there.

Normalization hides the brightness change, but not the change in shape. The [Fourier transform](fourier-transform-split.md) propagation multiplier has unit [complex modulus](complex-modulus.md), so [Plancherel theorem](plancherel-theorem.md) gives

$$
\int_{\mathbb R}\frac{I(x,z)}{I_{\rm inc}}dx=\int_{-D/2}^{D/2}1\,d\xi=D.
$$

This is conservation of transmitted [power](power.md) per unit height in the ideal scalar model. An [integral](integral-split.md) over only the displayed screen [interval](interval-mathematics.md) misses the tails; a peak-normalized profile is not a unit-[integral](integral-split.md) [probability density](probability-density.md). Spreading and decreasing brightness together preserve the transmitted [power](power.md).

## ↑ Ancestors (6)

1. [Fresnel diffraction](fresnel-diffraction.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Fresnel number](fresnel-number.md)
- [Near-field diffraction laboratory experiment](near-field-diffraction-laboratory-experiment.md)
