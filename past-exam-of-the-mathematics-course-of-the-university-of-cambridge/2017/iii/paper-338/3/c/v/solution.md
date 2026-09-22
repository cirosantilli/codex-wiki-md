<h1 id="3/c/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

If temporal variation is spatially uniform, summing all frames in each group still gives independent [Poisson distribution](../../../../../../../poisson-distribution.md) totals, but their means may now be $N_A,N_B$ with ratio $c=N_A/N_B\ne1$. At high counts and negligible [read noise](../../../../../../../read-noise.md), direct propagation gives

$$
\operatorname{Var}(A/B)\simeq\frac{c^2}{g}\left(\frac1{N_A}+\frac1{N_B}\right).
$$

After dividing the ratio image by its measured mean $c$, the appropriate estimator is

$$
\boxed{g\simeq\frac{1/N_A+1/N_B}{\operatorname{Var}((A/B)/c)}.}
$$

The original formula is recovered only for $N_A=N_B=N$. Uniform brightness drift does not automatically create a spatial pattern or extra ratio scatter beyond these changed noise levels; its leading problem is unequal group normalization. Interleave the groups in [time](../../../../../../../time-in-physics.md) or pair exposures of comparable flux, measure their separate means, and propagate shot and [read noise](../../../../../../../read-noise.md) when rescaling. If the spatial pattern or [photodetector](../../../../../../../photodetector.md) sensitivity also evolves, the ratio develops systematic structure that must be modeled or those frames rejected. A normalization inferred from finitely many [detector pixels](../../../../../../../optical-detector-pixel.md) introduces a small shared correlation, which vanishes in the large-pixel limit and can be included in a precise uncertainty analysis.

## ↑ Ancestors (12)

1. [V](../v.md)
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
