<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Substitute $x=\sin^2v$, with $0<v<\pi/2$, when integrating the target density. Since $dx=2\sin v\cos v\,dv$, its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) is

$$
F(x)=\frac2\pi\arcsin\sqrt{x}\qquad(0<x<1).
$$

Inverting gives the [arcsine distribution](../../../../../../arcsine-distribution.md) sampler

$$
\boxed{X=\sin^2\left(\frac{\pi U_1}{2}\right).}
$$

The [inverse transform sampling](../../../../../../inverse-transform-sampling.md) proof in the root solution shows that it has the required [probability density function](../../../../../../probability-density-function.md). Use successive independent uniforms for successive samples. A draw at the endpoint one can be discarded if values strictly inside the support are desired; this event has probability zero under the ideal continuous [uniform distribution](../../../../../../continuous-uniform-distribution.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
