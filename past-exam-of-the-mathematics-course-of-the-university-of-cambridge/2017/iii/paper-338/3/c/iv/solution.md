<h1 id="3/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If spatial illumination is stable between the two sums, it acts just like the sensitivity factor: the mean ratio remains one but each [detector pixel](../../../../../../../optical-detector-pixel.md) has a different shot-noise [variance](../../../../../../../variance-split.md). A whole-image [standard deviation](../../../../../../../standard-deviation.md) is disproportionately influenced by faint [detector pixels](../../../../../../../optical-detector-pixel.md), so substituting a global [arithmetic mean](../../../../../../../arithmetic-mean.md) signal generally underestimates [detector conversion gain](../../../../../../../detector-conversion-gain.md). If the illumination pattern differs between the sums, their noise-free ratio is not constant; its structure adds apparent [variance](../../../../../../../variance-split.md) and causes a further systematic error.

**Use locally uniform signal bins or subregions, remove offsets, mask defective or saturated [detector pixels](../../../../../../../optical-detector-pixel.md), and propagate the local shot and read [variances](../../../../../../../variance-split.md).** In the stable-pattern case a useful alternative to pooling raw ratios is the normalized difference

$$
U_i=\frac{A_i-B_i}{\sqrt{A_i+B_i}}.
$$

At high signal and negligible [read noise](../../../../../../../read-noise.md), treating the denominator at its mean gives $\operatorname{Var}(U_i)\simeq(2N_i/g)/(2N_i)=1/g$, independent of the illumination. Thus a [variance](../../../../../../../variance-split.md) fit or $g\simeq1/\operatorname{Var}(U)$ can use a spatially varying flat without the arithmetic/harmonic mismatch. Measured noisy denominators cause higher-order corrections, so independent or smoothed signal estimates can be preferable. Fit and subtract a genuine changing illumination pattern before noise analysis, using sufficient smoothing not to fit away the random noise. Arbitrary flat-field normalization without propagating its noise does not by itself recover the original gain.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
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
