<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $N$ be the input photoelectron count and $\mu=\eta Q$ its mean, with [quantum efficiency](../../../../../../../quantum-efficiency.md) $\eta$ and mean incident photon count $Q$. Independent arrivals give a [Poisson distribution](../../../../../../../poisson-distribution.md), so $\operatorname{Var}N=\mathbb EN=\mu$. Conditional on $N$, the preceding [gamma distribution](../../../../../../../gamma-distribution.md) gives $\mathbb E[X\mid N]=gN$ and $\operatorname{Var}(X\mid N)=g^2N$. The [law of total variance](../../../../../../../law-of-total-variance.md) therefore yields

$$
\mathbb EX=g\mu,\qquad
\operatorname{Var}X
=\mathbb E[g^2N]+\operatorname{Var}(gN)
=2g^2\mu.
$$

One contribution is the ordinary [photon shot noise](../../../../../../../photon-shot-noise.md); the other is [multiplication excess noise](../../../../../../../multiplication-excess-noise.md). Thus, neglecting [read noise](../../../../../../../read-noise.md) and backgrounds,

$$
\mathrm{SNR}=\frac{g\mu}{\sqrt{2g^2\mu}}=\sqrt{\frac{\eta Q}{2}},
\qquad \boxed{\eta_{\rm noise\ equivalent}=\frac\eta2.}
$$

This is an excess-noise factor $\sqrt2$ in analog operation: actual photon conversion efficiency has not been halved. At low occupancy, thresholding each pixel as zero or one event can avoid most multiplication noise, but high arrival rates produce coincident events that cannot be counted separately. That is why the high-rate result concerns charge measurement rather than ideal binary photon counting.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
