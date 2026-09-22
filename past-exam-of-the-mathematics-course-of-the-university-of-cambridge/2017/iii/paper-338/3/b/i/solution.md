<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the ideal detection convention of one collected [Electron](../../../../../../../electron.md) per detected [photon](../../../../../../../photon.md); otherwise replace [photon](../../../../../../../photon.md) totals by detected [Electron](../../../../../../../electron.md) totals using the [quantum efficiency](../../../../../../../quantum-efficiency.md). Let $A$ be the summed measurement on the [star](../../../../../../../star.md) patch and $B'$ the independent background-only patch. After additive offsets are removed, their means are $Q+B$ and $B$. Independent [Poisson distribution](../../../../../../../poisson-distribution.md) counts have [variance](../../../../../../../variance-split.md) equal to their mean, and a single read of $n$ [detector pixels](../../../../../../../optical-detector-pixel.md) contributes $nr^2$ to each patch's [variance](../../../../../../../variance-split.md). Therefore

$$
\mathbb E(A-B')=Q,\qquad\operatorname{Var}(A-B')=Q+2B+2nr^2,
\qquad
\boxed{Z=\frac{Q}{\sqrt{Q+2B+2nr^2}}.}
$$

The two factors of two arise from the independently measured background and the second patch's [read noise](../../../../../../../read-noise.md), not from doubling the stellar signal. The formula assumes equal background means, independent [detector pixels](../../../../../../../optical-detector-pixel.md) and patch measurements, one read per patch, and negligible [dark current](../../../../../../../dark-current-physics.md) or other noise. Several exposure reads or correlated [detector pixels](../../../../../../../optical-detector-pixel.md) require their own [variance](../../../../../../../variance-split.md) and [covariance](../../../../../../../covariance.md) terms.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
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
