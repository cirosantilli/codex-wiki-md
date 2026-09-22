<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

`read.table(...,header=T)` reads four grouped rows with column names. The displayed outcome counts give the observed risks $0.1519,0.2145,0.2611,0.5111$ in the indicated factor order. `rbind` in the first test pools over predisposition: the two rows represent no cannabis use and some use, with event/non-event counts $(341,1775)$ and $(82,238)$. Thus the pooled risks are $341/2116=0.1612$ and $82/320=0.2563$. This test concerns the marginal [statistical association](../../../../../statistical-association.md) between use and outcome, not an association adjusted for predisposition.

Under independence, expected counts in the two-by-two [contingency table](../../../../../contingency-table.md) are $E_{ij}=O_{i+}O_{+j}/N$. The ordinary [Pearson chi-squared statistic](../../../../../pearson-chi-squared-statistic.md) is $17.5183$. The printed $16.8618$ is reproduced by the default two-by-two [Yates continuity correction](../../../../../yates-s-correction-for-continuity.md):

$$
X_Y^2=\sum_{i,j}\frac{(|O_{ij}-E_{ij}|-1/2)^2}{E_{ij}}=16.8618.
$$

All absolute differences here exceed one half. Comparison with a [chi-squared distribution](../../../../../chi-squared-distribution.md) on one [statistical degree of freedom](../../../../../statistical-degrees-of-freedom.md) gives $p=4.02\times10^{-5}$. **There is strong evidence of marginal association.** The simplified output omits the usual continuity-correction wording, but its numerical value shows which statistic was used.

`attach` makes the data columns available by name, and `tot=with+without` obtains group sizes $1936,275,180,45$. The grouped [binomial regression](../../../../../binomial-regression.md) fits $Y_g\sim\operatorname{Bin}(n_g,\pi_g)$, with response $Y_g/n_g$ and prior weights $n_g$. These weights tell R the binomial denominator; treating the four proportions as four equally precise individual observations would be wrong. The default [logit link](../../../../../logit.md) is

$$
\eta_g=\log\frac{\pi_g}{1-\pi_g},\qquad
\pi_g=\frac{e^{\eta_g}}{1+e^{\eta_g}}.
$$

Let $A$ indicate some use and $B$ indicate predisposition. The additive [logistic regression](../../../../../logistic-regression.md) specifies $\eta=a+bA+cB$. Its [log-likelihood](../../../../../log-likelihood.md), including the binomial constants, is

$$
\ell=\sum_g\left[\log\binom{n_g}{Y_g}+Y_g\eta_g-n_g\log(1+e^{\eta_g})\right].
$$

Differentiation gives [score equations](../../../../../score-equation.md) $X^T(Y-n\pi)=0$ and [Fisher information matrix](../../../../../fisher-information-matrix.md) $X^TWX$, where $W_{gg}=n_g\pi_g(1-\pi_g)$. [Fisher scoring](../../../../../scoring-algorithm.md) solves these equations, and the inverse fitted [Fisher information matrix](../../../../../fisher-information-matrix.md) gives the reported approximate coefficient [variances](../../../../../variance-split.md). The number of scoring iterations records numerical convergence, not degrees of freedom or statistical evidence.

The intercept corresponds to no use and no predisposition and gives baseline fitted risk $\operatorname{logit}^{-1}(-1.73881)=0.1495$. The additive coefficients imply common adjusted [odds ratios](../../../../../odds-ratio.md):

$$
\boxed{\operatorname{OR}_{A\mid B}=e^{0.53847}=1.713,\qquad
\operatorname{OR}_{B\mid A}=e^{0.82824}=2.289.}
$$

They multiply the odds, not the risks. The [Wald tests](../../../../../wald-test.md) divide the estimates by their [standard errors](../../../../../standard-error.md) and use a [standard normal distribution](../../../../../standard-normal-distribution.md); both predictors have small two-sided [p-values](../../../../../p-value.md). Approximate $95\%$ [confidence intervals](../../../../../confidence-interval.md) for these [odds ratios](../../../../../odds-ratio.md) are $(1.296,2.266)$ and $(1.685,3.110)$, obtained by exponentiating the log-scale intervals. The intercept test against zero asks whether the reference risk equals one half, and is not a test of either exposure association. The binomial dispersion is assumed to be one because $\operatorname{Var}(Y_g)=n_g\pi_g(1-\pi_g)$; the output does not demonstrate independence or rule out extra-binomial variation.

There are four grouped probabilities and three fitted coefficients, leaving one [residual degree of freedom](../../../../../residual-degrees-of-freedom.md). The fitted risks are approximately $(0.1495,0.2314,0.2869,0.4080)$. The [binomial deviance](../../../../../binomial-deviance.md) compares this fit with the four unrestricted observed proportions:

