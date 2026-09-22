<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

There is a genuine syntax error in the printed command: `random=list(...)` must be a separate argument, following a comma rather than a plus. The intended call is
```
model2 <- gamm(npres ~ s(age, bs="cr") + s(wbc, bs="cr"), random=list(doctor=~age))
```
With the default Gaussian family, this [generalized additive mixed model](../../../../../../generalized-additive-mixed-model.md) is

$$
\boxed{Y_{ij}=\alpha+s_1(a_{ij})+s_2(w_{ij})+b_{0j}+b_{1j}a_{ij}+\varepsilon_{ij}.}
$$

Here $(b_{0j},b_{1j})^T\overset{\rm iid}{\sim}N_2(0,D)$ across doctors, $D$ is an estimated [covariance matrix](../../../../../../covariance-matrix.md), and the Gaussian errors have [variance](../../../../../../variance-split.md) $\sigma^2$ and are independent of the [random effects](../../../../../../random-effect.md). The formula `~age` includes a [random intercept](../../../../../../random-intercept.md) as well as a [random slope](../../../../../../random-slope.md); it does not force these two effects to be uncorrelated.

The [random intercept](../../../../../../random-intercept.md) allows different prescribing baselines, and the [random slope](../../../../../../random-slope.md) allows doctor-specific linear modifications to the population age curve. Conditional on these effects the observations are independent under the model, whereas two patients of the same doctor have additional [covariance](../../../../../../covariance.md) $(1,a_{ij})D(1,a_{kj})^T$. This accounts for [clustered data](../../../../../../clustered-data.md) and avoids treating doctor variation as independent patient-level noise. The population smooth and doctor-specific predictions are different targets. With only four doctors, estimates of the random-effect [covariance](../../../../../../covariance.md) can be imprecise; the Gaussian support issue for counts also remains. **The new model accounts for doctor-specific baselines and age slopes.**

## ↑ Ancestors (11)

1. [E](../e.md)
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
