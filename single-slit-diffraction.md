# Single-slit diffraction

↑ **Parent:** [Fraunhofer diffraction](fraunhofer-diffraction.md)

[Single-slit diffraction](single-slit-diffraction.md) is the spreading of [light](light.md) transmitted by one slit. Consider an ideal rectangular slit of width $a$, illuminated normally by a uniform [plane wave](plane-wave.md) with a single [wavelength](wavelength.md) $\lambda$ in the surrounding medium. This [monochromatic wave](monochromatic-wave.md) has uniform [wave amplitude](wave-amplitude.md) and equal incident [wave phases](phase-waves.md) across the slit, providing the required [optical coherence](optical-coherence.md). In the scalar [Fraunhofer diffraction](fraunhofer-diffraction.md) model, the normalized angular [wave intensity](intensity-physics.md) is

$$
\frac{I(\theta)}{I_0}=\left(\frac{\sin u}{u}\right)^2,\qquad u=\frac{\pi a\sin\theta}{\lambda},\qquad I_0=I(0),\qquad \lim_{u\to0}\frac{\sin u}{u}=1.
$$

Here $\theta$ is measured from the forward normal in the plane across the slit width. The [sinc function](sinc-function.md) uses the unnormalized convention $\operatorname{sinc}u=\sin u/u$. The [limit](limit-of-a-function.md) makes the central value one. This ideal envelope neglects additional direction-dependent propagation and detector factors; near the forward direction it describes the normalized screen [irradiance](irradiance.md). [Ling, Sanny and Moebs, University Physics Volume 3, §4.2: single-slit intensity](https://openstax.org/books/university-physics-volume-3/pages/4-2-intensity-in-single-slit-diffraction).

The noncentral zeros satisfy

$$
a\sin\theta_m=m\lambda,\qquad m\in\mathbb Z\setminus\{0\},\qquad \left|\frac{m\lambda}{a}\right|\leq1.
$$

The restriction follows from the range of the [sine](sine.md) of a real [angle](angle.md). The first minima have $\sin\theta=\pm\lambda/a$ when $\lambda/a\leq1$. If $a<\lambda$, this model has no noncentral zero in the forward hemisphere; equality puts the first zeros at grazing directions, outside the [small-angle approximation](small-angle-approximation.md) and off any finite perpendicular screen. [Ling, Sanny and Moebs, University Physics Volume 3, §4.1: positions of diffraction minima](https://openstax.org/books/university-physics-volume-3/pages/4-1-single-slit-diffraction).

For $0<\lambda/a<1$, define the central width as the separation between the two first minima. Its angular width and its width on a perpendicular screen are

$$
\Delta\theta=2\arcsin(\lambda/a)\approx\frac{2\lambda}{a},\qquad y=L\tan\theta,\qquad W=2L\tan\!\bigl(\arcsin(\lambda/a)\bigr)\approx\frac{2L\lambda}{a}.
$$

The angular approximation uses [radians](radian.md) and requires $\lambda/a\ll1$; the screen approximation uses $y\approx L\theta$. The [tangent](tangent.md) relation is exact straight-line geometry, even though the underlying [Fraunhofer diffraction](fraunhofer-diffraction.md) field is approximate. This width is distinct from the [full width at half maximum](full-width-at-half-maximum.md).

For $\lambda=500\,\mathrm{nm}$, $a=0.1\,\mathrm{mm}$ and $L=1\,\mathrm m$, the positive first minimum is

$$
\theta_1=\arcsin(0.005)\approx0.286480^\circ,\qquad y_1=\frac{L(0.005)}{\sqrt{1-0.005^2}}\approx5.00006\,\mathrm{mm},\qquad W\approx10.0001\,\mathrm{mm}.
$$

The dimensionless far-field parameter is $a^2/(\lambda L)=0.02$. Doubling the slit width to $a=0.2\,\mathrm{mm}$ gives $W\approx5.00002\,\mathrm{mm}$ and parameter $0.08$; both curves below use the [Fraunhofer diffraction](fraunhofer-diffraction.md) approximation. Choosing $L=2\,\mathrm m$ halves those parameters and doubles both screen widths.

<a id="image-normalized-single-slit-diffraction-on-a-screen-a-narrower-slit-produces-a-wider-central-maximum"></a>
![](single-slit-diffraction-width.png)

**[Figure 11](#image-normalized-single-slit-diffraction-on-a-screen-a-narrower-slit-produces-a-wider-central-maximum). Normalized single-slit diffraction on a screen: a narrower slit produces a wider central maximum**.

Each curve is normalized to its own $I_0$; the arrows measure between first minima. The calculation uses $\theta=\arctan(y/L)$ before evaluating the [sinc function](sinc-function.md), rather than replacing $\sin\theta$ by $y/L$. The lower diagram shows the exact screen geometry with the vertical scale enlarged. Normalization removes the change in peak brightness when the slit width changes.

The [wave interference](interference-wave-propagation.md) explanation is especially simple: divide the slit into equal narrow strips and add their [complex amplitudes](complex-amplitude.md), rather than their [wave intensities](intensity-physics.md). With [wavenumber](wavenumber.md) $k=2\pi/\lambda$, the continuous slit gives

$$
\frac{A(\theta)}{A(0)}=\frac1a\int_{-a/2}^{a/2}e^{ikx\sin\theta}\,dx=\frac{e^{iu}-e^{-iu}}{2iu}=\frac{\sin u}{u}.
$$

Integrating the [complex exponential](complex-exponential-function.md) gives the endpoint difference; its continuous value at zero is one. Taking the squared [complex modulus](complex-modulus.md) gives the stated [wave intensity](intensity-physics.md). This is the [Fourier transform of an interval indicator](fourier-transform-of-an-interval-indicator.md) expressed in angular coordinates. Feynman's continuous-source argument obtains the same pattern by letting the number of sources tend to infinity. [Feynman, Leighton and Sands, I §30–2: continuous distributions of oscillators](https://www.feynmanlectures.caltech.edu/I_30.html#Ch30-S2).

At the positive first minimum, the [wave phases](phase-waves.md) span exactly $2\pi$ across the slit. Every strip in one half has a partner $a/2$ away, with equal [wave amplitude](wave-amplitude.md) and [phase difference](phase-difference.md) $\pi$, so the pairs cancel. At $\theta=0$, all the [wave phases](phase-waves.md) align instead. [Ling, Sanny and Moebs, §4.1: cancellation between the slit halves](https://openstax.org/books/university-physics-volume-3/pages/4-1-single-slit-diffraction).

<a id="image-complex-amplitudes-across-a-slit-aligned-contributions-at-broadside-and-cancellation-at-the-first-minimum"></a>
![](single-slit-aperture-phase-cancellation.png)

**[Figure 12](#image-complex-amplitudes-across-a-slit-aligned-contributions-at-broadside-and-cancellation-at-the-first-minimum). Complex amplitudes across a slit: aligned contributions at broadside and cancellation at the first minimum**.

The drawing uses $N=8$ equally weighted midpoint samples $x_j/a=-1/2+(j+1/2)/8$, with $j=0,\ldots,7$. At the first minimum their [complex amplitudes](complex-amplitude.md) are a common rotation of the eight [roots of unity](root-of-unity.md), so their head-to-tail polygon closes exactly. This finite sum illustrates cancellation; the continuous [integral](integral-split.md), rather than eight point sources, defines the slit pattern at general [angles](angle.md). The circle shows the continuous range of [wave phases](phase-waves.md); coloured arrows show the eight samples.

A narrower [aperture](aperture.md) requires a larger [angle](angle.md) to accumulate the cancelling [phase difference](phase-difference.md), so narrowing the slit widens the beam. This is a useful limit on [geometrical optics](geometrical-optics-split.md): confining [light](light.md) more tightly at an opening increases its subsequent angular spread. At fixed incident [irradiance](irradiance.md) and slit height, reducing $a$ also reduces transmitted [power](power.md), exposing a practical balance between [diffraction-limited resolution](diffraction-limited-resolution.md) and light throughput. In a [diffraction grating](diffraction-grating.md), this [single-slit diffraction](single-slit-diffraction.md) envelope modulates the [wave interference](interference-wave-propagation.md) between different slits.

**Table of contents**

- [Polychromatic single-slit diffraction](polychromatic-single-slit-diffraction.md)
- [Demagnifying a distant diffraction pattern](demagnifying-a-distant-diffraction-pattern.md)

## ↑ Ancestors (6)

1. [Fraunhofer diffraction](fraunhofer-diffraction.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Diffraction grating](diffraction-grating.md)
- [Diffraction order](diffraction-order.md)
- [Fixed-illumination grating peak change with slit width](fixed-illumination-grating-peak-change-with-slit-width.md)
- [Four-slit Fraunhofer diffraction](four-slit-fraunhofer-diffraction.md)
- [Fraunhofer diffraction](fraunhofer-diffraction.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1/section-b/b8/solution.md)
- [Why the given slit width removes the chosen order](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-b/b8/why-the-given-slit-width-removes-the-chosen-order.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-b/b7/e/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-b/b8/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2/section-b/b7/c/ii/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2/section-b/b7/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-a/4/solution.md)
- [Single-slit diffraction](single-slit-diffraction.md)
- [Spatial optical coherence](spatial-optical-coherence.md)