$$
D=2\sum_g\left[Y_g\log\frac{Y_g}{n_g\widehat\pi_g}
+(n_g-Y_g)\log\frac{n_g-Y_g}{n_g(1-\widehat\pi_g)}\right]=3.0733.
$$

The [deviance goodness-of-fit test](../../../../../deviance-goodness-of-fit-test.md) against $\chi^2_1$ has [p-value](../../../../../p-value.md) $0.0796$. The common-odds-ratio fit is not rejected at $5\%$, although the doubly exposed group's observed risk exceeds its fitted risk appreciably and suggests possible [interaction](../../../../../interaction-statistics.md).

The second formula adds $\delta AB$. Its four coefficients fit all four probabilities, making a [saturated statistical model](../../../../../saturated-statistical-model.md) with zero grouped [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md). The near-zero deviance is roundoff from exact interpolation; it supplies no remaining grouped lack-of-fit test. Unlike Q1's unreplicated Gaussian fit, however, these grouped responses represent many independent Bernoulli trials, and their binomial [variances](../../../../../variance-split.md) are specified by their sizes and probabilities. Coefficient [standard errors](../../../../../standard-error.md) remain available from binomial information without estimating dispersion from the zero residual degrees of freedom.

Indeed, let $\eta_{ab}=\log[Y_{ab}/(n_{ab}-Y_{ab})]$ be the fitted cell [logit link](../../../../../logit.md) value. The saturated coefficients are

$$
a=\eta_{00},\qquad b=\eta_{10}-\eta_{00},\qquad
c=\eta_{01}-\eta_{00},\qquad
\delta=\eta_{11}-\eta_{10}-\eta_{01}+\eta_{00}.
$$

These calculations yield the printed estimates. The [delta method](../../../../../delta-method.md) gives $\operatorname{Var}(\widehat\eta_{ab})\approx1/Y_{ab}+1/(n_{ab}-Y_{ab})$, and independent groups make the [variance](../../../../../variance-split.md) of $\widehat\delta$ the sum of all eight reciprocal counts. Its square root is $0.37857$, reproducing the printed [standard error](../../../../../standard-error.md).

The saturated [logistic regression](../../../../../logistic-regression.md) describes the conditional [odds ratios](../../../../../odds-ratio.md) as follows:

$$
\operatorname{OR}_{A\mid B=0}=e^{0.42235}=1.526,\qquad
\operatorname{OR}_{A\mid B=1}=e^{0.42235+0.66230}=2.958,
$$



$$
\operatorname{OR}_{B\mid A=0}=e^{0.67989}=1.974,\qquad
\operatorname{OR}_{B\mid A=1}=e^{0.67989+0.66230}=3.827.
$$

Thus the main coefficients now concern effects at the other factor's reference level. [Logistic interaction as a ratio of odds ratios](../../../../../logistic-interaction-as-a-ratio-of-odds-ratios.md) gives $e^\delta=1.939$, with approximate $95\%$ [confidence interval](../../../../../confidence-interval.md) $(0.923,4.073)$. The interaction [Wald test](../../../../../wald-test.md) has $p=0.0802$, while the nested [likelihood-ratio test](../../../../../likelihood-ratio-test.md) uses deviance difference $3.0733$ on one [statistical degree of freedom](../../../../../statistical-degrees-of-freedom.md) and has $p=0.0796$. **The data suggest a larger odds association in predisposed subjects, but do not establish this interaction at the conventional $5\%$ level.** This conclusion is specific to the odds scale; absolute-risk differences can vary even with no logit-scale interaction.

The [Akaike information criterion](../../../../../akaike-information-criterion.md) is $-2\widehat\ell+2k$. The additive fit has $k=3$ and AIC $31.766$; the interaction fit has $k=4$ and AIC $30.692$. The extra coefficient improves twice the log-likelihood by $3.0733$ but incurs penalty $2$, so AIC falls by only $1.0733$. It weakly favors the larger fit rather than decisively establishing an interaction, and AIC is not a [p-value](../../../../../p-value.md).

The marginal [odds ratio](../../../../../odds-ratio.md) $1.793$ and the fitted conditional [odds ratios](../../../../../odds-ratio.md) are different quantities. Predisposition is associated with both use frequency and outcome, so [confounding](../../../../../confounding.md) is a substantive possibility; [noncollapsibility of the odds ratio](../../../../../noncollapsibility-of-the-odds-ratio.md) also means marginal and conditional odds ratios need not agree. This is an observational association analysis with only one adjustment factor. It does not by itself establish a causal effect, exclude other [confounding](../../../../../confounding.md), or validate the assumed independent binomial sampling.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
