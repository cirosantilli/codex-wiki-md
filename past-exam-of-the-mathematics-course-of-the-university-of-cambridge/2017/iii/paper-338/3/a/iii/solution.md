<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [speckle contrast of a sinusoidal wavefront error](../../../../../../../speckle-contrast-of-a-sinusoidal-wavefront-error.md) gives a peak modal [wave amplitude](../../../../../../../wave-amplitude.md) $h_0=(\lambda/\pi)\sqrt C$. If all $M$ residual modes have that [wave amplitude](../../../../../../../wave-amplitude.md), their coefficient norm is $H_{\rm coeff}=\sqrt M\,h_0$. Substituting the printed quadrant count gives the intended expression

$$
\boxed{H_{\rm coeff}=\frac{N\lambda\sqrt C}{4\sqrt\pi}.}
$$

There is a normalization issue if this quantity is called physical spatial [root mean square](../../../../../../../root-mean-square.md) [wavefront error](../../../../../../../wavefront-error.md). For $h(\mathbf r)=\sum_k h_{0k}\cos(2\pi\mathbf u_k\cdot\mathbf r/D+\psi_k)$, the actual pupil-averaged value is

$$
h_{\rm rms}^2=\sum_{k,l}h_{0k}h_{0l}\langle s_ks_l\rangle_{\rm pupil},\qquad s_k=\cos(2\pi\mathbf u_k\cdot\mathbf r/D+\psi_k).
$$

On an orthogonal full-period basis, $\langle s_k^2\rangle=1/2$ and cross terms vanish. Alternatively, independent uniform random [wave phases](../../../../../../../phase-waves.md) give this result after [wave phase](../../../../../../../phase-waves.md) averaging, even on a circular [optical pupil](../../../../../../../optical-pupil.md). With the same $M$ and equal contrasts the physical RMS is then

$$
\boxed{\sqrt{\mathbb E_{\psi}h_{\rm rms}^2}=\sqrt{\frac M2}\,h_0=\frac{N\lambda\sqrt C}{4\sqrt{2\pi}}.}
$$

A single full-period [cosine](../../../../../../../cosine.md) already demonstrates the issue: its RMS is $h_0/\sqrt2$, not $h_0$. On the actual circular [optical pupil](../../../../../../../optical-pupil.md), any nonconstant unit-peak [cosine](../../../../../../../cosine.md) also has mean square strictly less than one; averaging over its [wave phase](../../../../../../../phase-waves.md) gives exactly $1/2$. On a finite circular [optical pupil](../../../../../../../optical-pupil.md), phase-dependent mode overlaps can additionally matter. If a constant piston is removed before computing RMS, replace the mode Gram [matrix](../../../../../../../matrix.md) by its centred [optical pupil](../../../../../../../optical-pupil.md) [covariance](../../../../../../../covariance.md). The printed value can be recovered as a modal coefficient norm, or by counting $2M$ orthogonal peak-amplitude quadratures in the physical RMS; neither convention is specified by the quoted mode definition. This is the distinction between [modal amplitude norm versus wavefront RMS](../../../../../../../modal-amplitude-norm-versus-wavefront-rms.md), not a correction silently made to the PDF. Unequal residual contrasts require $\mathbb E_{\psi}h_{\rm rms}^2=\lambda^2\sum_k C_k/(2\pi^2)$, so one speckle's $C$ alone cannot determine the total RMS. The weak-aberration approximation also requires the total [wave phase](../../../../../../../phase-waves.md) error to stay small, not merely each coefficient separately.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
