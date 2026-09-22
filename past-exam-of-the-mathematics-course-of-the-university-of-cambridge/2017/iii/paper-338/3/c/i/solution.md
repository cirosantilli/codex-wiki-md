<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $k=m/2$. After offset subtraction, each summed image has mean $N$ [analogue-to-digital units](../../../../../../../analogue-to-digital-unit.md) per [detector pixel](../../../../../../../optical-detector-pixel.md). For a constant [detector conversion gain](../../../../../../../detector-conversion-gain.md) $g$ and independent [Poisson distribution](../../../../../../../poisson-distribution.md) detected counts, $\operatorname{Var}(A)=\operatorname{Var}(B)=N/g$: summing $k$ independent frames adds both their means and [variances](../../../../../../../variance-split.md). Here $N$ is the mean of the sum, not one frame.

Write $A=N+a$, $B=N+b$. At high counts, the [delta method](../../../../../../../delta-method.md) gives $A/B\simeq1+a/N-b/N$. Independence therefore gives

$$
E^2\simeq\frac{\operatorname{Var}(A)+\operatorname{Var}(B)}{N^2}=\frac{2}{gN},\qquad
\boxed{g\simeq\frac{2}{NE^2}.}
$$

Thus the formula is a high-signal [gain estimation from flat-field ratios](../../../../../../../gain-estimation-from-flat-field-ratios.md), not an exact identity for a ratio of [random variables](../../../../../../../random-variable-split.md). A [Poisson distribution](../../../../../../../poisson-distribution.md) denominator can even be zero at low counts. The exposures must be linear and unsaturated, offsets removed, and [read noise](../../../../../../../read-noise.md) negligible. Being close to saturation increases the signal but does not establish linearity; clipping or charge-induced correlations biases a [variance](../../../../../../../variance-split.md) estimate. A large ensemble of suitable [detector pixels](../../../../../../../optical-detector-pixel.md) supplies the measured [standard deviation](../../../../../../../standard-deviation.md). In normal [photodetector](../../../../../../../photodetector.md) terminology $g$ is collected [Electrons](../../../../../../../electron.md) per [ADU](../../../../../../../analogue-to-digital-unit.md), consistent with detected [photons](../../../../../../../photon.md) here only under the stated unit-yield convention; see [the instrument gain definition](https://hst-docs.stsci.edu/wfc3dhb/chapter-5-wfc3-uvis-sources-of-error/5-1-gain-and-read-noise).

## ↑ Ancestors (12)

1. [I](../i.md)
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
