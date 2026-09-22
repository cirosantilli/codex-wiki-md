<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because no family is specified, the command fits a Gaussian identity-link [generalized additive model](../../../../../../generalized-additive-model.md):

$$
Y_i=\alpha+s_1(a_i)+s_2(w_i)+\varepsilon_i,\qquad \varepsilon_i\overset{\rm iid}{\sim}N(0,\sigma^2).
$$

The $s_j$ are centered [penalized regression splines](../../../../../../penalized-regression-spline.md) with cubic regression bases; centering separates them from the intercept. The age curve in the original figure falls to a minimum near age 25, then rises markedly, particularly from about 40 onwards. Its [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) are $4.05$, reflecting curvature. The white-cell curve has [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) one and is nearly flat with a slight positive slope; the pointwise uncertainty bands are consistent with no substantial effect. These plots display centered partial mean contributions, not numbers of prescriptions by themselves.

A simpler mean model keeps the age [regression spline](../../../../../../regression-spline.md) and replaces the white-cell smooth by a linear term. A separate issue is that the response is a nonnegative count: a [Poisson regression](../../../../../../poisson-regression.md) with [logarithmic link function](../../../../../../logarithmic-link-function.md) respects that support and positivity of the mean. A reasonable candidate is
```
model1p <- gam(npres ~ s(age, bs="cr") + wbc, family=poisson(link="log"))
gam.check(model1p)
```
If diagnostics show [overdispersion](../../../../../../overdispersion.md), one can fit
```
model1nb <- gam(npres ~ s(age, bs="cr") + wbc, family=nb(link="log"))
```
using a [negative binomial regression](../../../../../../negative-binomial-regression.md). Alternatively, if a Gaussian approximation is adequate, the minimal simplification is `gam(npres ~ s(age, bs="cr") + wbc)`. These are candidates to compare by diagnostics and validation, rather than guaranteed improvements from the partial plots alone. **Retain the curved age effect; consider a linear or removable white-cell effect, and assess an appropriate count family.** Refit before interpreting the old curves on a new link scale.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
