<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Retain the [random-slope linear mixed model](../../../../../../random-slope-linear-mixed-model.md) of part (e), but replace the within-laboratory independent error covariance by [continuous-time autoregressive residual correlation](../../../../../../continuous-time-autoregressive-residual-correlation.md):

$$
\operatorname{Cov}(\varepsilon_{ij},\varepsilon_{kj})
=\sigma^2e^{-\kappa|t_{ij}-t_{kj}|},\qquad\kappa>0.
$$

Errors from different laboratories remain independent and are independent of the [random slopes](../../../../../../random-slope.md). The resulting marginal [covariance](../../../../../../covariance.md) within laboratory $j$ is

$$
\tau^2t_{ij}t_{kj}+\sigma^2e^{-\kappa|t_{ij}-t_{kj}|}.
$$

The exponential decay applies to the conditional errors, not the entire marginal correlation, which also contains the shared [random slope](../../../../../../random-slope.md).

Use `nlme`, since `lme4::lmer` does not fit this general residual correlation structure. With a data frame containing the observed variables, suitable code is
```
library(nlme)
dat <- data.frame(size = size, days = days, lab = lab)
dat <- dat[order(dat$lab, dat$days), ]
tumour_cor <- lme(size ~ days,
random = ~ 0 + days | lab,
correlation = corCAR1(form = ~ days | lab),
data = dat, method = "REML")
```
Here `corCAR1` estimates $\rho=e^{-\kappa}\in(0,1)$, the error correlation one day apart; correlation at separation $\Delta$ is $\rho^{|\Delta|}$. This works for noninteger or unequally spaced days. At equally spaced integer days, `corAR1(form = ~ days | lab)` gives the corresponding discrete-time construction when its parameter is positive. Distinct times within each error series are required: separate tumours with repeated day values should have separate series identifiers or an additional independent-error component, rather than being assigned perfectly correlated errors. The [continuous-time autoregressive residual correlation](../../../../../../continuous-time-autoregressive-residual-correlation.md) documentation describes the grouping and continuous-time conventions: [https://stat.ethz.ch/R-manual/R-patched/library/nlme/html/corCAR1.html.](https://stat.ethz.ch/R-manual/R-patched/library/nlme/html/corCAR1.html.) The fixed `days` term here follows the fitted output rather than the inconsistent command in part (e).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
