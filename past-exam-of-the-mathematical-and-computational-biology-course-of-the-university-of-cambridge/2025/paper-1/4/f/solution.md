<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [regression diagnostics](../../../../../regression-diagnostics.md) raise concerns about the mean and [variance](../../../../../variance-split.md) assumptions. The residual-versus-fitted smoother is curved rather than horizontal, and the scale-location plot suggests changing residual spread, contrary to [homoscedasticity](../../../../../homoscedasticity.md). Diagonal bands are expected when an [integer](../../../../../integer-split.md)-valued response is fitted by a continuous model, since each fixed response value gives $r=y-\widehat y$. They are not, by themselves, proof of a failed mean model. The residual [Q-Q plot](../../../../../q-q-plot.md) is broadly linear but has tail departures and unusual observations, so exact [normality](../../../../../normality-statistics.md) is questionable.

The [Cook's distance](../../../../../cook-s-distance.md) plot identifies observations worth checking for recording errors and influence on the age estimate. A rough $4/n\simeq0.023$ screening threshold flags several points, but it is not an automatic deletion rule. Repeat the fit with and without influential observations as a sensitivity analysis and report material changes.

The bird [random intercept](../../../../../random-intercept.md) [Q-Q plot](../../../../../q-q-plot.md) has a pronounced upper-tail departure; the year plot is closer to a line, although eleven groups give little power to assess [normality](../../../../../normality-statistics.md). These plotted effects are estimated, shrunken [conditional mode of Gaussian random effects](../../../../../conditional-mode-of-gaussian-random-effects.md), not independent observed draws from the latent [normal distribution](../../../../../normal-distribution.md), so their appearance requires care.

The analysis is therefore provisional. Check a nonlinear age effect, the changing residual [variance](../../../../../variance-split.md), dependence beyond the fitted [random intercepts](../../../../../random-intercept.md), and a response model appropriate for counts. If clutch size is known, a [binomial distribution](../../../../../binomial-distribution.md) model for hatched eggs out of available eggs may be more meaningful. A bootstrap from the existing Gaussian model cannot validate the assumptions questioned by these plots. Distinguishing within-bird ageing from between-bird differences would also strengthen interpretation.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
