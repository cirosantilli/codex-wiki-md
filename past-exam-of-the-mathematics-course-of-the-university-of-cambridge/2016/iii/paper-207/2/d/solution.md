<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $A_i(s)$ be age in years at follow-up time $s$ and let $G_i\in\{0,1\}$ indicate the genetic risk factor. An age-dependent [log-linear transition intensity model](../../../../../../log-linear-transition-intensity-model.md) is

$$
\boxed{q_{12,i}(s)=\exp\{\theta_0+\theta_A(A_i(s)-50)+\theta_GG_i\}.}
$$

Here $e^{\theta_0}$ is the onset [baseline hazard](../../../../../../baseline-hazard.md) for a 50-year-old without the factor; $e^{\theta_G}$ is the genetic [hazard ratio](../../../../../../hazard-ratio.md), and $e^{\theta_A}$ is the [hazard ratio](../../../../../../hazard-ratio.md) per additional year of age. A smooth function of age could replace the linear age term if a constant age [hazard ratio](../../../../../../hazard-ratio.md) were unsuitable.

Under the stated constant multiplicative [hazard ratios](../../../../../../hazard-ratio.md), the requested extrapolation is therefore **the baseline rate times both multipliers**:

$$
\boxed{q_{12}(60,1)=q\,\alpha_1\alpha_2^{10}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
