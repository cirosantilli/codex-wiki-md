<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

For uniform illumination, the aperture is $h(x)=1$ for $|x|<a/2$ and zero otherwise. With $q=2\pi\sin\theta/\lambda$,

$$
\widetilde h(q)=\int_{-a/2}^{a/2}e^{-iqx}\,dx
=a\frac{\sin(qa/2)}{qa/2},\qquad
\boxed{I(\theta)=I(0)\left(\frac{\sin\alpha}{\alpha}\right)^2,\quad
\alpha=\frac{\pi a\sin\theta}{\lambda}}.
$$

Zeros occur at $\sin\theta=j\lambda/a$, $j\ne0$; the central maximum extends between $\pm\lambda/a$. A monochromatic [laser](../../../../../laser-split.md) expanded into a collimated beam can illuminate the slit. A [lens](../../../../../lens-optics.md) with the screen in its back [focal plane](../../../../../focal-plane.md) produces the Fraunhofer pattern; alternatively use a sufficiently distant screen, $z\gg a^2/\lambda$. Align the slit and beam and avoid detector saturation.

For $N$ equally spaced slits, write the aperture as a [convolution](../../../../../convolution.md)

$$
h_N=\operatorname{rect}_a*\sum_{j=0}^{N-1}\delta(x-jb).
$$

The [convolution theorem](../../../../../convolution-theorem.md) converts this into a single-slit transform times the finite-array transform. Therefore

$$
\boxed{I_N(q)\propto a^2\operatorname{sinc}^2\left(\frac{qa}{2}\right)
\left[\frac{\sin(Nqb/2)}{\sin(qb/2)}\right]^2},
\qquad \operatorname{sinc}u=\frac{\sin u}{u}.
$$

Principal maxima are at $b\sin\theta=m\lambda$ for [normal incidence](../../../../../normal-incidence.md), inside the single-slit envelope. Their height scales as $N^2$ times the envelope, and their first zeros are separated from a peak by $\delta(\sin\theta)=\lambda/(Nb)$.

The envelope-to-order-spacing ratio is $b/a$: increasing it admits more orders within the central envelope and changes the relative order strengths. In particular, an order is missing when $ma/b$ is a nonzero integer. Statements about absolute angular spacing need a fixed dimension: at fixed $a$, increasing $b$ reduces order spacing; at fixed $b$, decreasing $a$ broadens the envelope.

For fixed incident angle, differentiating the [grating equation](../../../../../grating-equation.md) gives an order displacement $\delta(\sin\theta)=|m|\delta\lambda/b$. Equating this to the peak-to-first-zero width gives

$$
\boxed{\delta\lambda=\frac{\lambda}{|m|N}\simeq\frac{\lambda b}{|m|W}}.
$$

Here $W\simeq Nb$ is the illuminated grating width; this is the ideal Rayleigh limit, before slit width or aberrations broaden the spectral image.

With $b=(1600\ \mathrm{mm^{-1}})^{-1}=0.000625\ \mathrm{mm}$, the required count is $N\ge372.7/(2\times0.2)=931.75$. Thus **932 illuminated slits**, or **$W_{\min}\simeq0.5825\ \mathrm{mm}$**, suffice ideally. Checking [diffraction-order feasibility](../../../../../diffraction-order-feasibility.md), [normal incidence](../../../../../normal-incidence.md) cannot produce this second order because $2\lambda/b=1.193>1$; an oblique [spectrograph](../../../../../spectrograph.md) geometry is required. A feasible reflection-Littrow example has $\sin\theta=m\lambda/(2b)=0.5963$, or $\theta\simeq36.6^\circ$.

<a id="section-b/b8/image-original-slit-finite-array-convolution-diffraction-pattern-and-fourier-plane-experimental-layout"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-2-grating-fourier.png)

**[Figure 2](#section-b/b8/image-original-slit-finite-array-convolution-diffraction-pattern-and-fourier-plane-experimental-layout). Original slit, finite-array convolution, diffraction pattern and Fourier-plane experimental layout**.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
