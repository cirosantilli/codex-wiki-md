<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The number of [spaxels](../../../../../../../spaxel.md) is $M=(\beta/\theta)^2$. To obtain definite scaling exponents, keep the [spectral resolving power](../../../../../../../spectral-resolving-power.md), [wavelength](../../../../../../../wavelength.md) interval, [diffraction grating](../../../../../../../diffraction-grating.md) [angles](../../../../../../../angle.md) and groove spacing, input [focal ratio](../../../../../../../focal-ratio.md), and [photodetector](../../../../../../../photodetector.md) sampling of a [spectral resolution element](../../../../../../../spectral-resolution-element.md) fixed. A fixed [photodetector](../../../../../../../photodetector.md) then accommodates a fixed number $M_0$ of spectra, so $N\simeq M/M_0$ (rounded up in an actual instrument). The corresponding [etendue](../../../../../../../etendue.md) per [spaxel](../../../../../../../spaxel.md) scales as $\theta^2$. Angular ratios are independent of whether both [angles](../../../../../../../angle.md) are in arcseconds; optical invariant equations use radians.

Write $b$ for the collimated beam [diameter](../../../../../../../diameter.md). The [diffraction grating](../../../../../../../diffraction-grating.md) result $R\theta D=W(\sin\alpha+\sin\beta)$ gives $b\propto W\propto\theta$. A fixed [collimator](../../../../../../../collimator.md) [focal ratio](../../../../../../../focal-ratio.md) gives $f_{\rm coll}\propto b\propto\theta$. With a fixed image width $p$ in [photodetector](../../../../../../../photodetector.md) [detector pixels](../../../../../../../optical-detector-pixel.md), the invariant $\theta D=pA_{\rm cam}/f_{\rm cam}$ and $A_{\rm cam}\propto\theta$ instead imply $f_{\rm cam}$ is constant: the [optical camera](../../../../../../../optical-camera.md) [focal ratio](../../../../../../../focal-ratio.md) increases as $1/\theta$.

In a simple on-axis beam-envelope model, each [collimator](../../../../../../../collimator.md) and collimated disperser space has area proportional to $b^2$ and length proportional to $b$, whereas the [optical camera](../../../../../../../optical-camera.md) cone has area proportional to $b^2$ and fixed length. Hence

$$
\boxed{V_{\rm coll}\propto\theta^3,\quad V_{\rm grat}\propto\theta^3,\quad V_{\rm cam}\propto\theta^2,\quad
V_{\rm total}\simeq M(a\theta^3+b_0\theta^2).}
$$

The constants include $1/M_0$ and fixed design parameters. At fixed field size, the combined [collimator](../../../../../../../collimator.md) and [diffraction grating](../../../../../../../diffraction-grating.md) volumes scale as $M\theta^3\propto\theta\propto M^{-1/2}$, while the combined [optical camera](../../../../../../../optical-camera.md) beam-cone volume scales as $M\theta^2\propto1$.

These are [integral-field spectrograph volume scaling](../../../../../../../integral-field-spectrograph-volume-scaling.md) laws for the shrinking beam, not a claim that the whole apparatus can shrink without a floor. A [photodetector](../../../../../../../photodetector.md) of fixed transverse size $d_0$ needs space for its field: an [optical camera](../../../../../../../optical-camera.md) envelope interpolating between [optical pupil](../../../../../../../optical-pupil.md) width $b$ and [photodetector](../../../../../../../photodetector.md) width $d_0$ has volume proportional to $f_{\rm cam}(b^2+bd_0+d_0^2)$, rather than just $f_{\rm cam}b^2$. Replication then adds terms scaling as $M\theta$ and $M$, which can grow as the [spaxels](../../../../../../../spaxel.md) shrink. Other field clearances and mechanical margins also change the asymptote. Without the fixed spectral/design assumptions above, the information in the question does not determine unique physical-volume exponents. The role of fixed [photodetector](../../../../../../../photodetector.md) size and beam spread is discussed in [Allington-Smith's instrument scaling model](https://academic.oup.com/mnras/article/376/3/1099/1746825).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
