<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [convolution](../../../../../../convolution.md) of two [aperture](../../../../../../aperture.md) functions in one dimension is

$$
(f*g)(x)=\int_{-\infty}^{\infty}f(u)g(x-u)\,du.
$$

With [Fourier transform](../../../../../../fourier-transform-split.md) convention $\widehat f(q)=\int f(x)e^{-iqx}dx$, the [convolution theorem](../../../../../../convolution-theorem.md) states

$$
\boxed{\widehat{f*g}(q)=\widehat f(q)\widehat g(q)},\qquad
\boxed{\widehat{fg}(q)=\frac1{2\pi}(\widehat f*\widehat g)(q)}.
$$

The first identity follows by substituting the convolution integral, putting $v=x-u$, and separating the resulting double integral into $\int f(u)e^{-iqu}du$ times $\int g(v)e^{-iqv}dv$. For an absolutely integrable pair the interchange is justified by absolute convergence; finite optical [apertures](../../../../../../aperture.md) satisfy suitable integrability assumptions.

In [Fraunhofer diffraction](../../../../../../fraunhofer-diffraction.md), the observed field is the [Fourier transform](../../../../../../fourier-transform-split.md) of the _transmitted complex [aperture](../../../../../../aperture.md) field_. For two identical slits, let $g(x)$ be one slit and use a pair of [Dirac delta](../../../../../../dirac-delta-function.md) distributions to locate the centres:

$$
t(x)=g*[\delta(x-D/2)+\delta(x+D/2)].
$$

Consequently $\widehat t(q)=2\widehat g(q)\cos(qD/2)$. For a rectangular slit, $\widehat g=a\operatorname{sinc}(qa/2)$, giving a [single-slit diffraction](../../../../../../single-slit-diffraction.md) envelope times the [double-slit interference](../../../../../../double-slit-interference.md) factor in intensity. A $\pi$ [phase](../../../../../../phase-waves.md) reversal replaces the plus between the deltas by a minus, giving $\sin(qD/2)$ instead, as in B7.

More generally, an $N$-slit array is a single-aperture function convolved with a finite comb. Its field contains the factor

$$
\sum_{j=0}^{N-1}e^{-iqjD}=e^{-iq(N-1)D/2}\frac{\sin(NqD/2)}{\sin(qD/2)}.
$$

This separates the narrow [diffraction grating](../../../../../../diffraction-grating.md) maxima from the individual-aperture envelope. The same reasoning holds in two transverse dimensions. Multiplying an existing [aperture](../../../../../../aperture.md) by an additional finite mask instead convolves their field transforms and can broaden features. These are operations on complex fields: intensity is the squared modulus of the final field and cannot generally be substituted into the field-level [convolution theorem](../../../../../../convolution-theorem.md).

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
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
