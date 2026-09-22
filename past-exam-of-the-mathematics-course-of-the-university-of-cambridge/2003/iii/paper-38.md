# Paper 38

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper38.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper38.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [a](#5/ii/a)
      - [Solution](#5/ii/a/solution)
    - [b](#5/ii/b)
      - [Solution](#5/ii/b/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)

## 1

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The S-Plus input and the data table differ in one entry: the former uses $33$ for the first year in the second male age group, whereas the table has $22$. The displayed coefficients are reproduced by the software vector with $33$, so that is the input analysed here. Using $22$ instead would give a different fit, including an intercept of $36.175$ rather than $37.275$.

The factor grid has $5\times4\times2=40$ rows. Its first factor varies fastest, so the five years run within each age group, and the age groups run within each sex. All three predictors are [regression factors](../../../statistical-modelling.md#regression-factor): in particular the year coefficients are category contrasts, not a fitted linear slope in calendar time. Under reference-level coding, take the first year, youngest age group and men as the [reference levels in a regression factor](../../../statistical-modelling.md#reference-level-in-a-regression-factor). Write $s=1$ for women and $0$ for men, and $I_{yk},I_{aj}$ for the other year and age indicators. The [normal linear model](../../../statistical-modelling.md#normal-linear-model) is

$$
P=\alpha+\sum_{k=2}^5\gamma_kI_{yk}+\lambda s+\sum_{j=2}^4\eta_jI_{aj}+\sum_{j=2}^4\kappa_j sI_{aj}+\varepsilon,\qquad\varepsilon\sim N(0,\sigma^2).
$$

The star in the formula includes both main effects and their [statistical interaction](../../../statistical-model.md#interaction-statistics). There are twelve coefficients: an intercept, four year contrasts, one sex contrast, three age contrasts and three sex-by-age contrasts. Year effects are assumed common across all sex-age combinations; there is no year [interaction term](../../../statistical-model.md#interaction-term). Independent errors with common [variance](../../../variance.md) are additional assumptions of the reported exact tests.

The [least-squares estimator](../../../statistical-modelling.md#ordinary-least-squares-estimators) is $\widehat b=(X^TX)^{-1}X^TP$, where $X$ has rank twelve. Under the [normal linear model](../../../statistical-modelling.md#normal-linear-model),

$$
\widehat b\sim N_{12}(b,\sigma^2(X^TX)^{-1}),\qquad \frac{\mathrm{RSS}}{\sigma^2}\sim\chi^2_{28},
$$

and these quantities are independent. This standard normal-projection theorem gives $s^2=\mathrm{RSS}/28$ and estimated coefficient [standard errors](../../../statistical-inference.md#standard-error) $s\sqrt{(X^TX)^{-1}_{jj}}$. A coefficient estimate divided by its [standard error](../../../statistical-inference.md#standard-error) has a [Student t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution) with 28 [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) under its zero-coefficient null. These are the printed t statistics and two-sided [p-values](../../../statistical-modelling.md#p-value); a printed zero is rounding, not a probability of exactly zero. The option suppresses the coefficient-correlation display.

The fitted intercept $37.275$ is the expected percentage for the reference sex, age and year. Relative to that year, the year changes are $0.375,0.500,1.750,3.000$ percentage points. The last two are individually significant at the conventional five-percent level; the first two are not. The sex coefficient $-18.8$ is the female-minus-male difference in the youngest group. The male age changes are $-7,-12.8,-23$ points. Adding the three [interaction term](../../../statistical-model.md#interaction-term) coefficients gives the female age changes $-5.2,-8.2,-13.8$. Thus the sex gap shrinks with age. An individual insignificant [interaction term](../../../statistical-model.md#interaction-term) coefficient does not justify deleting the whole interaction: the joint [partial F-test](../../../probability-and-statistics.md#partial-f-test-for-nested-linear-models) for the three interaction terms gives $F=18.6822$ on $(3,28)$ [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom), with $p\simeq7.46\times10^{-7}$.

The [regression residuals](../../../probability-and-statistics.md#regression-residual) are observed minus fitted percentages; their printed five-number summary describes their spread. Direct calculation gives $\mathrm{RSS}=60.2$, so the [residual standard error](../../../statistical-modelling.md#residual-standard-error) is

$$
s=\sqrt{60.2/28}=1.46629\text{ percentage points}.
$$

The [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) is $1-\mathrm{RSS}/\mathrm{TSS}=0.985827$. The overall [F-test](../../../probability-and-statistics.md#f-test) compares all eleven non-intercept coefficients with zero:

$$
F=\frac{(\mathrm{TSS}-\mathrm{RSS})/11}{\mathrm{RSS}/28}=177.053.
$$

Under the null it has an [F-distribution](../../../continuous-probability-distribution.md#f-distribution) on $(11,28)$ [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom); its very small [p-value](../../../statistical-modelling.md#p-value) shows substantial explained variation. This does not independently validate the Gaussian error assumptions. Survey percentages can have different sampling [variances](../../../variance.md) and correlations, and the survey denominators and design are not supplied. The output's exact inferential interpretation is conditional on the stated [normal linear model](../../../statistical-modelling.md#normal-linear-model).

The final command makes an [interaction plot](../../../statistical-model.md#interaction-plot), not another regression fit. Its points are arithmetic averages over the five years for each sex-age combination. **It draws two decreasing, nonparallel lines**, with coordinates

$$
\boxed{\text{men: }(38.4,31.4,25.6,15.4),\qquad\text{women: }(19.6,14.4,11.4,5.8).}
$$

Their gaps are $18.8,17.0,14.2,9.6$ percentage points, illustrating the sex-by-age [statistical interaction](../../../statistical-model.md#interaction-statistics). The average uses the software vector's disputed entry, consistently with the displayed fit. These are means of percentages, not denominator-weighted pooled prevalence estimates.

<a id="1/image-sex-by-age-interaction-plot-averaged-over-years-using-the-printed-software-input"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38-interaction.png)

**[Figure 1](#1/image-sex-by-age-interaction-plot-averaged-over-years-using-the-printed-software-input). Sex-by-age interaction plot averaged over years, using the printed software input**.

## 2

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The prose names a second year that differs from the table label. The calculations use the four supplied counts, interpreting the first and second rows as the two displayed periods; no numerical conclusion depends on resolving that label discrepancy.

The first [generalized linear model](../../../statistical-modelling.md#generalized-linear-model) treats the four counts as independent [Poisson random variables](../../../discrete-probability-distribution.md#poisson-distribution), with a [log link](../../../statistical-modelling.md#logarithmic-link-function) and both row and column [regression factors](../../../statistical-modelling.md#regression-factor). The row-by-column interaction makes the [log-linear model](../../../statistical-modelling.md#log-linear-model) saturated. With $r,c\in\{0,1\}$, write

$$
\log\mu_{rc}=\alpha+\beta r+\gamma c+\delta rc.
$$

Its four [maximum-likelihood fitted values](../../../statistical-modelling.md#maximum-likelihood-fitted-value) equal the observed counts. Thus $\widehat\alpha=\log20$, $\widehat\beta=\log(12/20)$, $\widehat\gamma=\log(9/20)$, and

$$
\widehat\delta=\log\frac{20\cdot11}{9\cdot12}=0.711496.
$$

The interaction is the [log odds ratio](../../../statistical-modelling.md#log-odds-ratio) measuring association of row and column. Under independent Poisson sampling, the delta-method [variances](../../../variance.md) are $1/20$ for the intercept, $1/12+1/20$ for the row contrast, $1/9+1/20$ for the column contrast, and $1/20+1/9+1/12+1/11$ for the interaction. Their square roots reproduce the printed [standard errors](../../../statistical-inference.md#standard-error). Although the software labels the standardized ratios as t values, these are asymptotic normal [Wald statistics](../../../statistical-modelling.md#wald-test), with known [Poisson](../../../discrete-probability-distribution.md#poisson-distribution) dispersion one, not exact finite-df Student tests.

The [statistical saturated model](../../../statistical-modelling.md#saturated-statistical-model) has zero [residual deviance](../../../statistical-modelling.md#residual-deviance) and zero [residual degrees of freedom](../../../statistical-modelling.md#residual-degrees-of-freedom); this is a perfect interpolation, not evidence of predictive adequacy. The null deviance $5.016056$ compares the four observed counts with an intercept-only model, whose four fitted means are $52/4=13$. [Fisher scoring](../../../statistical-modelling.md#scoring-algorithm) is the numerical score/information iteration used to fit the model; the iteration count is a convergence report, not a test statistic.

Dropping the interaction gives the [independence log-linear model for a two-way contingency table](../../../statistical-modelling.md#independence-log-linear-model-for-a-two-way-contingency-table), $\log\mu_{rc}=\alpha+\beta r+\gamma c$. Its [Poisson regression margin-matching score equations](../../../statistical-modelling.md#poisson-regression-margin-matching-score-equations) match the row and column totals, so

$$
\widehat\mu_{rc}=\frac{r_r c_c}{N},\qquad \widehat\mu=\begin{pmatrix}17.846154&11.153846\\14.153846&8.846154\end{pmatrix},\qquad N=52.
$$

Here $r_r$ and $c_c$ denote the observed row and column totals. In particular the fitted row multiplier is $23/29$, the column multiplier is $20/32$, and the intercept is $\log(29\cdot32/52)=2.881788$. These produce the second coefficient table. Their [standard errors](../../../statistical-inference.md#standard-error) follow from the inverse [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix); for the row and column contrasts their squared values are $1/29+1/23$ and $1/32+1/20$, while the intercept [variance](../../../variance.md) is $1/29+1/32-1/52$.

The [Poisson deviance](../../../statistical-modelling.md#poisson-deviance) relative to the saturated fit is

$$
G^2=2\sum_{r,c}y_{rc}\log\frac{y_{rc}}{\widehat\mu_{rc}}=1.527855.
$$

The linear terms cancel because fitted and observed totals agree. The additive model has three coefficients, leaving one [degree of freedom](../../../classical-mechanics.md#degree-of-freedom). [Wilks theorem](../../../statistical-inference.md#wilks-theorem) calibrates this [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) approximately by $\chi^2_1$, giving $p\simeq0.2164$. The interaction [Wald test](../../../statistical-modelling.md#wald-test) instead gives $p\simeq0.2192$; the two are only asymptotically equivalent.

[Fisher's exact test](../../../statistical-modelling.md#fisher-s-exact-test) conditions on both margins under independence. If $X$ is the upper-left count, then

$$
P(X=x)=\frac{\binom{32}{x}\binom{20}{29-x}}{\binom{52}{29}},\qquad9\le x\le29.
$$

Its usual two-sided [p-value](../../../statistical-modelling.md#p-value) sums the probabilities of all tables no more probable than the observed $X=20$. That sum is $0.259724$, reproducing the output without an asymptotic approximation. It tests the same absence of row-column association, but conditioning and discreteness explain the numerical difference from the [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test).

In ordinary language, the male proportion among the cases is $20/29\simeq69.0\%$ in the first row and $12/23\simeq52.2\%$ in the second. The estimated case-sex [odds ratio](../../../statistical-modelling.md#odds-ratio) is $2.037$, but its approximate 95-percent [confidence interval](../../../statistical-inference.md#confidence-interval) is wide, $(0.655,6.338)$. **These small samples do not give convincing evidence that the sex composition of cases changed between the two periods.** Failure to reject is not evidence that the compositions are exactly equal. Nor do these counts establish a male-to-female disease-incidence ratio or an incidence trend: population denominators and comparable ascertainment would be needed for those interpretations.

## 3

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution), the [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\pi)=\sum_{i=1}^n\{y_i\log\pi_i+(1-y_i)\log(1-\pi_i)\}.
$$

Every [likelihood](../../../statistical-modelling.md#likelihood-function) factor is at most one, so $\ell\le0$. In the [statistical saturated model](../../../statistical-modelling.md#saturated-statistical-model), choose $\widehat\pi_i=y_i$ independently for each observation. The probability of each realised response is then exactly one. With the continuous convention $0\log0=0$, the [Bernoulli saturated log-likelihood](../../../statistical-modelling.md#bernoulli-saturated-log-likelihood) is therefore

$$
\boxed{\ell_{\mathrm{sat}}=0\text{ for every binary response vector}.}
$$

The inclusion of probabilities zero and one is important: if the parameter space required $0<\pi_i<1$, zero would be the supremum approached at the boundary, rather than an attained maximum.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The first fit is a [Bernoulli logistic-regression model](../../../statistical-modelling.md#bernoulli-logistic-regression-model) for the probability of a positive response. Its fitted [linear predictor](../../../statistical-modelling.md#linear-predictor) is

$$
\widehat\eta=-9.772794+0.103181\,\mathrm{npreg}+0.032116\,\mathrm{glu}-0.004767\,\mathrm{bp}-0.001917\,\mathrm{skin}+0.083621\,\mathrm{bmi}+1.820337\,\mathrm{ped}+0.041182\,\mathrm{age},
$$

and its fitted [probability](../../../probability-theory.md#probability) is $\widehat\pi=(1+e^{-\widehat\eta})^{-1}$. There are eight coefficients. The null [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) identify $n=200$, and the residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) are $200-8=192$.

Each slope is a change in the [log odds](../../../statistical-modelling.md#log-odds) per unit of its [covariate](../../../statistical-model.md#covariate), holding the others fixed. Exponentiating gives conditional [odds ratios](../../../statistical-modelling.md#odds-ratio); for example a ten-unit glucose increase multiplies fitted odds by $e^{10(0.032115958)}=1.379$, and a ten-year age increase by $e^{10(0.041182353)}=1.510$. These are changes in odds, not multiplicative changes in probability, and the observational associations are not automatically causal effects. The intercept corresponds to all numerical [covariates](../../../statistical-model.md#covariate) being zero, generally an extrapolation beyond meaningful subjects.

The [standard errors](../../../statistical-inference.md#standard-error) come from the inverse [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix) of the [logistic regression](../../../statistical-modelling.md#logistic-regression). With binomial [dispersion parameter](../../../exponential-family.md#dispersion-parameter) fixed at one, the displayed t ratios are asymptotic normal [Wald statistics](../../../statistical-modelling.md#wald-test). In the full fit, glucose and the pedigree measure have clear individual evidence of nonzero slopes, with two-sided $p\simeq2.09\times10^{-6}$ and $0.00609$. The body-mass and age terms are borderline, with $p\simeq0.0504$ and $0.0618$; pregnancy count is weaker, $p\simeq0.110$. Blood pressure and skinfold have little individual evidence after adjustment. These labels should not be converted into a claim that the weaker predictors have no effect, or used as automatic model-selection rules.

A [deviance residual](../../../statistical-modelling.md#deviance-residual) here is

$$
r_i^D=\operatorname{sign}(y_i-\widehat\pi_i)\sqrt{-2\{y_i\log\widehat\pi_i+(1-y_i)\log(1-\widehat\pi_i)\}}.
$$

Its square is the observation's contribution to [binomial deviance](../../../statistical-modelling.md#binomial-deviance), so the squared residuals sum to the printed [residual deviance](../../../statistical-modelling.md#residual-deviance). The five-number summaries describe the distribution of these signed residuals. The null deviance $256.4142$ belongs to an intercept-only [logistic regression](../../../statistical-modelling.md#logistic-regression); the full fitted deviance is $178.3907$. Four [Fisher scoring](../../../statistical-modelling.md#scoring-algorithm) iterations record convergence of the numerical likelihood fit.

The second model uses only glucose:

$$
\widehat\eta=-5.503635+0.03778371\,\mathrm{glu}.
$$

Its two coefficients leave $198$ residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom). A ten-unit glucose increase multiplies its fitted odds by $e^{0.3778371}\simeq1.459$. This differs from the adjusted multiplier $1.379$, because the models condition on different [covariates](../../../statistical-model.md#covariate); both adjustment and [noncollapsibility of the odds ratio](../../../statistical-modelling.md#noncollapsibility-of-the-odds-ratio) can change logistic coefficients. The glucose-only model has deviance $207.3727$, so its maximized [log-likelihood](../../../statistical-modelling.md#log-likelihood) is lower than the full model's.

For these fixed-dimensional nested models, [analysis of deviance](../../../statistical-modelling.md#analysis-of-deviance-for-nested-generalized-linear-models) and [Wilks theorem](../../../statistical-inference.md#wilks-theorem) give

$$
\begin{array}{c|c|c|c}
\text{comparison}&\text{deviance reduction}&\text{df}&\text{approximate }p\\\hline
\text{null to full}&78.0235&7&3.48\times10^{-14}\\
\text{null to glucose only}&49.0415&1&2.51\times10^{-12}\\
\text{glucose only to full}&28.9820&6&6.13\times10^{-5}
\end{array}
$$

Thus **the additional six predictors collectively improve the glucose-only model**, even though several individual [Wald tests](../../../statistical-modelling.md#wald-test) are not significant. These comparisons assume independent subjects, an appropriate logistic mean structure, full rank, and regular finite parameter estimates without [separation](../../../set-theory.md#axiom-schema-of-specification).

It would be incorrect to infer that absolute fit is good merely because $178.39<192$. [Individual Bernoulli deviance need not have a chi-squared calibration](../../../statistical-modelling.md#individual-bernoulli-deviance-need-not-have-a-chi-squared-calibration): there is just one binary observation per saturated probability, and the saturated dimension increases with sample size. A simple counterexample is an intercept-only model with true probability $1/2$, for which $D/n\to2\log2$, not one. For absolute adequacy, inspect residual patterns and predicted-risk calibration, use meaningful grouped comparisons when appropriate, or calibrate a chosen fit statistic by [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap). The regular nested-model tests above are not subject to that saturated-model dimensionality problem. Only the displayed summaries and a few example rows are supplied, so patient-level diagnostics or complete numerical refitting cannot be reconstructed from this page alone.

## 4

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use $\alpha$ for the intercept, to avoid confusing it with the observation means. Let $e_i=\exp(\widehat\alpha+\widehat\beta^Tx_i)$ be the fitted [Poisson regression](../../../statistical-modelling.md#poisson-regression) mean. Apart from constants, its [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\alpha,\beta)=\sum_i\{y_i(\alpha+\beta^Tx_i)-\exp(\alpha+\beta^Tx_i)-\log(y_i!)\}.
$$

At a finite interior [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator), the intercept [score equation](../../../statistical-modelling.md#score-equation) gives the [Poisson regression margin-matching score equations](../../../statistical-modelling.md#poisson-regression-margin-matching-score-equations):

$$
\frac{\partial\ell}{\partial\alpha}=\sum_i(y_i-e_i)=0,\qquad\boxed{\sum_i e_i=\sum_i y_i.}
$$

The [statistical saturated model](../../../statistical-modelling.md#saturated-statistical-model) fits each mean to $y_i$, taking the boundary mean zero if $y_i=0$. Subtracting fitted from saturated [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives the [Poisson deviance](../../../statistical-modelling.md#poisson-deviance)

$$
D=2\sum_i\left[y_i\log\frac{y_i}{e_i}-(y_i-e_i)\right].
$$

The intercept balance cancels the sum of linear terms. Consequently

$$
\boxed{D=2\sum_i y_i\log(y_i/e_i),\qquad0\log(0/e_i)=0.}
$$

The unsimplified formula makes nonnegativity transparent; individual terms in the simplified formula need not each be positive.

For the [deviance goodness-of-fit test](../../../statistical-modelling.md#deviance-goodness-of-fit-test), if the fitted design has rank $r$, compare a suitably calibrated $D$ with $\chi^2_{n-r}$, rejecting for large values. This approximation applies in a regular large-count regime, such as a fixed set of cells with increasing exposure and positive fitted proportions. It is not automatically accurate for many sparse [Poisson](../../../discrete-probability-distribution.md#poisson-distribution) observations. Check residual patterns and [overdispersion](../../../exponential-family.md#overdispersion); where the approximation is doubtful, simulate independent [Poisson random variables](../../../discrete-probability-distribution.md#poisson-distribution) with fitted means, refit each sample, and use a [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap) distribution of the same statistic. A large [p-value](../../../statistical-modelling.md#p-value) means no detected lack of fit, not proof of the model. If a finite interior estimate fails to exist, the score proof needs a boundary-limit interpretation; for example all-zero data give a supremum with every fitted mean tending to zero and limiting deviance zero.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Here the [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) has mean parameter $\mu>0$ and size parameter $\theta>0$. Its support in the original PDF is all nonnegative integers; a finite endpoint appearing in the TeX aid would be incorrect. The [probability generating function](../../../probability-theory.md#probability-generating-function), obtained from the generalized binomial series, is

$$
G(s)=\left(\frac{\theta}{\theta+\mu(1-s)}\right)^\theta.
$$

Differentiating at one gives $G'(1)=\mu$ and $G''(1)=\mu^2(1+1/\theta)$. Since the [variance](../../../variance.md) is $G''(1)+G'(1)-G'(1)^2$, this proves

$$
\boxed{\mathbb E Y=\mu,\qquad\operatorname{Var}(Y)=\mu+\mu^2/\theta.}
$$

The extra positive term explains its [overdispersion](../../../exponential-family.md#overdispersion) relative to a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution).

For one observation, write the [log-likelihood](../../../statistical-modelling.md#log-likelihood) as

$$
\ell_y=\log\Gamma(\theta+y)-\log\Gamma(\theta)-\log(y!)+y\log\mu+\theta\log\theta-(\theta+y)\log(\mu+\theta).
$$

The mean [score function](../../../statistical-modelling.md#informant-function) and its cross derivative are

$$
u_\mu=\frac{y}{\mu}-\frac{\theta+y}{\mu+\theta}=\frac{\theta(y-\mu)}{\mu(\mu+\theta)},\qquad \frac{\partial u_\mu}{\partial\theta}=\frac{y-\mu}{(\mu+\theta)^2}.
$$

Taking [expectations](../../../probability-theory.md#expected-value) gives $I_{\mu\theta}=-\mathbb E(\partial_\theta u_\mu)=0$. In addition,

$$
I_{\mu\mu}=\frac{\theta}{\mu(\mu+\theta)}=\frac1{\mu+\mu^2/\theta}.
$$

For reference, with $\psi$ the [digamma function](../../../complex-analysis.md#digamma-function), the size [score function](../../../statistical-modelling.md#informant-function) is

$$
u_\theta=\psi(\theta+y)-\psi(\theta)+\log\theta+1-\log(\mu+\theta)-\frac{\theta+y}{\mu+\theta}.
$$

Its [variance](../../../variance.md) $I_{\theta\theta}$ is finite and positive for finite positive $\mu,\theta$. Thus [negative binomial mean-size parameter orthogonality](../../../statistical-modelling.md#negative-binomial-mean-size-parameter-orthogonality) makes the expected [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix) diagonal. For an independent identically distributed sample and a regular identifiable interior true parameter, [asymptotic normality of a maximum likelihood estimator](../../../statistical-modelling.md#asymptotic-normality-of-a-maximum-likelihood-estimator) gives

$$
\sqrt n\begin{pmatrix}\widehat\mu-\mu\\\widehat\theta-\theta\end{pmatrix}\xrightarrow d N_2\left(0,\begin{pmatrix}\mu+\mu^2/\theta&0\\0&I_{\theta\theta}^{-1}\end{pmatrix}\right).
$$

Hence **the asymptotic correlation is zero**. This is first-order asymptotic independence, not a claim of exact finite-sample independence. Indeed the mean score yields $\widehat\mu=\bar y$ at an interior fit, while the size fit also depends on the observed dispersion. The argument excludes a true boundary such as the Poisson limit $\theta=\infty$.

## 5

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

**The independence analysis is not justified without further assumptions.** Three binary responses from the same subject generally remain correlated after conditioning on baseline [covariates](../../../statistical-model.md#covariate) and treatment. The fitted independent-Bernoulli [likelihood](../../../statistical-modelling.md#likelihood-function) discards that correlation and gives incorrect model-based [standard errors](../../../statistical-inference.md#standard-error) and tests if it is present. Positive within-subject correlation commonly makes those errors too small.

There is an important distinction between estimating the mean and estimating uncertainty. If the stated marginal [logistic regression](../../../statistical-modelling.md#logistic-regression) is correct and responses are fully observed, the independence score $\sum_{i,j}w_{ij}(Y_{ij}-m_{ij})$ still has zero [expectation](../../../probability-theory.md#expected-value). With independent subjects and regularity, its root can consistently estimate marginal coefficients despite within-subject dependence; a subject-level [sandwich covariance matrix](../../../statistical-inference.md#sandwich-covariance-matrix) is then needed. True independence is a special case in which the original [standard errors](../../../statistical-inference.md#standard-error) would be appropriate.

Dropout creates a separate issue. Restricting that score to observed responses need not preserve its zero [expectation](../../../probability-theory.md#expected-value) if observation depends on the response history or unseen depression outcomes. Therefore both point estimates and uncertainty may be wrong. Neither random treatment assignment nor baseline adjustment alone establishes an [ignorable missingness mechanism](../../../probability-and-statistics.md#ignorable-missingness-mechanism). We need a model matched to the scientific estimand and explicit assumptions about [missing data](../../../probability-and-statistics.md#missing-data).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/a">a</h4>

↑ **Parent:** [Ii](#5/ii)

<h5 id="5/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#5/ii/a)

For a population question use a [population-averaged logistic model for repeated binary outcomes](../../../statistical-inference.md#population-averaged-logistic-model-for-repeated-binary-outcomes). Code $z_i=1$ for the new treatment and $0$ for the control, with visit times $t_j=2j$ months for $j=1,2,3$. Let $w_{ij}=(1,z_i,x_i^T,t_j)^T$, $\gamma_M=(\alpha_M,\phi_M,\beta_M^T,\delta_M)^T$, and

$$
m_{ij}=P(Y_{ij}=1\mid z_i,x_i,t_j),\qquad\operatorname{logit}m_{ij}=w_{ij}^T\gamma_M.
$$

Different subjects are independent. Each response has a [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) with this marginal mean, but no independence of a subject's three responses is assumed. The linear time effect and absence of treatment-by-time [interaction](../../../statistical-model.md#interaction-statistics) are substantive mean assumptions; if inappropriate they can be replaced by time indicators and [interaction terms](../../../statistical-model.md#interaction-term).

For complete data, set $m_i=(m_{i1},m_{i2},m_{i3})^T$, $A_i=\operatorname{diag}(m_{ij}(1-m_{ij}))$, and $D_i=\partial m_i/\partial\gamma_M^T=A_iW_i$, where $W_i$ has rows $w_{ij}^T$. A working exchangeable [correlation matrix](../../../variance.md#correlation-matrix) has unit diagonal and off-diagonal value $\rho\in(-1/2,1)$; set $V_i=A_i^{1/2}C(\rho)A_i^{1/2}$. The [generalized estimating equation](../../../statistical-inference.md#generalized-estimating-equation) is

$$
\sum_iD_i^TV_i^{-1}(Y_i-m_i)=0.
$$

With correct means and independent subjects, a positive-definite working [covariance matrix](../../../variance.md#covariance-matrix) and regularity give consistency even if the working correlation is wrong. Write $H=\sum_iD_i^TV_i^{-1}D_i$ and $u_i=D_i^TV_i^{-1}(Y_i-m_i)$. The fitted subject-level [sandwich covariance matrix](../../../statistical-inference.md#sandwich-covariance-matrix) is

$$
\widehat{\operatorname{Var}}(\widehat\gamma_M)=H^{-1}\left(\sum_i u_iu_i^T\right)H^{-1},
$$

evaluated at the estimates. This inference is asymptotic in the number of independent subjects, not the number of visits.

For the actual incomplete data, define $R_{ij}=1$ if visit $j$ is observed, with $R_{i0}=1$ and monotone dropout. Let $\mathcal H_{i,j-1}$ contain treatment, baseline [covariates](../../../statistical-model.md#covariate) and responses observed before visit $j$. Under sequential [missing at random](../../../probability-and-statistics.md#missing-at-random), specify

$$
q_{ij}=P(R_{ij}=1\mid R_{i,j-1}=1,\mathcal H_{i,j-1}),\qquad \rho_{ij}=\prod_{k=1}^j q_{ik}>0.
$$

The assumption is that the retention decision, conditional on this history, does not additionally depend on unseen current or future outcomes. Fit the $q_{ij}$, for example by visit-specific [logistic regressions](../../../statistical-modelling.md#logistic-regression). A simple valid choice uses working independence and the [inverse-observation-weighted estimating equations for longitudinal dropout](../../../statistical-inference.md#inverse-observation-weighted-estimating-equations-for-longitudinal-dropout):

$$
\boxed{\sum_i\sum_{j=1}^3 w_{ij}\frac{R_{ij}}{\rho_{ij}}(Y_{ij}-m_{ij})=0.}
$$

Terms with $R_{ij}=0$ are zero and require no missing response. Given the full response vector, sequential [missing at random](../../../probability-and-statistics.md#missing-at-random) makes $\mathbb E(R_{ij}/\rho_{ij}\mid Y_i,z_i,x_i)=1$. Consequently the weighted score has the same [expectation](../../../probability-theory.md#expected-value) as the complete-data score, proving its mean-zero property. Correct retention probabilities, positivity and a correctly specified marginal mean are required. Use cluster-robust uncertainty, accounting for fitted retention-model coefficients, or resample entire subjects and refit both models. Under [missing completely at random](../../../probability-and-statistics.md#missing-completely-at-random), the simpler unweighted observed-response [GEE](../../../statistical-inference.md#generalized-estimating-equation) can suffice; ordinary unweighted [GEE](../../../statistical-inference.md#generalized-estimating-equation) is not valid under arbitrary history-dependent [missing at random](../../../probability-and-statistics.md#missing-at-random).

The treatment coefficient gives a population conditional-on-baseline [odds ratio](../../../statistical-modelling.md#odds-ratio) $e^{\phi_M}$ at each visit. To communicate an absolute population treatment benefit, standardize predicted [probabilities](../../../probability-theory.md#probability) over the full baseline population, rather than only completers:

$$
\widehat p_z(t)=\frac1m\sum_i\operatorname{logit}^{-1}(\widehat\alpha_M+\widehat\phi_M z+\widehat\beta_M^Tx_i+\widehat\delta_M t),\qquad \widehat p_1(t)-\widehat p_0(t).
$$

A causal reading additionally uses the [randomized controlled trial](../../../causal-inference.md#randomized-controlled-trial) assignment, consistency of the treatment definition, no interference and the dropout assumptions; the statistical model alone does not supply those conditions.

<h4 id="5/ii/b">b</h4>

↑ **Parent:** [Ii](#5/ii)

<h5 id="5/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#5/ii/b)

For conditional individual response profiles use a [logistic random-intercept model for repeated binary outcomes](../../../statistical-modelling.md#logistic-random-intercept-model-for-repeated-binary-outcomes). Introduce a subject effect $B_i\sim N(0,\tau^2)$ independently across subjects and independently of treatment and baseline [covariates](../../../statistical-model.md#covariate), under the specified model. Conditional on $B_i,z_i,x_i$, assume the three responses are independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) with

$$
p_{ij}(b)=P(Y_{ij}=1\mid B_i=b,z_i,x_i),\qquad \operatorname{logit}p_{ij}(b)=\alpha_C+\phi_C z_i+\beta_C^Tx_i+\delta_C t_j+b.
$$

Here $B_i$ is persistent unmeasured subject heterogeneity and $\tau^2$ its [variance](../../../variance.md). It induces dependence after integration: for distinct visits, the response [covariance](../../../variance.md#covariance) is $\operatorname{Cov}_B(p_{ij}(B),p_{ik}(B))$, generally positive. This is a complete joint [generalized linear mixed model](../../../statistical-modelling.md#generalized-linear-mixed-model), unlike a mean-only [GEE](../../../statistical-inference.md#generalized-estimating-equation) specification.

Under [missing at random](../../../probability-and-statistics.md#missing-at-random) conditional on the observed responses and baseline variables, with [distinct parameters](../../../probability-and-statistics.md#distinct-parameters) for missingness and outcomes, the missingness model is ignorable for likelihood inference. Let $\mathcal O_i=\{j:R_{ij}=1\}$. The outcome [observed-data likelihood](../../../statistical-modelling.md#observed-data-likelihood) is

$$
L(\gamma_C,\tau^2)=\prod_i\int_{-\infty}^{\infty}\prod_{j\in\mathcal O_i}p_{ij}(b)^{y_{ij}}[1-p_{ij}(b)]^{1-y_{ij}}\frac{e^{-b^2/(2\tau^2)}}{\sqrt{2\pi\tau^2}}\,db.
$$

The omitted Bernoulli factors sum to one over missing outcomes. Fit the fixed coefficients and $\tau^2$ by maximizing this integrated [likelihood](../../../statistical-modelling.md#likelihood-function), with suitable quadrature or another justified integration method. If $\tau=0$, use the limiting point-mass model. Correct response and random-effect distributions, identifiable coefficients and regularity are needed; the latent distribution assumption is not merely a convenient working covariance.

For patient $i$, combine the fitted model with the posterior density of $B_i$ proportional to its normal density times that patient's observed Bernoulli factors. Integrating $p_{ij}(b)$ over this posterior gives a patient-specific predicted response profile. The treatment [odds ratio](../../../statistical-modelling.md#odds-ratio) for a fixed $b$ and the same baseline variables is $e^{\phi_C}$. This conditional contrast does not by itself identify each person's unobserved causal treatment effect: a parallel-arm trial observes only one treatment per person. Random slopes or heterogeneous treatment effects require further modelling and sufficient information; they are not implied by fitting a [random intercept](../../../statistical-modelling.md#random-intercept).

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

The [population-averaged logistic regression](../../../statistical-inference.md#population-averaged-logistic-model-for-repeated-binary-outcomes) describes $P(Y_{ij}=1\mid z_i,x_i)$ after averaging over unmeasured individual heterogeneity. Its intercept is a marginal [log odds](../../../statistical-modelling.md#log-odds) at reference baseline values and time zero, its treatment coefficient is a population conditional-on-baseline [log odds ratio](../../../statistical-modelling.md#log-odds-ratio), and its time coefficient is the change in that marginal [log odds](../../../statistical-modelling.md#log-odds) per month. Time zero is an extrapolation here because the recorded visits begin later; centring time at the first visit would give a more interpretable intercept.

In the [random-intercept logistic model](../../../statistical-modelling.md#logistic-random-intercept-model-for-repeated-binary-outcomes), the intercept is instead the conditional [log odds](../../../statistical-modelling.md#log-odds) for a subject with $B_i=0$. The treatment and time coefficients apply at fixed $B_i$; the subject's actual intercept is $\alpha_C+B_i$. Even with a treatment-independent [random intercept](../../../statistical-modelling.md#random-intercept), the conditional and marginal coefficients generally differ through [noncollapsibility of the odds ratio](../../../statistical-modelling.md#noncollapsibility-of-the-odds-ratio). Indeed, if $\eta=\alpha_C+\phi_Cz+\beta_C^Tx+\delta_Ct$, marginalization gives

$$
M(\eta)=\mathbb E_B[\operatorname{logit}^{-1}(\eta+B)],
$$

which is not generally a logistic curve with the same linear coefficients. To quantify [random-intercept attenuation of marginal logistic slopes](../../../statistical-modelling.md#random-intercept-attenuation-of-marginal-logistic-slopes), let $p_B=\operatorname{logit}^{-1}(\eta+B)$. Then

$$
M'=\mathbb E[p_B(1-p_B)]=M(1-M)-\operatorname{Var}(p_B),\qquad \frac{d\operatorname{logit}M}{d\eta}=1-\frac{\operatorname{Var}(p_B)}{M(1-M)}.
$$

For a nondegenerate finite [random intercept](../../../statistical-modelling.md#random-intercept) this derivative lies strictly between zero and one and usually varies with $\eta$. Thus the marginal treatment contrast is an integrated, attenuated version of the conditional contrast, and the marginal time slope need not be constant. One should not equate the two sets of coefficients, even in a [randomized controlled trial](../../../causal-inference.md#randomized-controlled-trial) without treatment confounding.

For [missing completely at random](../../../probability-and-statistics.md#missing-completely-at-random), an unweighted observed-response [GEE](../../../statistical-inference.md#generalized-estimating-equation) with cluster-robust [standard errors](../../../statistical-inference.md#standard-error) can consistently fit the marginal mean, and a correctly specified integrated [GLMM](../../../statistical-modelling.md#generalized-linear-mixed-model) likelihood is valid as well. Under [missing at random](../../../probability-and-statistics.md#missing-at-random) depending on previous observed outcomes, ordinary unweighted [GEE](../../../statistical-inference.md#generalized-estimating-equation) is generally biased because the remaining responses are selected by informative observed history. Correct [inverse-observation-weighted estimating equations for longitudinal dropout](../../../statistical-inference.md#inverse-observation-weighted-estimating-equations-for-longitudinal-dropout) recover the marginal target under the sequential MAR and positivity assumptions already stated. Covariate-only observation mechanisms are a simpler special case in which correctly conditioned unweighted mean equations can remain valid.

A correctly specified joint response [GLMM](../../../statistical-modelling.md#generalized-linear-mixed-model), fitted by [observed-data likelihood](../../../statistical-modelling.md#observed-data-likelihood), is valid under ignorable [missing at random](../../../probability-and-statistics.md#missing-at-random) with [distinct parameters](../../../probability-and-statistics.md#distinct-parameters), including dependence of missingness on observed response history. This is a likelihood property, not a claim that every mixed model automatically fixes missingness. Under [missing not at random](../../../probability-and-statistics.md#missing-not-at-random), neither ordinary [GEE](../../../statistical-inference.md#generalized-estimating-equation), MAR-based weights nor a response-only [GLMM](../../../statistical-modelling.md#generalized-linear-mixed-model) is generally valid; the unseen-outcome dependence requires further modelling and sensitivity assumptions.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

First investigate what predicts dropout among variables actually observed, record reasons where possible, and seek additional outcome follow-up. Dependence on observed history alone can be [missing at random](../../../probability-and-statistics.md#missing-at-random); informative dependence on unseen responses or latent heterogeneity requires a [missing not at random](../../../probability-and-statistics.md#missing-not-at-random) analysis. Observed data do not ordinarily distinguish MAR from all MNAR explanations.

An explicit [selection model for informative longitudinal dropout](../../../probability-and-statistics.md#selection-model-for-informative-longitudinal-dropout) can augment a joint response model $f_\vartheta(Y_i\mid z_i,x_i)$ by dropout hazards. Define $R_{ij}$ as above and, among subjects retained through visit $j-1$, put

$$
h_{ij}(Y_i)=P(R_{ij}=0\mid R_{i,j-1}=1,Y_i,z_i,x_i),\qquad \operatorname{logit}h_{ij}=a_j+c^Tx_i+d z_i+\lambda Y_{i,j-1}+\kappa Y_{ij}.
$$

Omit the previous-response term at the first visit. A nonzero $\kappa$ makes dropout depend on the currently missing response. For monotone observation indicators $r_i$, let

$$
g_\eta(r_i\mid Y_i,z_i,x_i)=\prod_{j:r_{i,j-1}=1}h_{ij}(Y_i)^{1-r_{ij}}[1-h_{ij}(Y_i)]^{r_{ij}}.
$$

The appropriate [observed-data likelihood](../../../statistical-modelling.md#observed-data-likelihood) is

$$
L(\vartheta,\eta)=\prod_i\sum_{Y_i^{\mathrm{mis}}\in\{0,1\}^{|\mathcal O_i^c|}} f_\vartheta(Y_i^{\mathrm{obs}},Y_i^{\mathrm{mis}}\mid z_i,x_i)\,g_\eta(r_i\mid Y_i,z_i,x_i).
$$

Thus a patient's dropout pattern contributes information in the model; dropping the $g_\eta$ factor is not justified under this informative mechanism.

Another option is a [shared-parameter model for informative dropout](../../../probability-and-statistics.md#shared-parameter-model-for-informative-dropout): retain the conditional Bernoulli response model, but let the dropout [logit](../../../statistical-modelling.md#logit) contain the same latent effect, for example $a_j+c^Tx_i+d z_i+\lambda Y_{i,j-1}+\kappa_B B_i$. Conditional on the shared effect and observed history the processes can be independent, while marginally dropout remains associated with unseen responses. The joint [likelihood](../../../statistical-modelling.md#likelihood-function) must integrate the response factors and dropout factors together over $B_i$. A response-only mixed-model fit does not generally account for this dependence.

Because $\kappa$ or $\kappa_B$ can be weakly identified from the observed outcomes, **report sensitivity of the treatment conclusion to plausible informative-dropout assumptions**. One can fix a range of these dependence parameters and refit, or use [pattern-mixture sensitivity analysis](../../../probability-and-statistics.md#pattern-mixture-sensitivity-analysis) that shifts the imputed post-dropout [log odds](../../../statistical-modelling.md#log-odds) by a specified amount from the MAR prediction. Present population risks and treatment contrasts across these scenarios with their uncertainty. These are explicit identifying assumptions, not an empirical test proving which missingness mechanism is true. Neither a complete-case analysis nor carrying forward the last response supplies such a justification.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
