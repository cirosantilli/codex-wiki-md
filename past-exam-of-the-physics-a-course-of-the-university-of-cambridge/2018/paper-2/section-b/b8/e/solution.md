<h1 id="section-b/b8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For mutually incoherent spectral components, the detected intensities add. If $S(\nu)$ describes the mean output spectral intensity, the [interferogram](../../../../../../interferogram.md) is

$$
I(x)=\int_0^\infty S(\nu)\,d\nu+\int_0^\infty S(\nu)\cos(2\pi\nu x/c)\,d\nu.
$$

Subtract the constant background, scan the mirror with a calibrated displacement, and take the [Fourier transform](../../../../../../fourier-transform-split.md) with respect to delay $\tau=x/c=2d/c$. This is [Fourier transform spectroscopy](../../../../../../fourier-transform-spectroscopy.md). The transform recovers the spectrum subject to detector response, finite scan length and any window function. Sampling the displacement finely enough to resolve the shortest optical fringes avoids aliasing.

Using the usual reciprocal-maximum-delay resolution estimate, $\delta\nu\simeq c/x_{\max}$, and $|\delta\nu|\simeq c\delta\lambda/\lambda^2$, gives

$$
x_{\max}\simeq\frac{\lambda^2}{\delta\lambda}=2.50\times10^{-2}\,\mathrm m,
\qquad
\boxed{d_{\max}=x_{\max}/2\simeq1.25\times10^{-2}\,\mathrm m=12.5\,\mathrm{mm}}.
$$

The mirror displacement is measured from zero [optical path difference](../../../../../../optical-path-difference.md). This [delay-range resolution in Fourier transform spectroscopy](../../../../../../delay-range-resolution-in-fourier-transform-spectroscopy.md) is a conventional estimate: a specified window and resolution definition introduce a numerical factor. For example, a symmetric rectangular delay window has its first instrumental zero at $\delta\nu=1/(2\tau_{\max})$, which would give $6.25\,\mathrm{mm}$ under that particular criterion. The paper does not specify a line-profile criterion; the standard $12.5\,\mathrm{mm}$ estimate states its convention explicitly.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
