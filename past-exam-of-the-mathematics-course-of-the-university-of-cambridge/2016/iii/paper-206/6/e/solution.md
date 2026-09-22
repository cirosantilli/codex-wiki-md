<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [generalized additive mixed model](../../../../../../generalized-additive-mixed-model.md) fits

$$
Y_{ij}=\alpha+f(t_{ij})+u_j+\varepsilon_{ij},\qquad
u_j\sim N(0,\tau_0^2),\quad\varepsilon_{ij}\sim N(0,\sigma^2),
$$

where $u_j$ denotes the furnace [random intercept](../../../../../../random-intercept.md) and $f$ is a centered penalized [cubic regression spline](../../../../../../cubic-regression-spline.md). Its wiggly components have a mixed-model representation; there is no explicit furnace-specific [random slope](../../../../../../random-slope.md) in this formula.

**The plotted smooth gives no evidence that a nonparametric [fixed effect](../../../../../../fixed-effect.md) is needed.** It is essentially a straight rising line, and `s(stir,1)` indicates [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) close to one. The wider bands at extreme stirring rates reflect uncertainty, not detected nonlinearity. A linear fixed stirring effect is adequate on this evidence.

If the three supplied [Akaike information criterion](../../../../../../akaike-information-criterion.md) values are on a common valid likelihood basis, choose **`strength_model3`**, the fixed linear slope plus random-intercept model: its AIC $206.6408$ is smallest, versus $208.3243$ for the additional [random slope](../../../../../../random-slope.md) and $210.3425$ for the smooth. The differences are $1.6835$ and $3.7017$, respectively, so especially the random-slope comparison represents modest support rather than decisive evidence. Retaining the population slope is consistent with part (c); this choice removes only its random variation.

There is a likelihood-basis caveat in the literal printed commands. `lmer` fits by REML by default, whereas the Gaussian `gamm` call defaults to ML; direct AIC on these objects need not compare the same type of likelihood. Moreover the earlier ML ANOVA prints $210.22$ for `strength_model`, whereas this table prints $208.3243$, so these numbers should not silently be treated as one identical ML fit. To obtain a defensible common comparison, fit all candidates to the same observations by ML:
```
fit_slope <- update(strength_model, REML = FALSE)
fit_intercept <- update(strength_model3, REML = FALSE)
fit_smooth <- mgcv::gamm(strength ~ s(stir, bs = "cr"),
random = list(furnace = ~ 1), method = "ML")
AIC(fit_slope, fit_intercept, fit_smooth$lme)
```
The supplied ranking favours the simpler random-intercept model; the displayed original calls alone do not certify that ranking as a consistent ML comparison. This distinction is particularly relevant when the smooth changes the fixed-effect space. The Gaussian `gamm` ML default and mixed-model representation are documented at [https://stat.ethz.ch/R-manual/R-devel/library/mgcv/html/gamm.html.](https://stat.ethz.ch/R-manual/R-devel/library/mgcv/html/gamm.html.)

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
