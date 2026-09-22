<h1 id="5/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a rubber-like solid, a [spring](../../../../../../spring.md) is a first model of recoverable [elasticity](../../../../../../elasticity-physics-split.md), while a viscous element can represent rate-dependent loss and delayed recovery. An immediate extension followed by bounded delayed [material creep](../../../../../../creep-deformation.md) is represented by [series spring and Voigt-branch creep](../../../../../../series-spring-and-voigt-branch-creep.md), a [standard linear solid model](../../../../../../standard-linear-solid-model.md):

$$
\varepsilon(t)=\frac{\sigma_0}{E_0}
+\frac{\sigma_0}{E_1}(1-e^{-E_1t/\eta}).
$$

The first term is immediate and recoverable; the second is delayed and also recoverable. For a load held until $t=t_h$, [recovery after a finite-duration stress load](../../../../../../recovery-after-a-finite-duration-stress-load.md) predicts an immediate drop of $\sigma_0/E_0$ on unloading, followed by

$$
\boxed{\varepsilon(t)=\frac{\sigma_0}{E_1}(1-e^{-t_h/\tau})e^{-(t-t_h)/\tau},\qquad\tau=\frac\eta{E_1},\quad t>t_h.}
$$

This supplies a direct comparison with a loading-and-unloading observation: the model returns completely to its original length, with separate immediate and delayed recovery. A single [Kelvin-Voigt model](../../../../../../kelvin-voigt-model.md) misses the immediate compliance, while a free series [dashpot](../../../../../../dashpot.md) would predict unbounded flow that an intact crosslinked rubber need not show. A [spring](../../../../../../spring.md) alone suffices over a timescale on which the measured response is effectively immediate and elastic.

These are local small-strain analogues. Large-strain [rubber elasticity](../../../../../../rubber-elasticity.md) is nonlinear, nearly incompressible and sensitive to temperature, loading history and internal damage. A small set of linear [springs](../../../../../../spring.md) and [dashpots](../../../../../../dashpot.md) cannot reproduce every amplitude, timescale or [hysteresis](../../../../../../hysteresis.md) loop.

No numerical rubber trace or fitted constants are supplied, so these are explicit qualitative model predictions for comparison with the practical observations.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [E](../../e.md)
3. [5](../../../5.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the materials science course of the University of Cambridge](../../../../../split.md)
7. [Materials science course of the University of Cambridge](../../../../../../materials-science-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
