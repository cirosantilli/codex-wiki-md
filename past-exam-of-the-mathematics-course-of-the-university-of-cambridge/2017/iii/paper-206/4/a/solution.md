<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [random-slope linear mixed model](../../../../../../random-slope-linear-mixed-model.md) is

$$
Y_{ij}=\beta_0+\beta_1t_{ij}+b_jt_{ij}+\varepsilon_{ij},\qquad b_j\overset{\rm iid}{\sim}N(0,\tau^2),\quad \varepsilon_{ij}\overset{\rm iid}{\sim}N(0,\sigma^2),
$$

with [independence](../../../../../../independent-random-variables.md) between the [random effects](../../../../../../random-effect.md) and errors. The estimates are

$$
\widehat\beta_0=24.32646,\quad\widehat\beta_1=0.70005,\quad\widehat\tau^2=0.00642,\quad\widehat\sigma^2=374.64823.
$$

Incubators are treated as exchangeable representatives of possible growth environments, so a [random slope](../../../../../../random-slope.md) permits their growth rates to differ while estimating a population mean growth rate. The formula `0+hours` deliberately removes a [random intercept](../../../../../../random-intercept.md): larvae are assigned only after hatching, so it is reasonable to assume no incubator-specific baseline at time zero. Random assignment supports this common-baseline assumption in [expectation](../../../../../../expected-value.md); it does not prove that observed initial sizes or other baseline differences are exactly identical.

For a new incubator, no observations are available to estimate its realized [random slope](../../../../../../random-slope.md), and its mean effect is zero. Under [squared-error loss](../../../../../../squared-error-loss.md) the best prediction integrates over that effect and the residual error:

$$
\boxed{\widehat Y(10,\text{new incubator})=24.32646+10(0.70005)=31.32696\ \mathrm{mm}.}
$$

This is the plug-in conditional [expectation](../../../../../../expected-value.md) given the population parameters, rather than a prediction using a fitted effect from one of the four existing incubators. Ignoring parameter-estimation uncertainty, the prediction [variance](../../../../../../variance-split.md) for a new individual is $10^2\widehat\tau^2+\widehat\sigma^2=375.29023$; it is not just the uncertainty in the population mean.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
