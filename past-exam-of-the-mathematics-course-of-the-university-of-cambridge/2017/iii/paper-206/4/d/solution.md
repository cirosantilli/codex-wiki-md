<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Add a location-specific [random intercept](../../../../../../random-intercept.md) to the [random-slope linear mixed model](../../../../../../random-slope-linear-mixed-model.md):

$$
\boxed{Y_i=\beta_0+\beta_1t_i+b_{j(i)}t_i+u_{\ell(i)}+\varepsilon_i,\qquad u_\ell\overset{\rm iid}{\sim}N(0,\omega^2).}
$$

Take the location effects, incubator slopes and individual errors to be mutually independent, with the original [variances](../../../../../../variance-split.md) $\tau^2$ and $\sigma^2$. The [random intercept](../../../../../../random-intercept.md) models variation already present at hatching because of the origin of the eggs. Because larvae are subsequently assigned to incubators, location and incubator are [crossed random effects](../../../../../../crossed-random-effects.md), not automatically nested groups. The corresponding code is
```
fly.model.loc <- lmer(size ~ hours + (0+hours|incubator) + (1|location))
```
The resulting [covariance](../../../../../../covariance.md) between two observations contains $\omega^2$ if they share a location and $\tau^2t_it_k$ if they share an incubator. If the three named locations themselves are the only populations of interest, use a fixed location factor instead:
```
fly.model.loc.fixed <- lmer(size ~ hours + location + (0+hours|incubator))
```
Choosing between these interpretations depends on the inferential target; with only three locations, a location [variance](../../../../../../variance-split.md) component will be weakly estimated.

## ↑ Ancestors (11)

1. [D](../d.md)
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
